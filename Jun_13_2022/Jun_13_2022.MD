# Notes for Jun_13_2022

This is a note or a diary for the things I research in a day, this note intended for me not to forget the knowlegde I has gain (or things I has read).

## Notable techniques of EMOTET

- Using CVE-2017-11882
  
## Linux Malware name Symbiote

- <https://www.sandflysecurity.com/blog/bpfdoor-an-evasive-linux-backdoor-technical-analysis/>
- <https://thehackernews.com/2022/06/symbiote-stealthy-linux-malware.html>

The Symbiote malware is a **shared object library**, instead of an executable file.

Symbiote is targeting financial institutions in **Latin America**, with all file, processes, and network artifacts hidden by the malware, making it virtually invisible to detection by live forensics.

The malware also has Berkeley Packet Filter (BPF) hooking functionality. Packet capture tools intercept, or capture, network traffic typically for the purposes of an investigation.

Symbiote uses the **LD_PRELOAD** variable that allows it to be pre-loaded by applications before other shared object libraries.

## Registry Query for Native Messaging hosts

This appeared on the SIEM, which is querying for POSTMAN in nativemessaginghost
Host: mbanking01\
Source User: thanhtt\
Signature ID: 47-8000268
Description: -> reg query hkcu\software\google\chrome\nativemessaginghosts\com.postman.postmanapp

### What is Navive Messaging Hosts

- <https://developer.chrome.com/docs/apps/nativeMessaging/>
- <https://developer.mozilla.org/en-US/docs/Mozilla/Add-ons/WebExtensions/Native_messaging>
- <https://medium0.com/fme-developer-stories/native-messaging-as-bridge-between-web-and-desktop-d288ea28cfd7>

Native messaging enables **an extension to exchange messages with a native application**, installed on the user's computer. The native messaging serves the extensions without additional accesses over the web. -> Native Messaging as bridge between web and desktop

Chrome starts each native messaging host in a separate process and communicates with it using standard input (stdin) and standard output (stdout).

Because Native Messaging is only working in the bounds of the machine the security risk is minimal when the host was carefully implemented

## ELK Stack - Docker Compose on Cloud - AWS (ECS)

- <https://aws.amazon.com/blogs/containers/deploy-applications-on-amazon-ecs-using-docker-compose/>

I have a task to deploy our docker-compose elk stack on aws ecs so I have to research about ECS and how to deploy on it, which kinda fun to be honest

### Amazon Elastic Container Service (Amazon ECS)

#### What is ECS?

It is a highly scalable, high-performance container orchestration service that supports Docker containers and allows you to easily run and scale containerized applications on AWS.

#### What is Spot instance?

A Spot Instance is an instance that uses spare EC2 capacity that is available for less than the On-Demand price.

#### What is Task?

A **task definition is required** to run Docker containers in Amazon ECS, basically you can specify the config, the image, the size, the networking,... of the Docker Container just like a Dockerfile I would say but it is for the aws environment (Which will have IAM and some AWS specific config)

Each task that uses the **Fargate launch type has its own isolation boundary and does not share the underlying kernel, CPU resources, memory resources, or elastic network interface with another task.**

#### What is Fargate?
