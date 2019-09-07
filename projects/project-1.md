---
layout: project
type: project
image: images/openvas-logo.png
title: UH Manoa OpenVAS
permalink: projects/openvas
# All dates must be YYYY-MM-DD format!
date: 2019-07-18
labels:
  - PHP
  - Vulnerability Scanning
  - Website
summary: I maintain and update UHM's OpenVAS site at https://openvas.hawaii.edu. (Not accessible outside of ITC network).
---
## What is OpenVAS

OpenVAS is short for "Open Vulnerability Assessment Scanner". It is typically installed on a Linux machine and can then be used to scan other computers for any vulnerabilities such as commonly used passwords, open ports and the use of outdated/vulnerable versions of applications. Once the scan is finished, the users are able to retrieve a scan showing what was found to be vulnerable on the target machine and to what severity, allowing users to further harden their systems. 

Due to policy, some workers may be required to scan their machines to test their resilience against possible attacks. The scanner tool chosen by the university was OpenVAS.

The collective OpenVAS package includes its own user interface to start and manage scans, manage users, and view reports, but it can be hard to use. So, an interface written in PHP was created to allow ease of creating scans, viewing reports, and managing users. This interface is located at https://openvas.hawaii.edu. However, this website is only reachable from the Information Technology Center's network. 

## My Role

I was not involved with the creation of this interface. Instead, I have been tasked with maintaining its code the server it runs on whenever something may break or if a new feature must be added. For instance just recently I was tasked with getting the interface to communicate with two seperate scanners and have them balance the workload since many scans need to run during this time of year. 

I am also tasked to do a rewrite and improve this interface since the code was not very well put together by the original developer. Both the PHP code and the design were poor. Comments were scarce, the naming of variables was confusing and the database design could be better. 

## What I Learned

Throughout this experience of maintaining openvas.hawaii.edu website I've learned some PHP, how to troubleshoot and configure servers, and more Linux skills. Prior to taking up this project I had little experience working with servers, Linux, and PHP.  

Documentation and writing clean code is very important. Taking some time to take note of what is occurring in regards to code can be extremely helpful and decrease the time it takes to conduct a code review. 

## Source Code

I am unable to share the source code for the custom interface I'm in charge of maintaing as it is a private repository. 

## Screenshots of OpenVAS Site
IPs have been blurred for privacy purposes.

<img height="600" width="1000" src="https://gabrielundan.github.io/images/openvas-login.PNG">*Login page*
<img height="600" width="1000" src="https://gabrielundan.github.io/images/openvas-batchscan.PNG">*Example of batchscan page where a scan is created*
<img height="600" width="1000" src="https://gabrielundan.github.io/images/openvas-results.PNG">*Example of results page showing scan results*

