<div align="center">

# 🔐 Cybersecurity Lab Environment Setup

### Building an isolated virtual lab for penetration testing and ethical hacking practice

</div>

---

<p align="center">

![Cybersecurity](https://img.shields.io/badge/Skill-Cybersecurity-red)
![VirtualBox](https://img.shields.io/badge/VirtualBox-v7.2-blue)
![Kali Linux](https://img.shields.io/badge/Kali%20Linux-v2026.2-orange)
![Linux](https://img.shields.io/badge/Skill-Linux-red)
![Network](https://img.shields.io/badge/Network-10.0.0.0%2F24-blue)
![Penetration Testing](https://img.shields.io/badge/Penetration%20Testing-red)

![Virtualization](https://img.shields.io/badge/Skill-Virtualization-red)
![GitHub](https://img.shields.io/badge/GitHub-black)
![Ethical Hacking](https://img.shields.io/badge/Ethical%20Hacking-red)

</p>

---

## 📌 Project Overview

This project focuses on setting up a virtual cybersecurity and
penetration-testing laboratory using VirtualBox and Kali Linux.

The purpose of the lab is to create a controlled environment where
cybersecurity tools, network scanning, reconnaissance, vulnerability
assessment, and other security-testing activities can be performed
safely and repeatedly.

The lab is configured on a private virtual network so that additional
machines can be added later and used as targets for authorized security
testing.

---

## 🎯 Objectives

The main objectives of this project are to:

- Install and configure VirtualBox.
- Install/import Kali Linux as a virtual machine.
- Create a private NAT Network for the cybersecurity lab.
- Configure network connectivity for Kali Linux.
- Assign a consistent IP address to the Kali VM.
- Verify network connectivity and DNS resolution.
- Take a clean VM snapshot for recovery.
- Document the complete setup process.
- Prepare the environment for future cybersecurity projects.

---

## 🛡️ Purpose of the Lab
The purpose is to Build an isolated cybersecurity laboratory to carry out the following activities:

- Network reconnaissance
- Port scanning
- Vulnerability assessment
- Packet analysis
- Web security testing
- Exploitation practice
- Security-tool experimentation

---

## 🏗️ Lab Configuration

---

|🧩 Component | ⚙️ Configuration |
| ------- | ---------------- |
| 🖥️ Host OS	| Windows 10        |
| 🧠 Host RAM	| 8 GB   |
| ⚡ Processor	Intel | Core i7   |
| 🧰 Hypervisor	| VirtualBox 7.2 |
| 🐉 Security OS	| Kali Linux 2026.2 |
| 🧠 Kali RAM	| 2048 MB |
| 🌐 Virtual Network	| NAT Network |
| 📡 Network Address	| 10.0.0.0/24 |
| 🐧 Kali IP Address	| 10.0.0.2/24 |
| 🚪 Default Gateway	| 10.0.0.1 |
| 🌍 DNS Server	 | 8.8.8.8 |
| 🔮 Future VM Range |	10.0.0.3–10.0.0.99 |
  

---

## 💻 Virtual Machines

---

| Machine | Operating System | IP Address | Purpose                |
| ------- | ---------------- | ---------- | ---------------------- |
| VM 1    | Kali Linux       | 10.0.0.10  | Security workstation   |
| VM 2    | Linux Target     | 10.0.0.20  | Authorized test target |
| VM 3    | Windows Target   | 10.0.0.30  | Authorized test target |

---

## 🪜 Lab Setup Procedure

---

## Step 1. Install VirtualBox

---

VirtualBox was installed as the hypervisor.

---

## Step 2. Create the NAT Network

---

A dedicated NAT Network was created in VirtualBox.

Configuration: 

Network Name: NatNetwork 

IPv4 Prefix: 10.0.0.0/24 

DHCP: Enabled 

IPv6: Disabled

A NAT Network was selected because multiple virtual machines connected to the same NAT Network can communicate with one another while also having outbound network connectivity.

---

## Step 3. Import Kali Linux

---

The Kali Linux virtual machine was downloaded from the official Kali Linux website and imported into VirtualBox.

The VM network adapter was configured as follows:

```text
Adapter 1
Attached to: NAT Network
Network:     NatNetwork
Adapter Type: Intel PRO/1000 MT Desktop
```

The VM was allocated:

```text
RAM: 2048 MB
```
---

## Step 4. Configure the Kali Linux Network

The Kali Linux network configuration was checked and configured with a consistent IPv4 address.

Example configuration:

```text
IP Address: 10.0.0.2
Subnet Mask: 255.255.255.0
Gateway: 10.0.0.1
DNS: 8.8.8.8
```
A consistent IP address makes it easier to document the lab and reference the Kali machine in future exercises.

---

## 🔐 Security & Ethical Use

---

This laboratory is intended strictly for education purposes only.

---

## 🔗 Tools & Resources

---

VirtualBox: https://virtualbox.org/wiki/Downloads

Kali Linux: https://kali.org/get-kali

---

## 👤 Author

---

Irabor Richard Ehis

Cybersecurity Internship B083

LinkedIn: https://www.linkedin.com/in/richard-ehis-irabor/

---

## 📌 Project Information

Program Name: Cybersecurity at Networkwalks | Week: 01 | Project: Cybersecurity & Pentesting Lab Setup | Repository: GitHub

