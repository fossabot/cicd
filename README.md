#CICD Demo

## Purpose
This repo serves for preparing CI/CD pipeline for testing

## Install

type `bin\0_install.sh`

This script will install docker, docker-compose & ansible on the host VM.
Then create GitLab, GitLab runner, WeaveScope, Jenkins BlueOcean, Ansible, SonarQube, Artifactory & Conjur as containers

## Host names
xip.io will be used for DNS names for containers.


## Login Details
By default, a text file will be generated, containing all the login url, username & passwords.



## Individual Componments

### Gitlab

Two containers are used, one for SCM & one for CI runner
A ruby script is used to get the registration token as there is no offical way to fetch it using CLI or API (as of 2018.03)


## Useful Scripts

###bin/cleanup.sh
This script kills & removes all related containers

