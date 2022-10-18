# Domain Threat Intel

## Cloudflair

**Description:**
CloudFlair is a tool to find origin servers of websites protected by CloudFlare who are publicly exposed and don't restrict network access to the CloudFlare IP ranges as they should. 
```
python3 cloudflair.py leroy.com --censys-api-id <API key> --censys-api-secret <Secret Key> -o cloudflair-8-8-2022.txt
```

--censys-api-id <id>
--censys-api-secret <secret>
-o output file

## Cloudmare

**Description:**
Cloudmare is a simple tool to find the origin servers of websites protected by Cloudflare, Sucuri or Incapsula with a misconfiguration DNS.
```
python3 Cloudmare.py -u ljenkins.com
```


## CloudUnflare

**Description**
Reconnaissance Real IP address for Cloudflare Bypass.
```
bash cloudunflare.bash
```


## DnsRecon

**Description:** Basic DNS recon also using brute force
```
python3 dnsrecon.py -d wingnut.com
```


## Masscan

**Description:** This is an Internet-scale port scanner. It can scan the entire Internet in under 5 minutes, transmitting 10 million packets per second, from a single machine.
```
sudo masscan -p 80,8000-8100 10.2.2.2/22 --rate=10000
```


## Sublist3r

**Description:** Sudomain bruteforcer
```
python3 sublist3r.py -d wingnut.com -b
```

-b is for enabling bruteforcing

To list all the basic options and switches use -h switch:
``` 
python sublist3r.py -h
```

To enumerate subdomains of specific domain:
``` 
python sublist3r.py -d example.com
```

To enumerate subdomains of specific domain and show only subdomains which have open ports 80 and 443 :
``` 
python sublist3r.py -d example.com -p 80,443
```

To enumerate subdomains of specific domain and show the results in realtime:
``` 
python sublist3r.py -v -d example.com
```

To enumerate subdomains and enable the bruteforce module:
``` 
python sublist3r.py -b -d example.com
```

To enumerate subdomains and use specific engines such Google, Yahoo and Virustotal engines
``` 
python sublist3r.py -e google,yahoo,virustotal -d example.com
```


## Fierce: 

**Description:** DNS brute force
```
fierce --domain wingnut.com
```


## theHarvester
  **Description:** General OSINT tool on domains
  https://github.com/laramies/theHarvester \
  
  Recon scan for example.com. The -d is for the domain, the -l is to limit the results, the -b is for the source you want to use. You can also do -b all to use all of the sources, but you would need API keys for some of them. The -f is to write the reults to an XML file.
``` 
python3 theharvester.py -d example.com -l 500 -b google -f myresults.xml
```

