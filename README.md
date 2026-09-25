# network-traffic-analysis-wireshark
# Network Traffic Analysis & Packet Investigation using Wireshark

## Project Overview

This project demonstrates network traffic capture and packet analysis using Wireshark in a controlled VMware lab environment.

The objective was to capture and analyze different types of network traffic, including ICMP, TCP/HTTP, and ARP, and understand how these protocols behave during normal network communication.

## Objectives

- Capture network traffic using Wireshark
- Analyze ICMP packets
- Analyze TCP and HTTP communication
- Analyze ARP requests and responses
- Use Wireshark display filters
- Understand basic packet-level network investigation

## Lab Environment

| Component | Details |
|---|---|
| Operating System | Parrot OS |
| Network Analysis Tool | Wireshark |
| Target | Metasploitable 2 |
| Virtualization | VMware Workstation |
| Network Interface | ens33 |
| Parrot OS IP | 192.168.36.128 |
| Target IP | 192.168.36.129 |

## Tools Used

- **Wireshark** – Packet capture and network traffic analysis
- **Parrot OS** – Security testing environment
- **VMware Workstation** – Virtual lab environment
- **Metasploitable 2** – Lab target for generating network traffic

## Methodology

The project followed these steps:

1. Identified the correct network interface.
2. Started packet capture on `ens33`.
3. Generated ICMP traffic between Parrot OS and Metasploitable 2.
4. Generated TCP/HTTP traffic to the target web server.
5. Generated ARP traffic on the local network.
6. Applied Wireshark display filters.
7. Analyzed the captured packets.

## 1. ICMP Traffic Analysis

ICMP traffic was generated using:

```bash
ping -c 4 192.168.36.129
