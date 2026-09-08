# Cybersecurity-Lab-SETUP
**PROJECT OVERVIEW:**
This project focuses on the installation of the Virtual Lab using VirtualBox and Kali Linux for penetration testing and cybersecurity.
The aim of the Lab is to ensure a controlled environment where cybersecurity tools, network scanning, vulnerability assessment, reconnaissance, and other security testing activities are performed safely and repeatedly. 
The lab is configured on a private virtual network so that additional machines can be added later and used as targets for authorized security testing.
**OBJECTIVES**
The main objectives of this project are to:
•	Install and configure VirtualBox.
•	Install/import Kali Linux as a virtual machine.
•	Create a private NAT Network for the cybersecurity lab.
•	Configure network connectivity for Kali Linux.
•	Assign a consistent IP address to the Kali VM.
•	Verify network connectivity and DNS resolution.
•	Take a clean VM snapshot for recovery.
•	Document the complete setup process.
•	Prepare the environment for future cybersecurity projects.
**PURPOSE OF THE LAB**
The lab provides an isolated and controlled environment for cybersecurity learning and authorized security testing.
It can be used for activities such as:
•	Network reconnaissance
•	Port scanning
•	Vulnerability assessment
•	Packet analysis
•	Web security testing
•	Exploitation practice
•	Security-tool experimentation
**LAB SETUP PROCEDURE**
Step 1. Install VirtualBox
VirtualBox was installed as the hypervisor.
Step 2. Create the NAT Network
A dedicated NAT Network was created in VirtualBox.
Configuration: 
Network Name: NatNetwork 
IPv4 Prefix: 10.0.0.0/24 
DHCP: Enabled 
IPv6: Disabled
 
Step 3. Import Kali Linux
The Kali Linux virtual machine was downloaded from the official Kali Linux website and imported into VirtualBox.
The VM network adapter was configured as follows:

Adapter 1
Attached to: NAT Network
Network:     NatNetwork
Adapter Type: Intel PRO/1000 MT Desktop

 
Step 4. Configure the Kali Linux Network
The Kali Linux network configuration was checked and configured with a consistent IPv4 address.
Example configuration:
IP Address: 10.0.0.2
Subnet Mask: 255.255.255.0
Gateway: 10.0.0.1
DNS: 8.8.8.8
A consistent IP address makes it easier to document the lab and reference the Kali machine in future exercises.
 
**Author**
Irabor Richard Ehis
Cybersecurity Professional B083
LinkedIn: https://www.linkedin.com/in/richard-ehis-irabor/

