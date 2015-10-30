---
name: Docker Tasks
author: Bruce Becker
modified: 26-10-2015
---


# Preludes


  1. Install docker
    * Debian : `apt-get install docker.io`
    * CentOS : `yum install docker`
  1. Start Docker
    * Debian : `service docker.io start`
    * CentOS : `service docker start`

# Getting the Containers

A few containers have been prepared. Get them from Docker Hub:

```
docker pull aaroc/code-rade-sl6-ansible
docker pull aaroc/code-rade-u1404-ansible
```
