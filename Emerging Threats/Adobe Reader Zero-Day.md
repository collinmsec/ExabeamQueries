_NOTE: Some of the fields that are being used may be different in your environment depending on parsing._ 
_NOTE: Some of the IOCs in the queries will be dafanged just for safety so please take this into account when using in your environment._ 

### Network IOCs :

_NOTE: This is more of query to look for synchronizer initiated traffic, would be good to look at vendors logging http & https ._ 
`vendor:"zscaler" AND user_agent:"Mozilla/3.0 (compatible; Adobe Synchronizer 23.8.20533)"`

_NOTE: I did not specify a vendor for these, but would be good to look at vendors logging http & https ._ 
`src_ip:(169[.]40[.]2[.]68, 188[.]214[.]34[.]20) AND (src_port:(34123,45191) OR dest_port:(34123,45191))`

_NOTE: I did not specify a vendor for these, but would be good to look at vendors logging http & https ._ 
`dest_ip:(169[.]40[.]2[.]68, 188[.]214[.]34[.]20) AND (src_port:(34123,45191) OR dest_port:(34123,45191))`

_NOTE: Looking for malicious domain._ 
`vendor:"zscaler" AND web_domain:"ado-read-parser[.]com"`
`vendor:"zscaler" AND web_domain:"zx.ado-read-parser[.]com"`

_NOTE: Looking for malicious URLs._ 

`vendor:"zscaler" AND url:"hxxp[://]188[.]214[.]34[.]20:34123/rs1?rnd=<float>&od=422974"`

`vendor:"zscaler" AND url:"hxxp[://]188[.]214[.]34[.]20:34123/s11?language=ENU&viewerType=Reader&viewerVersion=[.][.][.]&platform=WIN&activeDocs=[.][.][.]&errs=[.][.][.]&av=[.][.][.]&osVersion=[.][.][.]&pdfFile=[.][.][.]&rnd=[.][.][.]&od=422974"`

`vendor:"zscaler" AND url:"hxxp[://]188[.]214[.]34[.]20:34123/s12?language=ENU&viewerType=Reader&viewerVersion=25[.]00120435&platform=WIN"`

`vendor:"zscaler" AND url:"hxxp[://]188[.]214[.]34[.]20:34123/rs2"`

`vendor:"zscaler" AND url:"hxxp[://]zx[.]ado-read-parser[.]com/"`

`vendor:"zscaler" AND url:"hxxp[://]169[.]40[.]2[.]68:45191/rs1?rnd=<float>&od=319988"`

`vendor:"zscaler" AND url:"hxxp[://]169[.]40[.]2[.]68:45191/s11?language=ENU&[.][.][.]&od=319988"`


Inspiration/Reference: https://gist.github.com/N3mes1s/9e55e8d781235ee256d5b3f6720222dd
