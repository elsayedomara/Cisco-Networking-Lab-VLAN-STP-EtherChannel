# Cisco Networking Lab - VLAN, STP & EtherChannel

A hands-on Cisco Packet Tracer networking project covering VLANs, trunking, STP, EtherChannel, IP addressing, and connectivity testing.

## Project Overview

This project was built using Cisco Packet Tracer to practice essential Cisco networking concepts and configuration techniques.

## Technologies & Concepts

- Cisco Packet Tracer
- VLANs
- Access Ports
- Trunking
- 802.1Q Encapsulation
- Spanning Tree Protocol (STP)
- EtherChannel with LACP
- IP Addressing
- Connectivity Testing

## Network Topology

The network consists of two Cisco switches and six PCs.

- SW1: PC1, PC2, PC3
- SW2: PC4, PC5, PC6
- Inter-switch trunk connection
- VLANs 10, 20, and 30

## VLAN Configuration

| VLAN | Name |
|------|------|
| 10 | IT |
| 20 | HR |
| 30 | SALES |

### Access Ports

| Port | VLAN |
|------|------|
| Fa0/1 | VLAN 10 |
| Fa0/2 | VLAN 20 |
| Fa0/3 | VLAN 30 |

## IP Addressing

| Device | IP Address | Subnet Mask |
|--------|------------|-------------|
| PC1 | 192.168.10.11 | 255.255.255.0 |
| PC2 | 192.168.20.11 | 255.255.255.0 |
| PC3 | 192.168.30.11 | 255.255.255.0 |
| PC4 | 192.168.10.12 | 255.255.255.0 |
| PC5 | 192.168.20.12 | 255.255.255.0 |
| PC6 | 192.168.30.12 | 255.255.255.0 |

## Trunking

The inter-switch connection was configured as a trunk using 802.1Q and allows VLANs 10, 20, and 30.

## STP

STP was configured for VLAN 20.

SW1 was configured with a priority of 4096 to make it the Root Bridge for VLAN 20.

## EtherChannel

An EtherChannel was configured between the switches using LACP.

The Port-Channel operates as a trunk and carries VLANs 10, 20, and 30.

## Connectivity Testing

Connectivity was tested between devices in the same VLAN:

- PC1 → PC4
- PC2 → PC5
- PC3 → PC6

The connectivity tests were successful.

## Packet Tracer File

The complete Packet Tracer project file is included in this repository:

`Cisco_Networking_Practical_Project.pkt`

## Project Evidence

The repository includes screenshots showing:

- Network topology
- VLAN configuration
- Connectivity testing
- VLAN verification
- Trunk verification
- STP verification
- EtherChannel verification
