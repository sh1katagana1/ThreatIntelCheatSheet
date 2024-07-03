# Daily Threat Research

## Vulnerabilities and Zero Days and Research
**ExploitAlert** https://exploitalert.com/browse-exploit.html \
**CXSecurity** https://cxsecurity.com/ \
**Vulnerability Lab** https://www.vulnerability-lab.com/ \
**Sploitus** https://sploitus.com/ \
**ExploitDB** https://www.exploit-db.com/ \
**Oday Today** https://0day.today/ \
**Debricked** https://debricked.com/vulnerability-database \
**Github Advisories** https://github.com/advisories \
**Online Threat Alerts** https://www.onlinethreatalerts.com/categories/latest/ \
**Talos Intelligence** https://talosintelligence.com/vulnerability_info \
**Zero Day Initiative** https://www.zerodayinitiative.com/advisories/published/ \
**WordPress Vulnerabilities** https://patchstack.com/database/ \
**VulDB** https://vuldb.com/ \
**PacketStorm** https://packetstormsecurity.com/ \
**Full Disclosure** https://seclists.org/fulldisclosure/ \
**Vulners** https://vulners.com/search?query=viewCount:[50%20TO%20*]%20order:viewCount%20last%207%20days \
**Reddit NetSec** https://www.reddit.com/r/netsec/ \
**CVE Trends** https://cvetrends.com/ \
**CVExploits** https://cvexploits.io/ \
**DateBreaches.net** https://www.databreaches.net/news/ \
**Breach Forums** https://breachforums.vc/ \
**Black Forums** https://blackforums.net/ \
**Ransomlooker** https://cybernews.com/ransomlooker/ A good site to track the latest ransomware groups statistics \
**Phishy Domains** https://phishydomains.com/ This is to check domains registered in past 24 hours based on keywords \
**Infostealers** https://www.infostealers.com/ \
**Ransomchat** https://ransomch.at/Akira-20230606 An interesting viewer of ransomware chats with victims \
**Dark Mirror** https://socradar.io/labs/darkmirror  Dark Web news \
**CVE Crowd** https://cvecrowd.com/ Trending CVEs 


## CVEMAP
Navigate the Common Vulnerabilities and Exposures (CVE) jungle with ease using CVEMAP, a command-line interface (CLI) tool designed to provide a structured and easily navigable interface to various vulnerability databases. \
https://github.com/projectdiscovery/cvemap \
Features:
1. CVE Dataset Search & Query
2. CVE to EPSS Mapping
3. CVE to KEV Mapping
4. CVE to CPE Mapping
5. CVE to GitHub POCs Mapping
6. CVE to Nuclei Template Mapping
7. CVE to HackerOne report Mapping
8. Customizable Filters on CVE data
9. STDIN Input / JSONL Output


Install
```
go install github.com/projectdiscovery/cvemap/cmd/cvemap@latest
```
Setup API Key. (required, but you can sign up for free)
```
cvemap -auth


   ______   _____  ____ ___  ____  ____
  / ___/ | / / _ \/ __ \__ \/ __ \/ __ \
 / /__ | |/ /  __/ / / / / / /_/ / /_/ /
 \___/ |___/\___/_/ /_/ /_/\__,_/ .___/ 
                               /_/
            

    projectdiscovery.io

[INF] Get your free api key by signing up at https://cloud.projectdiscovery.io
[*] Enter PDCP API Key (exit to abort): *************
[INF] Successfully logged in as (@user)
```
Run a check on a CVE ID:
```
./cvemap -id CVE-2023-40547
```

## Sicat
https://github.com/justakazh/sicat

SiCat is an advanced exploit search tool designed to identify and gather information about exploits from both open sources and local repositories effectively. With a focus on cybersecurity, SiCat allows users to quickly search online, finding potential vulnerabilities and relevant exploits for ongoing projects or systems.

SiCat's main strength lies in its ability to traverse both online and local resources to collect information about relevant exploitations. This tool aids cybersecurity professionals and researchers in understanding potential security risks, providing valuable insights to enhance system security.

Sites it uses are:
1. Exploit-DB
2. Packetstorm Security
3. Exploit Alert
4. NVD Database
5. Metasploit Modules

Installation
```
git clone https://github.com/justakazh/sicat
```
```
cd sicat
```
```
pip3  install  -r  requirements.txt
```
Example Usage using exploitdb and msfmodule chekcing for Apache exploits:
```
python3 sicat.py -k apache --exploitdb --msfmodule
```
Run it based on Nmap output:
```
nmap -sV localhost -oX nmap_out | python sicat -nm --packetstorm
```






## General Security Blogs
**Bleeping Computer** https://www.bleepingcomputer.com/ \
**Security Affairs** https://securityaffairs.com/ \
**Naked Security** https://nakedsecurity.sophos.com/ \
**The Hacker News** https://thehackernews.com/ \
**Krebs on Security** https://krebsonsecurity.com/ \
**Dark Reading** https://www.darkreading.com/ \
**We Live Security** https://www.welivesecurity.com/ \
**Infosecurity Magazine** https://www.infosecurity-magazine.com/ \
**ATT Security Blog** https://cybersecurity.att.com/blogs \
**Checkpoint Research** https://research.checkpoint.com \
**CI Security** https://www.cisecurity.org/feed/advisories \
**CISA Alerts** https://us-cert.cisa.gov \
**Digital NHS** https://digital.nhs.uk \
**The Latest Hacking News** https://latesthackingnews.com/ \
**SEC-Consult** https://sec-consult.com/blog/ \
**SOC Radar** https://socradar.io/blog/ 

## Tooling
**Kitploit** https://www.kitploit.com/ 


## Forums
**Exposed.vc** https://exposed.vc/ \
**Ramp4u.io** https://ramp4u.io/

## POCs
[POC In Github](https://github.com/nomi-sec/PoC-in-GitHub) A list of POCs in a github repo
