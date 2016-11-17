# Deliverable-5
##Vulnerability 1: Cross Site Scripting
1.	What part of the InfoSec Triad does this vulnerability attack (confidentiality, integrity, or availability)?
Availability, Confidentiality, Integrity.
2.	What kind of security attack can exploit this vulnerability (interruption, interception, modification, or fabrication)?
Interception, Modification, Fabrication.
3.	Are attacks that exploit this vulnerability active or passive?
Active 
4.	What business value would be lost due to exploiting this vulnerability (data loss, unauthorized access, denial of service, etc)?
It can access any cookies, session tokens, or other sensitive information retained by the browser. Because user will bypass the access control. Depend on these, attacker will take control of data, devices, and steal account information, etc.
5.	What steps should the development team take to fix this vulnerability?
The simple way to fix that is to add XSS protect function. Developer may conduct a checking inspection that does not allow any JavaScript statements, symbols or HTML tags in the input box.



