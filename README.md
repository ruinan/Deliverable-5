# Deliverable-5
##Vulnerability 1: Cross Site Scripting
###1.	What part of the InfoSec Triad does this vulnerability attack (confidentiality, integrity, or availability)
Availability, Confidentiality, Integrity.
###2.	What kind of security attack can exploit this vulnerability (interruption, interception, modification, or fabrication)?
Interception, Modification, Fabrication.
###3.	Are attacks that exploit this vulnerability active or passive?
Active 
###4.	What business value would be lost due to exploiting this vulnerability (data loss, unauthorized access, denial of service, etc)?
It can access any cookies, session tokens, or other sensitive information retained by the browser. Because user will bypass the access control. Depend on these, attacker will take control of data, devices, and steal account information, etc.
###5.	What steps should the development team take to fix this vulnerability?
The simple way to fix that is to add XSS protect function. Developer may conduct a checking inspection that does not allow any JavaScript statements, symbols or HTML tags in the input box.
###A.	The URL of the website with the described vulnerability.
TestURL:http://testaspnet.vulnweb.com/ReadNews.aspx?NewsAd=javascript%3Aalert%28%22This%20is%20attact%22%29%3B&id=0
###B.	Steps taken to exploit the vulnerability.
First, change the original URL: http://testaspnet.vulnweb.com/ReadNews.aspx?NewsAd=ads%2fdef.html&id=0<br /> 
   &nbsp;&nbsp; &nbsp;&nbsp;To: http://testaspnet.vulnweb.com/ReadNews.aspx?NewsAd=javascript%3Aalert%28%22This%20is%20attact%22%29%3B&id=0<br /> 
Second, press Enter;
###C.	A screenshot (if applicable) of the vulnerability.
![Alt text](https://github.com/ruinan/Deliverable-5/blob/master/screenshots/v-1.png)

##Vulnerability 2: SQL Injection
###1.	What part of the InfoSec Triad does this vulnerability attack (confidentiality, integrity, or availability)?
  Because the value got from input box will be insert into a Select SQL statement.
Availability, Integrity
###2.	What kind of security attack can exploit this vulnerability (interruption, interception, modification, or fabrication)?
  Fabrication
###3.	Are attacks that exploit this vulnerability active or passive?
  Active
###4.	What business value would be lost due to exploiting this vulnerability (data loss, unauthorized access, denial of service, etc)?
  The unauthorized user will access administrator account. It means user will obtain some authorities that would control whole site.
###5.	What steps should the development team take to fix this vulnerability?
  I think the way to fix the vulnerability is like the method for fixing the previous vulnerability. First, developer needs to install some checking mechanism to make sure what input is in accordance with the rules. Second, the database should set a firewall.
###A. The URL of the website with the described vulnerability.
Test URL: http://demo.testfire.net/bank/login.aspx.
###B. Steps taken to exploit the vulnerability.
First, click the ONLINE BANKING LOGIN link;
Second, input “ZAP' OR '1'='1' –“ to the password box, then type any username you want.
Third, click LOGIN button.
###C. A screenshot (if applicable) of the vulnerability.
I will got the admin access.
![Alt text](https://github.com/ruinan/Deliverable-5/blob/master/screenshots/vulnerability2-2.png)
![Alt text](https://github.com/ruinan/Deliverable-5/blob/master/screenshots/vulnerability2-1.png)

##Vulnerability 3: Directory Browsing
###1.	What part of the InfoSec Triad does this vulnerability attack (confidentiality, integrity, or availability)?
Confidentiality, Integrity
###2.	What kind of security attack can exploit this vulnerability (interruption, interception, modification, or fabrication)?
Modification, Fabrication
###3.	Are attacks that exploit this vulnerability active or passive?
Passive
###4.	What business value would be lost due to exploiting this vulnerability (data loss, unauthorized access, denial of service, etc)?
The whole directory exposed. So the visitor could read the source code for your website. And maybe they can upload or download files through the server. Because they already know where are the files and what are their function. So it is much easier to modify the files or insert some malicious codes in order to manipulate the website.
###5.	What steps should the development team take to fix this vulnerability?
The directory should be invisible for the visitor. Development team could add some statements into configure file to prevent this happen.
###A.	The URL of the website with the described vulnerability.
Test URL: http://scanme.nmap.org/shared/
###B.	Steps taken to exploit the vulnerability.
First, add /shared/ behind http://scanme.nmap.org
Second, click Enter, or let browser visit this site.
Third, you can visit the directory.
###C.	A screenshot (if applicable) of the vulnerability.
![Alt text](https://github.com/ruinan/Deliverable-5/blob/master/screenshots/vulnerability3.png)




