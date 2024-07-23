# Information Gathering on Websites Using Linux

## Overview

This repository contains lab exercises focused on information gathering and network analysis using various tools on Linux. Each lab demonstrates different techniques and tools for security assessments, including Nmap for network scanning, Macchanger for MAC address spoofing, Netstat for port enumeration, and Wireshark for protocol analysis.

## Labs

### Lab 1: Nmap

**Objective:** Find the IP address, OS details, port details, and service details of a target machine.

**Commands:**

```bash
# Scan the target machine to find its IP address
nmap -sn <target-ip>

# Find OS details
nmap -O <target-ip>

# Scan for open ports and identify services
nmap -sV <target-ip>

# Example of a comprehensive scan
nmap -A <target-ip>

## Lab 2: Macchanger
Objective: Experiment with changing your MAC address to understand how it can help in maintaining anonymity or bypassing certain security measures.

Commands:

bash
Copy code
# Install macchanger (if not already installed)
sudo apt-get install macchanger

# Show current MAC address
ip link show <interface>

# Change MAC address
sudo macchanger -r <interface>

# Verify the new MAC address
ip link show <interface>


## Lab 3: Netstat
Objective: Use Netstat on Windows to enumerate ports and display the routing table of a machine.

Commands:

bash
Copy code
# Display all open ports and associated IP addresses
netstat -an

# Show routing table
netstat -r

# Display listening ports with their associated application
netstat -ab

## Lab 4: Wireshark
Objective: Identify different protocols, find the protocol through which data is passed, and analyze TCP streams to find actual data being transmitted.

Commands:

Capture packets using Wireshark:

Open Wireshark and start capturing on the desired network interface.
Analyze protocols:

Use the "Protocol" filter to identify different protocols.
Find and analyze TCP streams:

Filter for TCP streams and follow the stream to see actual data being transmitted.



### Steps to Add This to GitHub

1. **Create a new repository** on GitHub.

2. **Clone the repository** to your local machine:

   ```bash
   git clone https://github.com/yourusername/Information-Gathering-Linux.git
   cd Information-Gathering-Linux



