# Red Hat RHCSA-RHCE 7 Cert Guide (Lab Environment)

## About
This is a copy of [this repo](https://github.com/AnwarYagoub/RHCSA-RHCE-Lab-Environment) by @AnwarYagoub 

## What is included?
- server1: CentOS box (Server With GUI).
- server2: same as Server1
- cache-server: Debian box used for package caching.
- labipa: CentOS box with FreeIPA configured.

## Install dependencies:
- [Virtualbox](https://www.virtualbox.org): cross-platform virtualization application.
- [Vagrant](https://www.vagrantup.com): tool for building complete development environments. With an easy-to-use workflow and focus on automation

## How to start servers?
Navigate to project path where Vagranfile exists.

- start all servers
```shell
$ vagrant up
```
- start a specific server (server1, server2, cache-server, labipa)
```shell
$ vagrant up MACHINE_NAME
```

## How to access servers?
Navigate to project path where Vagranfile exists.

- to get shell access to any of environment servers
```shell
$ vagrant ssh MACHINE_NAME
```
- You can also access servers using ip addresses listed below.
```shell
ssh root@192.168.4.210
```
## How to stop servers?
Navigate to project path where Vagrantfile exists.

- stop all servers
```shell
$ vagrant halt
```
- stop a specific server
```shell
$ vagrant halt MACHINE_NAME
```
## IP addresses & credentials
| Server | IP address | username | password | username | password |
|---|---|:---:|:---:|:---:|:---:|
|cache-server|192.168.4.100 |vagrant|vagrant| | |
|server1|192.168.4.210|user|password|root|password|
|server2|192.168.4.220|user|password|root|password|
|labipa|192.168.4.200 |user|password|root|password|
