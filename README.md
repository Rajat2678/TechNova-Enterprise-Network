# TechNova Enterprise Network

### Enterprise Network Design and Implementation | Cisco Packet Tracer

## Project Overview

Designed and implemented a simulated enterprise network for TechNova, connecting a Head Office, Branch Office and ISP network.

The project focuses on enterprise network infrastructure, routing, switching, network security and centralized network services.

## Network Architecture

The network consists of:
- 3 Routers — HQ-R1, ISP-R2, BRANCH-R3
- 5 Switches — Core, Departmental, Server and Branch switches
- 2 Servers — DHCP/DNS Server and Application Server
- Multiple departmental PCs
- 7 VLANs across Head Office and Branch networks

## Technologies and Skills

- VLAN Configuration and Trunking
- Inter-VLAN Routing (Router-on-a-Stick)
- Spanning Tree Protocol (STP)
- DHCP and DHCP Relay
- DNS Configuration
- Static Routing
- SSH Version 2
- Extended Access Control Lists (ACL)
- Switch Port Security
- NAT/PAT (Overload)
- Network Troubleshooting

## VLAN and IP Addressing

| VLAN | Department | Network |
|---|---|---|
| 10 | HR | 192.168.10.0/24 |
| 20 | IT | 192.168.20.0/24 |
| 30 | Finance | 192.168.30.0/24 |
| 40 | Sales | 192.168.40.0/24 |
| 50 | Servers | 192.168.50.0/24 |
| 99 | Management | 192.168.99.0/24 |
| 60 | Branch | 192.168.60.0/24 |

## Network Services

- Centralized DHCP for Head Office VLANs.
- Branch DHCP configured on BRANCH-R3.
- DNS record: www.xyz.local
- Application Server hosted at 192.168.50.11.
- Inter-VLAN and Branch-to-HQ communication.

## Network Security

- SSH Version 2 for secure remote administration.
- Extended ACL restricting HR-to-Finance traffic.
- Sticky MAC-based switch port security.
- Restrict violation mode on secured access ports.

## NAT/PAT

Configured NAT overload on HQ-R1 to translate internal network addresses using the WAN interface address.

An ISP router loopback address (203.0.113.1) was used as a simulated external test destination.

## Testing and Verification

The following were tested:
- VLAN and trunk configuration.
- Inter-VLAN connectivity.
- DHCP address assignment.
- DNS name resolution.
- HTTP application access.
- Branch-to-HQ connectivity.
- SSH remote management.
- ACL traffic restrictions.
- Switch port security.
- NAT/PAT translations.

## Project Files

- Cisco Packet Tracer topology file.
- Network configuration screenshots.
- Project documentation in PDF and Word formats.

## Learning Outcomes

Gained practical experience in enterprise network design, routing and switching, network segmentation, infrastructure services, remote device administration and network security.

## Tools Used

Cisco Packet Tracer | Cisco IOS CLI

---

**Project Type:** Networking Lab / Simulation  
**Domain:** Enterprise Networking  
**Status:** Implemented and tested in Cisco Packet Tracer
