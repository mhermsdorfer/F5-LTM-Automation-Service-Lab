# F5 LTM Automation Service Lab 

The officially supported App Services Integration iApp is unlike other iApps in that it offers configuration of all common L4-L7 services.  Because of this it proves to be a useful tool for automation integration, as a single declarative REST call can configure: nodes, monitors, pools, profiles, virtual servers, etc.

This Lab is intended to give an introduction into the App Services iApp.  Specifically, it's designed as a ready to use environment to follow the lab guide that is contained in the App Services iApp documentation.

Additionally, on the windows desktop there is a postman collection that contains the REST/JSON payloads to perform each step in the lab.  I strongly encourage you to explore the postman collection as opposed to running though the labs via the WebUI.  The iApp is intended as an integration tool with existing automation suites, it was not really designed to be used in the WebUI.

There are some IP differences between this LAB and the current published lab guide.  Notably, this lab does not have an HA BIG-IP Pair, and the BIG-IP uses .8 as the last octet for both management and self-ip addresses.



## Lab Environment

UDF pre-build environment

### Networks
VLAN | Subnet
---- | ------
Management | 10.1.1.0/24
Internal   | 10.1.10.0/24
External   | 10.1.20.0/24


### BIG-IP
```
Management IP: 10.1.1.8
Internal IP: 10.1.10.8/24
External IP: 10.1.20.8/24
Username: admin
Password: admin
```

### Windows Jump Host
```
Management IP: 10.1.1.4
External IP: 10.1.20.250/24
Username: Administrator
Password: bdfbEWaE1
```

### Linux Webserver	
```
Management: 10.1.1.5
Internal: 10.1.10.100-103/24
Services: HTTP/HTTPS/SSH
Auth: SSH Key Auth Only
```

