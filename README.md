## Video:
  - https://www.youtube.com/watch?v=ZBi8Qa9m5c0&t=5566s
  
## Bugbounty:
- 'https://bugcrowd.com/irobot'

# Enumerate 
## emails
- https://hunter.io/
## subdomains
- crt.sh
```
crt.sh/?q=.%25<what are you looking for as subdomain>.%25.<domain>.<top level domain>
crt.sh/?q=.%25api.%25.yahoo.com

```
- sublist3r
  ```bash
  sublist3r -d 'irobot.com'
  ```

## technology etc. 
- https://builtwith.com/irobot.com
- securityheaders.com
- nikto
  ```bash
  nikto -h https://irobot.com
  ```
- httprobe
  - https://github.com/tomnomnom/httprobe
```bash
cat recon/example/domains.txt | httprobe --prefer-https
certspotter $TARGET | httprobe --prefer-https
```

## Other
- https://vulners.com
