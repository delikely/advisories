## Multiple Vulnerabilities in GARO Wallbox

| Product                  | Vulnerable Version | Fixed Version                                        | Found                |
| :----------------------- | :----------------- | :--------------------------------------------------- | :------------------- |
| GARO Wallbox GLB/GTB/GTC | <=185              |                                                      | 2021.09.16           |
| **CVE Number**           | **Impact**         | **Homepage**                                         | **By**               |
|                          | critical           | [starvlab.qianxin.com](http://starvlab.qianxin.com/) | delikely \| StarVLab |

### Vendor description

[GARO AB](http://www.garo.se/) is responsible for the business areas of electrical installation and systems. Electrical installation comprises DIN rail components, meter cabinets with distribution panels and blocks, power outlets for car parks, switchgear, CEE sockets, etc. The Systems business area specialises in marine power outlets, camping and EV charging posts.

GARO AB is the parent company of the GARO Group.

### Vulnerability overview

#### 1. Without Authentication

Lack of access control on the web manger pages that allows any user  to view and modify information.

#### 2. Unauthenticated Command Injection 

The `url` parameter of the function module `downloadAndUpdate` is vulnerable to an command Injection. Unfiltered user input is used to generate code  which then gets executed when downloading  new firmware.

#### 3.Hard Coded Credentials for Tomcat Manager

A hardcoded credential  in  `/etc/tomcat8/tomcat-user.xml`, which allows attackers to gain authorized access and control the tomcat completely; Normal user can't be modified or deleted the account .

### Proof of concept

#### 1. Without Authentication



#### 2. Unauthenticated Command Injection 



#### 3. Hard Coded Credentials for Tomcat Manager



### Solution

**Advisory URL:** Contact GARO,didn't get reply.

### Vendor contact timeline

- 2021-09-13 Contacting vendor through Email 
- 2021-10-12  Contacting vendor through Email Again
- 2021-12-25 We have not got in touch with GARO,Disclosure the advisory.
