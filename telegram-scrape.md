
# Telegram Channel Search Script

This would be if you had a list of keywords you were wanting to check against a specific Telegram channel for any mentions of them. This is useful if you have a list of vendor names you use and want to see if they are showing up in ransomware victim blogs, by searching them against a channel like Ransomwatcher. 

## Instructions
1. First you have to create a free Telegram app from the web Telegram page to get an AppID and an AppHash https://core.telegram.org/api/obtaining_api_id
2. Install the required library:
```
pip install telethon
```

3. Replace the placeholders in the script:
```
YOUR_API_ID: Your Telegram API ID.
YOUR_API_HASH: Your Telegram API hash.
YOUR_PHONE_NUMBER: Your Telegram account's phone number. Make sure you use the format +15555555555
CHANNEL_USERNAME_OR_ID: The username or ID of the channel you want to search. Go to the Telegram channel and look for the @username but do not include @
```
5. Create a text file named keywords.txt in the same directory as the script. Add one keyword per line.
6. Run the script. It will search the last 1000 messages in the specified channel for the keywords. This can be modified to whatever you want. 
7. The script will save the results in a CSV file named search_results.csv.

## What is the script doing?
1. Connects to the Telegram API using your credentials.
2. Reads keywords from the keywords.txt file.
3. Searches the last 1000 messages in the specified channel.
4. If a keyword is found in a message, it saves the date, message text, and the matching keyword to the CSV file.
5. The search is case-insensitive. The re.IGNORECASE flag makes the search case-insensitive.
6. The csv.writer includes a third column labeled Matched Phrase. When writing each row to the CSV file, it includes the keyword that was found in the message. This ensures that each entry in the CSV not only records the date and message but also specifies which keyword triggered the entry. This modification allows you to easily identify which keyword was matched with each message directly in your CSV output.
7. It uses re.search() with word boundaries (\b) to ensure we're matching whole phrases.
8. re.escape(phrase) is used to escape any special regex characters in the phrase.
9. Added encoding='utf-8' when opening the keywords file to ensure proper handling of non-ASCII characters.

## Script

```
from telethon import TelegramClient, events
from telethon.tl.types import InputPeerChannel
import asyncio
import csv
import re

# Replace these with your own API credentials
api_id = 'YOUR_API_ID'
api_hash = 'YOUR_API_HASH'
phone_number = 'YOUR_PHONE_NUMBER'

# Channel username or ID to search
channel_username = 'CHANNEL_USERNAME_OR_ID'

# File containing keywords/phrases
keywords_file = 'keywords.txt'

# Output CSV file
output_file = 'search_results.csv'

# Read keywords/phrases from file
with open(keywords_file, 'r', encoding='utf-8') as f:
    keywords = [line.strip() for line in f]

async def main():
    async with TelegramClient('session', api_id, api_hash) as client:
        await client.start(phone=phone_number)
        
        # Get the channel entity
        channel = await client.get_entity(channel_username)
        
        # Open CSV file for writing results
        with open(output_file, 'w', newline='', encoding='utf-8') as csvfile:
            writer = csv.writer(csvfile)
            writer.writerow(['Date', 'Message', 'Matched Phrase'])
            
            # Search for keywords/phrases in the last 1000 messages
            async for message in client.iter_messages(channel, limit=1000):
                if message.text:
                    for phrase in keywords:
                        # Use regex to find whole phrase, case-insensitive
                        if re.search(r'\b' + re.escape(phrase) + r'\b', message.text, re.IGNORECASE):
                            writer.writerow([message.date, message.text, phrase])
                            break  # Move to next message after finding a match

        print(f"Search complete. Results saved to {output_file}")

asyncio.run(main())
```
