## Multiple Vulnerabilities in Bender/Bee  Charge Controller

| **Product**    | **Vulnerable Version** | Fixed Version                                        | **Found**            |
| -------------- | ---------------------- | ---------------------------------------------------- | -------------------- |
|  Charge Controller |                        |                                                      |                      |
| **CVE Number** | **Impact**             | **Homepage**                                         | **By**               |
|                |                        | [starvlab.qianxin.com](http://starvlab.qianxin.com/) | delikely \| StarVLab |

**Status**: RESERVED

### Vendor description


### Vulnerability overview

#### 1. Hardcoded Credentials in Charge Controller(CVE-2021-34601)

In Bender/ebee Charge Controllers in multiple versions are prone to Hardcoded Credentials. Bender charge controller CC612 in version 5.20.1 and below is prone to hardcoded ssh credentials. An attacker may use the password to gain administrative access to the web-UI.


#### 2. Command injection via Web interface(CVE-2021-34602)
In Bender/ebee Charge Controllers in multiple versions are prone to Command injection via Web interface. An authenticated attacker could enter shell commands into some input fields that are executed with root privileges.


### Proof of concept



### Solution




### Vendor contact timeline

- 2021-09-13	Contacting vendor through CERT@VDE

