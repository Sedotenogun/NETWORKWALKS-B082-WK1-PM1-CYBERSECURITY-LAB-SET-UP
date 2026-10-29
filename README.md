
# NETWORKWALKS-B082-WK1-PM1-CYBERSECURITY-LAB-SET-UP

## Project Overview
This project covers the setup of my cybersecurity lab using VirtualBox and Kali Linux. I configured the network, set up the virtual machine, and worked on getting everything running properly for my cybersecurity practicals.

## Project Objectives
-Install and configure Kali Linux in VirtualBox.
-Create a NAT Network using the 10.0.0.0/24 subnet.
-Configure network settings and internet connectivity.
-Enable clipboard sharing, drag-and-drop, and shared folders.
-Prepare a virtual lab environment for future cybersecurity practicals.

## Tools Used
- Oracle VirtualBox
- Kali Linux

## What I Did
- Set up Kali Linux as a virtual machine.
- Configured a custom NAT Network using the `10.0.0.0/24` subnet.
- Configured the virtual machine's network settings.
- Enabled clipboard sharing, drag-and-drop, and shared folders.
- Worked on ensuring Kali Linux had internet access.

## Lab Setup Procedure
- Downloaded and installed Oracle VirtualBox.
- Downloaded and imported the Kali Linux virtual machine.
- Created a custom NAT Network with the subnet 10.0.0.0/24.
- Configured Kali Linux network settings and assigned the IP address 10.0.0.2/24.
- Enabled clipboard sharing and drag-and-drop in the virtual machine settings.
- Configured a shared folder between the host computer and Kali Linux.
- Tested internet connectivity on Kali Linux.
- Took a snapshot of the virtual machine to save its initial configuration.

## Purpose
Purpose of the Lab
- To create a controlled environment for cybersecurity practice.
- To learn how to use Kali Linux and its security tools.
- To practise network configuration and troubleshooting.
- To explore ethical hacking techniques safely.
- To prepare for hands-on cybersecurity labs and challenges.
- To understand how virtual machines communicate over a network.
- To build practical skills in cybersecurity and network security.
  
## Network configuration
- Operating System: Kali Linux
- Network type: NAT Network
- Network Subnet: 10.0.0.0/24
- Kali Linux IP: 10.0.0.2/24
- Internet access: Configured and tested

## Challenges I Ran Into & How I Fixed Them
- Blank NAT Network Dropdown: The network list was empty because I hadn't created the NAT Network in VirtualBox yet. I fixed this by setting up a new network with the 10.0.0.0/24 subnet.

- NO-CARRIER Network Error: My adapter was stuck down because the virtual "cable" wasn't plugged in. I checked the box in VirtualBox settings and turned the interface on via the terminal.

- DNS Resolution Issues: Kali couldn't reach websites by name at first. I fixed it by manually configuring my static IP (10.0.0.2), gateway (10.0.0.1), and external DNS (8.8.8.8).

- Shared Folder Permission Denied: I couldn't open sf_downloads initially because my user wasn't in the correct group. I ran sudo usermod -aG vboxsf kali and rebooted to gain access.

## What I Learned 
In carrying out this project i learnt the following : 
Virtualization Basics: Got hands-on experience setting up virtual machines in VirtualBox, attaching virtual network adapters, and configuring shared folders between my host PC and Linux.

Linux Networking & Terminal Commands: Learned how to configure static IP addresses, gateways, and DNS servers using command-line tools like nmcli and nmtui.

Real-World Troubleshooting: Learned how to read terminal error messages (like NO-CARRIER and DNS failures) and track down simple fixes, like checking virtual cable connections.

Linux User Permissions: Understood how Linux manages group permissions by adding my user to the vboxsf group to access restricted shared folders.

Documenting the Process: Realized the value of writing down errors and solutions as they happen so I can easily reference them or share them with others.

## Lab Screenshots

### VirtualBox Network Configuration

<img width="1366" height="768" alt="Screenshot network setings 1" src="https://github.com/user-attachments/assets/00861f2c-256c-4844-81a5-4701441a73ae" />

<img width="1366" height="768" alt="Screenshot network settings 2" src="https://github.com/user-attachments/assets/39c4fe2a-11a9-4e9f-b5d2-1195345cff6f" />

### Kali Linux IP Address

<img width="816" height="721" alt="Screenshot Kali Network Settings" src="https://github.com/user-attachments/assets/11d17e4f-83b3-4adb-84c3-5725513a03bf" />

### Internet Connectivity Test

<img width="818" height="722" alt="Screenshot Internet Connectivity test" src="https://github.com/user-attachments/assets/4286b899-ab6c-4a63-a2bc-cf6013d39df1" />





