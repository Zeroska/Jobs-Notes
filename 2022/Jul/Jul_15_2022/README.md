# Notes for Jul_15_2022

This is a note or a diary for the things I research in a day, this note intended for me not to forget the knowlegde I has gain (or things I has read).

## CVE-2022-32223 Discovery: DLL Hijacking via npm CLI

Link: <https://blog.aquasec.com/cve-2022-32223-dll-hijacking>

## Windows Security Feature 

### Control Flow Guard or CIG

*Notes: the Edge broker processes are protected almost to the maximum possible level with the above techniques.*

Well it is suppose to protect your processes from being inject, DLL injection will have to has Microsoft Signed

---
## SSL and self-certs

- Link: <https://devopscube.com/create-self-signed-certificates-openssl/>
- Link: <https://blogs.oracle.com/blogbypuneeth/post/create-an-internal-certification-authority-ca-using-keytool-and-sign-your-server-certificate>
- Link: <https://dzone.com/articles/ssl-in-java>

I don't know about you guys but when I started to learn about SSL and Certificate, I don't pay much attention so now I have to revise it and dig a little deeper on this subject -> Don't be like me guys, stay focus and pay attention to everything.

### Java specific SSL

**Key Store**: keystores hold keys that our application owns, which we can use to prove the integrity of a message and the authenticity of the sender, say by signing payloads. 

**Trust Store**: A truststore is the opposite. While a keystore typically holds onto certificates that identify us, a truststore holds onto certificates that identify others. | In Java in has default Trust Store call cacerts which located at **JAVA_HOME/jre/lib/security/cacerts** 

Since Java 9, the default keystore format is PKCS12. The biggest difference between JKS and PKCS12 is that JKS is a format specific to Java, while PKCS12 is a standardized and language-neutral way of storing encrypted private keys and certificates.

