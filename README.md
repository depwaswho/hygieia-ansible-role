## Ansible Playbook to install Capital One's [Hygieia](https://github.com/capitalone/Hygieia "Hygieia Repository")

### Introduction

This playbook will install the Hygieia prerequisites, compile, build and run docker images for the API, UI, Collectors (Jenkins, Gitlab, Sonarqube). It is written for CentOS 7. The target machine can be changed in the included hosts file.

## Hygieia Pre-Requisites

* JDK
* Maven
* Bzip2
* Git
* Docker
* Node js
* Bower
* Gulp
* Mongodb database

## Hygieia Configuration

Before you run the playbook make sure you have changed the environment variables value in the `hosts` file

### Usage
You can run the playbook with
```ansible-playbook install.yml -i hosts -u <user> --private-key <path to pem file>```