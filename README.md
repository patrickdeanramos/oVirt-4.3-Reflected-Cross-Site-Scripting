# oVirt-4.3-Reflected-Cross-Site-Scripting

Summary: oVirt-engine Open Virtualization Manager version 4.3 login page is vulnerable to reflected Cross-site scripting (XSS).  The parameter "scope" fails to sanitize the entry, allowing the malicious script to execute as part of the GET request.

Affected Parameter: scope 

Sample urls:
https://x.x.x.x/ovirt-engine/login?scope=ovirt-ext%3dauth%3aidentityxj2o4%3cscript%3ealert('XSS')%3c%2fscript%3eol2fb

Screenshot:
https://github.com/patrickdeanramos/oVirt-4.3-Reflected-Cross-Site-Scripting/blob/master/oVirt%20XSS.png?raw=True

Response from RedHat:<
oVirt 4.3 is an obsolete version 

Authors: 
Patrick Dean Ramos
Nathu Nandwani
Junnair Manla 