# Overview
Setup and demo of equifax hack

# Setup
* [Apache Struts with CVE-2017-5638 - set up a vulnerable server (Part-I)](https://www.youtube.com/watch?v=gidRh_4xugQ)

## Setup Docker For Apache Image
* [Docker image with apache structs vulnerability](https://hub.docker.com/r/piesecurity/apache-struts2-cve-2017-5638/)
* [Install Docker](https://docs.docker.com/install/linux/docker-ce/ubuntu/#set-up-the-repository)
* [Docker tutorial](https://stackify.com/docker-tutorial/)


### Instructions
* Download docker image with vunerablility ```docker pull piesecurity/apache-struts2-cve-2017-5638```
* View docker images ```docker images```
* Run docker image with exposed port ```run piesecurity/apache-struts2-cve-2017-5638:latest -p 8080:8080 ```
* Navigate to server via browser ```http:\\localhost:8080```
* EC@ Example: 
```python exploit.py "http://ec2-13-127-53-72.ap-south-1.compute.amazonaws.com:8080/showcase.action" "ls -l"```
```python exploit.py "http://ec2-13-127-53-72.ap-south-1.compute.amazonaws.com:8080" "cat /etc/passwd"``` 

* Reading /etc/passwd : https://www.youtube.com/watch?v=UxQ9m3L33a0

* Adding user : https://www.digitalocean.com/community/tutorials/how-to-use-passwd-and-adduser-to-manage-passwords-on-a-linux-vps

* Decrypt passwords online via : http://md5decrypt.net
* Example hashed password (MD5): 

# Media & Link
* [zdnet article](https://www.zdnet.com/article/equifax-confirms-apache-struts-flaw-it-failed-to-patch-was-to-blame-for-data-breach/)
* [Apache vulnerbility](https://securingtomorrow.mcafee.com/mcafee-labs/apache-struts-at-rest-analyzing-remote-code-execution-vulnerability-cve-2017-9805/)
* [Fortune 100 firms](https://www.zdnet.com/article/critical-security-bug-threatens-fortune-100-companies/)
* [Data & Stats about the attack](https://www.imperva.com/blog/2017/03/cve-2017-5638-new-remote-code-execution-rce-vulnerability-in-apache-struts-2/)
* [Demo, Breakdown and Code](https://dzone.com/articles/will-it-pwn-cve-2017-5638-remote-code-execution-in)
* [Demo 2](https://dzone.com/articles/live-demo-exploiting-apache-struts-vulnerabilities)