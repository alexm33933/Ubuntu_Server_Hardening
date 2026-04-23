# Ubuntu_Server_Hardening English

## What is Hardening?
Hardening is the process of establishing a minimun level of security. It involves securing different components such as the file system, user accounts, services, software updates, etc. This process follows recognized best practices and standards defined by worldwide organizations, such as ISO/IEC 27001 and ISO/IEC 27002.

## Introduction
This proyect explains how to configure an Ubuntu Server VM (v24.04 LTS) to enhance security across all systems layers. The lab environment is deployed on VMware WorkStation, running on a Windows 11 host system.

## Objectives
The main objective of this proyect is to apply security hardening techniques to an Ubuntu Server VM. This includes reducing the attack surface, securing access, and implementing bes practices to protect the system against common threats.

## Environment
- Host OS: Windows 11
- Virtualization Platform: VMware WokstStation PRO 17
- Gest OS: Ubuntu Server 24.04 LTS
- Network: NAT or Bridged

## Initial Setup
After installing Ubuntu Server with the default configuration, the system should be updated to ensure all packages are current:

sudo apt update && sudo apt upgrade -y

A noon-root user is created to perform administrative tasks.

## SSH Configuration
The first step is to configure SSH Key-based authentication by adding the public key to the server. This improves security by removing the need for password-based.

To generate a Key Pair, run the following command on the client machine:
ssh-keygen -t ed25519

Copy the public key to the server:
ssh-copy-id user@server_ip

# Ubuntu_Server_Hardening Español









