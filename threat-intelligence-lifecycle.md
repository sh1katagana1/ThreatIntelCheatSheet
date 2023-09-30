# Threat Intelligence Lifecycle

To be effective at Threat Intelligence, its important to follow a documented plan of action. For threat intelligence, this comes in the form of the Threat Intelligence Lifecycle. Your company may ask to you to generate a report regarding a known threat targeting their industry. Following this lifecycle can make this task more efficient

## Planning and Direction
Here is where you set goals, also known as requirements (sometimes called PIRs). This is where the Threat Intel team meets with other teams to discuss what types of intelligence would benefit them, kind of like seeing them as "customers" of the Threat Intel program. Without requirements, the program is almost rudderless and likely will not be able to be measured properly for its value. Some examples may be: \
1. Identify initial access brokers targeting your industry.
2. What is the most common ransomware delivery method they would use?

## Collection
This is where you get the raw data needed to analyze. A common way is to use a Threat Intel Platform and have multiple Threat Intel feeds sourcing it with all kinds of raw data on threats. Some may or may not be relevant to your organization, but that is where the third phase of Processing comes in. the price of the Intel Feed can influence the quality of the data, so do some research into what Intel Feeds would give you the most quality data

## Processing and Analysis
This is where you enrich the raw data you collected. Once again, a tool like a Threat Intel Platform can provide enrichment for the data mapping and correlating it for you to analzye. Here we sort for false positives and redunant data and remove these. We also use tools for enrichment, like Shodan, which can give more detail about a data point like an IP address. We keep and formulate the data that is relevant for our organization, and connect any similar attributes to it. 

## Dissemination
Once you have parsed out the relevant data and did the proper correlation to APTs and TTPs, it needs to be cataloged and sent to the teams that need it. We have already determined what typ eof data needs to go to what team from our first phase of Planning and Direction. Now we need to give the intel to them in a way that they can consume it. It may be wise to make multiple versions of these reports with varying levels of verbosity and technical details depending on the audience. 

## Feedback
This is mainly used to determine metrics for things like KPIs. Was the Intelligence I delivered useful and accurate?
