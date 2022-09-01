## Video:
  - https://www.youtube.com/watch?v=ZBi8Qa9m5c0&t=5566s
  
## Bugbounty:
- 'https://bugcrowd.com/irobot'

# Enumeration 
## emails
- https://hunter.io/
## Subdomains enumeration
![](/media/subdomain_enum.png)
#### main links
- https://search.censys.io/
- certspotter
- whoxy.com
- subdomainizer(find keys)
- subscraper
- shodan.io
- https://sslmate.com/help/reference/ct_search_api_v1
- crt.sh

#### asn enumeration
- hurricane electronic internet service bgp.he.net
- metabigor
```bash
echo 'name' | metabigor net --org -v
```
```bash
amas intel -asn <ASN number>
```
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
#### Spiders
- hackrawler
- gospider
- 
#### subdomain brutforcing
- https://portswigger.net/burp/documentation/desktop/tutorials/enumerating-subdomains
------------


## Investigate the technology etc. 
- https://builtwith.com/irobot.com
- securityheaders.com
- nikto (warning don't use it if you need to be stealth)
  ```bash
  nikto -h https://irobot.com
  ```


## Other
- https://vulners.com
