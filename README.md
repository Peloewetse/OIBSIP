# Basic Network Scanning with Nmap

## Overview
This repository contains documentation and evidence of basic network scanning with Nmap.The scan was done from Kali Linux virtual machine to scan a windows virtual machine.
The goal was to identify open ports and services on the windows host and document the findings.

### Lab Setup
Scanning machine:Kali Linux Vm (Test/Attacker system)
Target Machine:Windows VM (Victim/test sytem)
Network:Both Virtual machines were  connected to the same virtual network for isolated and safe testing.

#### Commands executed
1.nmap --version 
This command was used to identify the version,build and installation of Nmap on Kali Linux.The scan showed the installation was complete and ready for scanning.

2.nmap -sV 127.0.0.1 
This command executed an initial scan against Kali Linux (localhost) to confirm the functionality of Nmap.

3.ipconfig
This command was used to get Windows machine Ip Configuration.

4.nmap -sV windows virtual machine IP -oN nmap_scan_results.txt
This command was used to save the scan results to a text file.

##### Included files:
nmap_scan_results.txt : a raw text output from the Nmap scan.
Nmapscan.png :a screenshot of the scan results.

###### Interpretation of scan results
The scan showed that the machine runs Nmap 7.98 on a 64-bit Linux system and is ready for advanced scanning.
At the time of the scan no services were being run by the Kali Linux machine on default ports thouh it was reachable.
No active services were exposed as there were no enabled services.
The file was saved as the host was reachable but all 1000 common TCP ports were closed.
