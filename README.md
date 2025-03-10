link: https://kcoof.github.io/Dorks-for-all-/

# Dorks for Bug Bounty

A list of  Dorks for Bug Bounty

---
### Broad domain search w/ negative search

> site:example.com -www

### Server Errors

> site:example.com intext:"error" | intext:"exception" | intext:"failure" | intext:"server at" | intext:exception | intext:"database error" | intext:"SQL syntax" | intext:"undefined index" | intext:"unhandled exception" | intext:"stack trace"

### Login Page (User)

> site:example.com inurl:login | inurl:logon | inurl:sign-in | inurl:signin | inurl:wp-login | inurl: weblogin | inurl:loginpanel | inurl:quicklogin | inurl:memberlogin | inurl:forgotpassword | inurl:forgot-password | intitle:login | intitle:signin | intitle:sign-in | inurl:panel

> site:example.com inurl:login | inurl:signin Google

### Login Page (Admin)

> site:example.com inurl:admin | inurl:administrator | inurl:adm | inurl:wp-admin | inurl:adminlogin | inurl:admin-login

### Backup Files

> site:example.com ext:bkf | ext:bkp | ext:bak | ext:old | ext:backup | ext:log | ext:sql

> site:example.com intitle:"Index of" ext:sql | ext:sql.gz | ext:sql.rar | ext:sql.zip | ext:bkp | ext:bkp.gz | ext:bkp.rar | ext:bkp.zip | ext:zip | ext:7z | ext:rar | ext:gz

### API DOCS

> site:example.com inurl:api | inurl:*/rest | inurl:*/v1 | inurl:*/v2 | inurl:*/v3 | inurl:swagger | inurl:graphql | inurl:graphiql

### Juicy Info

> site:example.com ext:txt | ext:conf | ext:cnf | ext:ini | ext:env | ext:sh | ext:swp | ext:old | ext:~ | ext:htpasswd | ext:htaccess | ext:csv | ext:.git-credentials | ext:yaml | ext:yml | ext:ppk | ext:pem | ext:json | ext:cfg | ext:xml | ext:ps1 | ext:reg | ext:inf | ext:rdp | ext:ora | ext:dbf | ext:mdb

> site:example.com inurl:conf | inurl:env | inurl:cgi | inurl:bin | inurl:etc | inurl:root | inurl:sql | inurl:backup | inurl:admin | inurl:php

> site:example.com ext:doc | ext:xlsx | ext:docx | ext:dotx | ext:xls | ext:xlsm | ext:odt | ext:pdf | ext:rtf | ext:sxw | ext:psw | ext:ppt | ext:pptx | ext:pps | ext:csv | ext:swf intext:password|pass|email|admin|user|offer|data|employee|order|internal|sensitive

> site:example.com intext:confidential|"Not for Public Release"|"internal use only"|"do not distribute"

> site:example.com intext:username|password|pass|email|confidential filetype:log

> site:example.com intitle:"index of /"

> site:example.com intitle:"index of /" admin|user|portal|data|config|backup|password|email|employee|upload|uploads|download

> site:example.com intitle:"Index of" .env | .git | wc.db | .svn | .hg | .ovpn | config.php | database.sql

> site:example.com jdbc

> site:example.com inurl:admin/default.aspx | inurl:/wp-includes/uploads

> site:example.com inurl:/admin ext:config

> site:example.com inurl:wp- | inurl:wp-content | inurl:plugins | inurl:uploads | inurl:themes | inurl:download

> site:example.com inurl:readme | inurl:license | inurl:install | inurl:setup | inurl:config

> site:example.com inurl:shell | inurl:backdoor | inurl:wso | inurl:cmd | shadow | passwd | boot.ini | inurl:backdoor

### Blind XSS (Forms)

> site:example.com intitle:"support" | inurl:support | inurl:"contact" | intitle:"survey" | inurl:"survey" -pdf -doc -docx -xls

> site:example.com inurl:"feedback" | intitle:"feedback" | inurl:"submit" | intitle:"submit" -pdf -doc -docx -xls

### PHP extension w/ parameters

> site:example.com ext:php | ext:phtm | ext:phtml

### Java extension w/ parameters

> site:example.com ext:jsp | ext:do | ext:action | ext:struts | ext:java | ext:class | ext:jar | ext:war | ext:ear

### NET extension w/ parameters

> site:example.com ext:aspx | ext:asa | ext:asp | ext:asax

### Perl extension

> site:"example.com" ext:pl

### Other extensions

> site:example.com ext:cfm | ext:py | ext:rb | ext:js

### App frameworks and their exposures

> site:example.com inurl:/content/usergenerated | inurl:/content/dam | inurl:/jcr:content | inurl:/libs/granite | inurl:/etc/clientlibs | inurl:/content/geometrixx | inurl:/bin/wcm | inurl:/crx/de

> site:example.com "Whoops! There was an error."

> site:example.com inurl:/frontend_dev.php/$

> site:example.com inurl:/app/config/ | inurl:/settings.py intitle:"Index of"

> site:example.com "SF_ROOT_DIR"

> site:example.com Application Trace + nil:NilClass (10%) TBD

> site:example.com "unexpected error" | "Uncaught Exception" | "fatal error" | "Unknown column" | "exception occurred"

### XSS prone parameters

> inurl:lang= | inurl:name= | inurl:view= | inurl:name= | inurl:callback= | inurl:id= | inurl:q= | inurl:s= | inurl:keyword= | inurl:search= | inurl:page= | inurl:query= inurl:& site:example.com

### Open Redirect prone parameters

> inurl:page= | inurl:next= | inurl:host= | inurl:go= | inurl:goto= | inurl:file= | inurl:host= | inurl:redirect_to= | inurl:url= | inurl:redirect | inurl:src=http | inurl:r=http | inurl:return= | inurl:next= | inurl:redir= | inurl:http inurl:& site:example.com

### SQLi Prone Parameters

> inurl:id= | inurl:query= | inurl:q= | inurl:name= | inurl:from= | inurl:s= | inurl:search= | inurl:page= | inurl:filter= | inurl:action= | inurl:sort= | inurl:dir= | inurl:reg= | inurl:order= | inurl:update= | inurl:delete= | inurl:create= inurl:& site:example.com

### SSRF Prone Parameters

> inurl:http= | inurl:load= | inurl:exec= | inurl:resource= | inurl:resources= | inurl:url= | inurl:path= | inurl:host= | inurl:proxy= | inurl:html= | inurl:data= | inurl:domain=  | inurl:uri= inurl:& site:example.com

### LFI Prone Parameters

> inurl:include= | inurl:page= | inurl:http= | inurl:path= | inurl:template= | inurl:show= | inurl:locate= | inurl:site= | inurl:dir= | inurl:detail= | inurl:file= | inurl:folder= | inurl:locate= | inurl:doc= | inurl:filename= inurl:& site:example.com

### SSTI Prone Parameters

> inurl:module= | inurl:template= | inurl:load= | inurl:run= | inurl:preview= | inurl:view= | inurl:content= | inurl:activity= | inurl:name= inurl:& site:example.com

### RCE Prone Parameters

> inurl:cmd= | inurl:ip= | inurl:cli= | inurl:load= | inurl:module= | inurl:run= | inurl:print= | inurl:exec= | inurl:query= | inurl:code= | inurl:do= | inurl:run= | inurl:read= | inurl:ping= inurl:& site:example.com

### Sensitive Parameters

> inurl:email= | inurl:phone= | inurl:password= | inurl:secret= | inurl:token= inurl:& site:example.com

### File Upload

> site:example.com & intext:"choose file"
> site:example.com intext:"file upload"
> site:example.com (inurl:upload.php | inurl:upload.asp  | inurl:upload.aspx | inurl:upload.jsp | inurl:upload.do | inurl:upload.action)
> site:example.com intitle:"index of" "upload"

### Code Leaks

> site:gitlab.com "example.com"

> site:trello.com "example.com"

> site:atlassian.net "example.com"

> site:atlassian.net inurl:/servicedesk/customer/user/login "example.com"

> site:bitbucket.org "example.com"

> site:bitbucket.org inurl:example.com

> site:codebeautify.org "example.com"

> site:codepad.co "example.com"

> site:codepen.io "example.com"

> site:codeshare.io "example.com"

> site:coggle.it "example.com"

> site:firebaseio.com "example.com"

> site:gitter.im "example.com"

> site:google.com "example.com"

> site:box.com "example.com"

> site:jfrog.io "example.com"

> site:jsdelivr.net "example.com"

> site:jsfiddle.net "example.com"

> site:libraries.io "example.com"

> site:npm.runkit.com "example.com"

> site:npmjs.com "example.com"

> site:papaly.com "example.com"

> site:pastebin.com "example.com"

> site:prezi.com "example.com"

> site:productforums.google.com "example.com"

> site:repl.it "example.com"

> site:scribd.com "example.com"

> site:sharecode.io "example.com"

> site:trello.com "example.com"

> site:ycombinator.com "example.com"

> site:zoom.us inurl:"example.com"

### Cloud Storage

> site:s3.amazonaws.com "example.com"

> site:blob.core.windows.net "example.com"

> site:googleapis.com "example.com"

> site:drive.google.com "example.com"

> site:dev.azure.com "example.com"

> site:onedrive.live.com "example.com"

> site:digitaloceanspaces.com "example.com"

> site:sharepoint.com "example.com"

> site:amazonaws.com "example.com"

> inurl:www.dropbox.com/s/ "example.com"

> site:box.com/s "example.com"

> site:docs.google.com inurl:"/d/" "example.com"

---
