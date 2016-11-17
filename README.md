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

##Vulnerability 2: SQL Injection
1.	What part of the InfoSec Triad does this vulnerability attack (confidentiality, integrity, or availability)?
Because the value got from input box will be insert into a Select SQL statement.
Availability, Integrity
2.	What kind of security attack can exploit this vulnerability (interruption, interception, modification, or fabrication)?
Fabrication
3.	What business value would be lost due to exploiting this vulnerability (data loss, unauthorized access, denial of service, etc)?
The unauthorized user will access administrator account. It means user will obtain some authorities that would control whole site.
4.	What steps should the development team take to fix this vulnerability?
I think the way to fix the vulnerability is like the method for fixing the previous vulnerability. First, developer needs to install some checking mechanism to make sure what input is in accordance with the rules. Second, the database should set a firewall.

A.  The URL of the website with the described vulnerability.
Test URL: http://demo.testfire.net/bank/login.aspx.
B.  Steps taken to exploit the vulnerability.
First, click the ONLINE BANKING LOGIN link;
Second, input “ZAP' OR '1'='1' –“ to the password box, then type any username you want.
Third, click LOGIN button.
C.	A screenshot (if applicable) of the vulnerability.
I will got the admin access.





