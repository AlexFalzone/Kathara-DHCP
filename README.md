# Kathara Lab with DHCP

## Overview

This Kathara lab is designed to simulate a network environment with two hosts on separate domains connected by a router that also functions as a DHCP server. The lab demonstrates the configuration of DHCP settings to dynamically assign IP addresses to the hosts.

## Lab Configuration

### Router (Router/DHCP Server)

- **Interfaces:**
  - Eth0: Connected to Host A (192.168.1.0/24)
  - Eth1: Connected to Host B (10.0.1.0/24)

- **DHCP Configuration:**
  - Eth0
    - DHCP Pool: 192.168.2.2 to 192.168.2.100
    - Subnet Mask: 255.255.255.0
  - Eth1
    - DHCP Pool: 10.0.1.50 10.0.1.200
    - Subnet Mask: 255.255.255.0


### PC1

- **Domain:** domain_A
- **IP Configuration:** DHCP Client

### PC2

- **Domain:** domain_B
- **IP Configuration:** DHCP Client

## Setup Instructions

1. Ensure that you have Kathara installed on your system. If not, follow the installation instructions: [Kathara Installation Guide](https://github.com/KatharaFramework/Kathara/wiki/Installation).

2. Download the lab configuration files from this repository.

3. Open a terminal in the directory where the lab files are located.

4. Run the following command to start the Kathara lab:

    ```bash
    kathara lstart
    ```

5. Once the lab is started, try pinging pc1 from pc2 or vice versa.

## Additional Notes

- Feel free to explore additional configurations and scenarios to enhance your understanding of networking concepts.
