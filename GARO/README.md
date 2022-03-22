## Multiple Vulnerabilities in GARO Wallbox

| Product                    | Vulnerable Version | Fixed Version                                        | Found                                                |
| :------------------------- | :----------------- | :--------------------------------------------------- | :--------------------------------------------------- |
| GARO Wallbox GLB/GTB/GTC   | <=185              |                                                      | 2021.09.16                                           |
| **CVE Number**             | **Impact**         | **Homepage**                                         | **By**                                               |
| CVE-2021-45876/45877/45878 | critical           | [www.garo.se](https://www.garo.se)                   | delikely@[StarVLab](http://starvlab.qianxin.com/) |

### Vendor description

[GARO AB](http://www.garo.se/) is responsible for the business areas of electrical installation and systems. Electrical installation comprises DIN rail components, meter cabinets with distribution panels and blocks, power outlets for car parks, switchgear, CEE sockets, etc. The Systems business area specialises in marine power outlets, camping and EV charging posts.

GARO AB is the parent company of the GARO Group.

### Vulnerability overview
#### 1. Without Authentication(CVE-2021-45878)

Lack of access control on the web manger pages that allows any user  to view and modify information.

#### 2. Hard Coded Credentials for Tomcat Manager(CVE-2021-45877)

A hardcoded credential  in  `/etc/tomcat8/tomcat-user.xml`, which allows attackers to gain authorized access and control the tomcat completely; Normal user can't be modified or deleted the account .

#### 3. Unauthenticated Command Injection(CVE-2021-45876)

The `url` parameter of the function module `downloadAndUpdate` is vulnerable to an command Injection. Unfiltered user input is used to generate code  which then gets executed when downloading  new firmware.


### Proof of concept

#### 1. Without Authentication

#### 2. Hard Coded Credentials for Tomcat Manager

#### 3. Unauthenticated Command Injection 


### Solution

**Advisory URL:** Contact GARO,didn't get reply.

### Vendor contact timeline

- 2021-09-13 Contacting vendor through Email.
- 2021-10-12 Contacting vendor through Email Again.
- 2021-12-25 We have not got in touch with GARO,Disclosure the advisory.
- 2021-12-26 Reporting to CVE.
- 2022-03-21 CVE Team assigned CVE number.
