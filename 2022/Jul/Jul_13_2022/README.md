# Notes for Jul_13_2022

This is a note or a diary for the things I research in a day, this note intended for me not to forget the knowlegde I has gain (or things I has read).

## Processs Injection | How to create detection rule.

Links: <https://redcanary.com/blog/process-injection-primer/>

This is a Windows feature but was use by bad guys to create a way to **inject their malicous code to a legit process**, the first step to learn how to detect it to know how it works and what are the log and the resource it will create when using this technique and how hard can we detect it using SIEM and EDR

### DLL Injection | [T1055.001](https://attack.mitre.org/techniques/T1055/001)

Link: <https://sec.vnpt.vn/2019/01/dll-injection/> explain very well about DLL Injection but use Vietnamese 

This picture can explain it very well, this picture I copy from the link above:

![dll injection](./assets/2022-07-13_08-33.png)

There are few key point you need to remmeber about this technique:

- It is noisy as hell 
- 

### PE Injection | [T1055.002](https://attack.mitre.org/techniques/T1055/002)



### Process Hollowing

---
## Sysmon Logging

Really Powerful Logging Drive from sysinternal. It provides detailed information about process creations, network connections, and changes to file creation time

Some example configuration link: <https://github.com/SwiftOnSecurity/sysmon-config/blob/master/sysmonconfig-export.xml>. at the momment I haven't read or understand all the configuration in here. But in the near future I will be able to understand all of this




