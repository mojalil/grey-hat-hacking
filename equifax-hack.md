# Overview


# Setup
* [Apache Struts with CVE-2017-5638 - set up a vulnerable server (Part-I)](https://www.youtube.com/watch?v=gidRh_4xugQ)

## Setup Docker For Apache Image
* [Docker image with apache structs vulnerability](https://hub.docker.com/r/piesecurity/apache-struts2-cve-2017-5638/)
* [Install Docker](https://docs.docker.com/install/linux/docker-ce/ubuntu/#set-up-the-repository)
* [Docker tutorial](https://stackify.com/docker-tutorial/)

Download docker image with vunerablility ```docker pull piesecurity/apache-struts2-cve-2017-5638```
View docker images ```docker images```
Run docker image with exposed port ```run piesecurity/apache-struts2-cve-2017-5638:latest -p 8080:8080 ```
Navigate to server via browser ```http:\\localhost:8080```

# Media
* [zdnet article](https://www.zdnet.com/article/equifax-confirms-apache-struts-flaw-it-failed-to-patch-was-to-blame-for-data-breach/)
* [Apache vulnerbility](https://securingtomorrow.mcafee.com/mcafee-labs/apache-struts-at-rest-analyzing-remote-code-execution-vulnerability-cve-2017-9805/)
* [Fortune 100 firms](https://www.zdnet.com/article/critical-security-bug-threatens-fortune-100-companies/)
* [Data & Stats about the attack](https://www.imperva.com/blog/2017/03/cve-2017-5638-new-remote-code-execution-rce-vulnerability-in-apache-struts-2/)