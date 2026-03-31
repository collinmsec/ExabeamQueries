_NOTE: Some of the fields that are being used may be different in your environment depending on parsing._ 
_NOTE: Some of the IOCs in the queries will be dafanged just for safety so please take this into account when using in your environment._ 

### Network IOCs :
`url:RGXi("^packages\.npm\.org\/product[0-2]$")`

`web_domain:"sfrclak[.]com"`

`dest_ip:142[.]11[.]206[.]73`

Inspiration/Reference: https://www.stepsecurity.io/blog/axios-compromised-on-npm-malicious-versions-drop-remote-access-trojan, https://www.aikido.dev/blog/axios-npm-compromised-maintainer-hijacked-rat
