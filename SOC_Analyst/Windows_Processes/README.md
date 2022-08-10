# Windows Processes

- Link: <http://undocumented.ntinternals.net/index.html?page=UserMode%2FUndocumented%20Functions%2FNT%20Objects%2FProcess%2FPEB.html> | undocumented Windows 
- Link: <https://github.com/alphaSeclab/injection-stuff>
- Link: <https://redcanary.com/blog/process-integrity-levels/> | Process integrity level
Research Topic:

- [x] PEB 
- [ ] _EPROCESS
- [ ] Process Injection
- [ ] Process integrity level


---
## Let's talk about PEB

Structure PEB (Process Enviroment Block) contains all User-Mode parameters associated by system with current process. you can find a process image by search for ```ImageBaseAddress``` using ```ReadRemotePEB()``` or ```NtQueryProcessInformation()```  


---

## Windows integrity level

Integrity levels define the trust between process/thread and another object (files, processes, threads) and help control what that object can or can’t do on a system. **A sudden change in a process’s integrity level might be a sign that an adversary has obtained system privileges**. 


