# MasterOfSudo  

## Introduction  
MasterOfSudo is a Linux system administration project designed to enhance your understanding of virtualization, partitioning, security policies, user management, and essential Linux commands. This project aims to strengthen your ability to manage a Linux-based server effectively.  

## Table of Contents  
- [What is Virtualization?](#what-is-virtualization)  
- [What is a Virtual Machine (VM)?](#what-is-a-virtual-machine-vm)  
- [Differences Between Rocky Linux and Debian](#differences-between-rocky-linux-and-debian)  
- [AppArmor and apt vs. aptitude](#apparmor-and-apt-vs-aptitude)  
- [Partitions and Configuration](#partitions-and-configuration)  
- [Logical Volume Manager (LVM)](#logical-volume-manager-lvm)  
- [Sudo: Privilege Management](#sudo-privilege-management)  
- [User and Group Management](#user-and-group-management)  
- [Basic Linux Commands](#basic-linux-commands)  
- [SSH and Secure Access](#ssh-and-secure-access)  
- [Firewall (UFW) Configuration](#firewall-ufw-configuration)  
- [Additional Security Tips](#additional-security-tips)  

---

## What is Virtualization?  
Virtualization is a technology that enables the creation of virtual instances of physical resources such as servers, networks, and storage, improving efficiency and flexibility.  

## What is a Virtual Machine (VM)?  
A virtual machine is an isolated computing environment that functions as a separate operating system within a host machine.  

## Differences Between Rocky Linux and Debian  
- **Rocky Linux**: A community-driven, enterprise-grade Linux distribution that is binary-compatible with Red Hat Enterprise Linux (RHEL).  
- **Debian**: A widely used, stable, and secure Linux distribution with an extensive package repository.  

## AppArmor and apt vs. aptitude  
- **AppArmor**: A Linux security module that restricts applications' privileges to enhance security.  
- **apt** vs. **aptitude**: Both are package management tools in Debian-based systems, but `aptitude` offers a more advanced dependency resolver.  

## Partitions and Configuration  
Partitions divide a disk into sections for better data organization.  

### Viewing Partitions  
Use the following commands to inspect disk partitions:  
```bash
fdisk -l  
lsblk  
df -h  
