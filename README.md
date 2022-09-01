## Video:
  - https://www.youtube.com/watch?v=ZBi8Qa9m5c0&t=5566s
  
## Bugbounty:
- 'https://bugcrowd.com/irobot'

# Enumerate 
## emails
- https://hunter.io/
## subdomains
- https://search.censys.io/
- https://sslmate.com/help/reference/ct_search_api_v1
 ```
 GET https://api.certspotter.com/v1/issuances?domain=DOMAIN
 ```
- crt.sh
```
crt.sh/?q=.%25<what are you looking for as subdomain>.%25.<domain>.<top level domain>
crt.sh/?q=.%25api.%25.yahoo.com
crt.sh/?q=.%25.%25.%25.%25.yahoo.com
```
```bash
curl -s https://crt.sh/?q=%.$1 | sed 's/<\/\?[^>]+>//g' | grep $1
```
- sublist3r
  ```bash
  sublist3r -d 'irobot.com'
  ```
- httprobe
  - https://github.com/tomnomnom/httprobe
```bash
cat recon/example/domains.txt | httprobe --prefer-https
certspotter $TARGET | httprobe --prefer-https
```

## technology etc. 
- https://builtwith.com/irobot.com
- securityheaders.com
- nikto (warning don't use it if you need to be stealth)
  ```bash
  nikto -h https://irobot.com
  ```


## Other
- https://vulners.com
