# Breaches and Leaks Threat Intel

## Trufflehog

**Description:** Find leaked credentials in:
git
github
gitlab
S3
filesystem
syslog

`sudo docker run -it -v "$PWD:/pwd" trufflesecurity/trufflehog:latest s3 --help`

Command above is running the app from docker, then searching s3, then running the help command

`sudo docker run -it -v "$PWD:/pwd" trufflesecurity/trufflehog:latest s3 --bucket=http://trinet-logs.s3.amazonaws.com/`


## h8mail

**Description:** A tool to parse emails against Breach Data intel feeds as well as your own local Breach Databases

Generate a config file to put your API keys in

`/usr/local/bin$ sudo ./h8mail --gen-config`

The config file is named h8mail_config.ini)

`h8mail -t /home/sh1katagana1/my_emails -c /home/sh1katagana1/osint/h8mail/h8mail_config.ini -o /home/sh1katagana1/pwned/pwned_targets.csv`

When I want to use one of my local breach files, I do: 

`h8mail -t leroyjenkins@gmail.com -lb '5000000 Gmail.txt' -sk`

To search emails using Compilation Of Many Breaches, I do: 

`h8mail -t dabluezpreacher@gmail.com -sk -bc CompilationOfManyBreaches`

I can also replace my email with a text file of emails
 
To search just by domain: 

`h8mail -t example.com fcorp.com -sk -lb ./CompilationOfManyBreaches/ --loose`

--loose param tells h8mail to accept any type of input, instead of enforcing the email pattern.
-lb param tells h8mail to perform a standard local breach search using multiprocessing.

To search for specific passwords: 

`h8mail -t "Yourefired" "Another_s3cretP@ss" -sk -lb ./CompilationOfManyBreaches/ --loose`


Query for a single target

`h8mail -t target@example.com`

Query for list of targets, indicate config file for API keys, output to pwned_targets.csv

`h8mail -t targets.txt -c config.ini -o pwned_targets.csv`

Query a list of targets against local copy of the Breach Compilation, pass API key for Snusbase from the command line

`h8mail -t targets.txt -bc ../Downloads/BreachCompilation/ -k "snusbase_token=$snusbase_token"`

Query without making API calls against local copy of the Breach Compilation

`h8mail -t targets.txt -bc ../Downloads/BreachCompilation/ -sk`

Search every .gz file for targets found in targets.txt locally, skip default checks

`h8mail -t targets.txt -gz /tmp/Collection1/ -sk`

Check a cleartext dump for target. Add the next 10 related emails to targets to check. Read keys from CLI

`h8mail -t admin@evilcorp.com -lb /tmp/4k_Combo.txt -ch 10 -k "hunterio=ABCDE123"`

Query username. Read keys from CLI

`h8mail -t JSmith89 -q username -k "dehashed_email=user@email.com" "dehashed_key=ABCDE123"`

Query IP. Chase all related targets. Read keys from CLI

`h8mail -t 42.202.0.42 -q ip -c h8mail_config_priv.ini -ch 2 --power-chase`

Fetch URL content (CLI + file). Target all found emails

`h8mail -u "https://pastebin.com/raw/kQ6WNKqY" "list_of_urls.txt"`



