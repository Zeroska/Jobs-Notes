# Notes for Jul_04_2022

This is a note or a diary for the things I research in a day, this note intended for me not to forget the knowlegde I has gain (or things I has read).

## AWS SecurityHub and GuardDuty

### Findings

It is AWS Security Finding Format - ASFF which is format that AWS use to exchange information between Security Hub and other service

---

## WebShell Incident Response - Tomcat 8

**Learn more about Tomcat 8**: <https://tomcat.apache.org/tomcat-8.0-doc/security-howto.html>

In Tomcat server you can upload a war file into it using **this path /manager/html** but luckly not everyone will have the permission to upload, you can obtain this credentials by bruteforce or phishing the account of the Admin but if your admin is "good" enough he will set it to admin/admin (or some default credentials)

Link <https://book.hacktricks.xyz/network-services-pentesting/pentesting-web/tomcat> you can find more specific guidance in here

### Does it has a huge impact?

If the credential that has the following permissions in order for this attack to works:

- admin, admin-gui
- manager, **manager-gui**, manager-script

### What is WAR File?

Short for Web Archive. Java web applications are usually packaged as WAR files for deployment. These files can be created on the command line or with an IDE, like Eclipse.

After deploying the WAR file, Tomcat unpacks it and stores all the project files from the webapps directory in a new directory named after the project

### Some real world implemtation

Link: <https://github.com/Rica123/spider>
