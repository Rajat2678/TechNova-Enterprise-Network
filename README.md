# TechNova Enterprise Network

### Enterprise Network Design and Implementation | Cisco Packet Tracer

A simulated enterprise network designed and implemented using Cisco Packet Tracer. The project connects a Head Office, Branch Office and ISP network, demonstrating enterprise networking, routing, switching, network services and security.

## 1. Project Overview

The objective was to design a scalable and secure enterprise network with departmental segmentation, centralized network services and connectivity between different locations.

**Network components:**
- 3 Routers: HQ-R1, ISP-R2, BRANCH-R3
- 5 Switches: CORE-SW1, HR-IT-SW2, FIN-SALES-SW3, SERVER-SW4, BRANCH-SW5
- 2 Servers: DHCP/DNS Server and Application Server
- Multiple departmental PCs
- 7 VLANs across Head Office and Branch networks

## 2. Network Architecture

The network consists of three main sections:

- **Head Office:** Departmental VLANs for HR, IT, Finance, Sales, Servers and Management.
- **Branch Office:** A separate branch LAN connected to the Head Office through a router.
- **ISP Network:** A simulated ISP connection providing an external test destination.

## 3. VLAN and IP Addressing Plan

| VLAN | Department | Network | Gateway |
|---|---|---|---|
| 10 | HR | 192.168.10.0/24 | 192.168.10.1 |
| 20 | IT | 192.168.20.0/24 | 192.168.20.1 |
| 30 | Finance | 192.168.30.0/24 | 192.168.30.1 |
| 40 | Sales | 192.168.40.0/24 | 192.168.40.1 |
| 50 | Servers | 192.168.50.0/24 | 192.168.50.1 |
| 99 | Management | 192.168.99.0/24 | 192.168.99.1 |
| 60 | Branch | 192.168.60.0/24 | 192.168.60.1 |

## 4. Technologies Implemented

- VLAN Configuration and Departmental Segmentation
- Trunking using IEEE 802.1Q
- Inter-VLAN Routing using Router-on-a-Stick
- Spanning Tree Protocol (STP)
- DHCP and DHCP Relay using IP Helper Address
- DNS Configuration and Name Resolution
- HTTP and HTTPS Application Server
- Static Routing between Head Office, Branch and ISP
- SSH Remote Device Management
- Extended Access Control Lists (ACLs)
- Switch Port Security with Sticky MAC and Restrict Mode
- Network Address Translation (NAT)
- Port Address Translation (PAT / NAT Overload)

## 5. Network Security

The following security features were configured:

- SSH Version 2 for secure remote administration.
- Local authentication on routers and switches.
- Extended ACL restricting HR-to-Finance communication.
- Port Security limiting the number of MAC addresses on access ports.
- Sticky MAC address learning and Restrict violation mode.

## 6. Network Services

**DHCP:** Centralized DHCP service for Head Office VLANs, with DHCP relay configured on the router. Branch DHCP is provided by BRANCH-R3.

**DNS:** Configured the domain `www.xyz.local` to resolve to the Application Server.

**Web Server:** HTTP and HTTPS services enabled on the Application Server at `192.168.50.11`.

## 7. Routing and NAT

Static routes were configured to provide communication between the Head Office, Branch and simulated ISP.

PAT was implemented on HQ-R1 using its ISP-facing interface to translate internal private addresses to the WAN interface address.

A simulated external test destination (`203.0.113.1`) was used to verify connectivity and NAT translations.

## 8. Testing and Verification

The following tests were performed:

- VLAN and trunk verification.
- Inter-VLAN connectivity.
- DHCP address allocation.
- DNS name resolution.
- HTTP access using IP address and domain name.
- SSH access to routers and switches.
- ACL policy verification.
- Port Security status and violation counters.
- NAT/PAT translation verification.
- Head Office-to-Branch connectivity.
- End-to-end connectivity testing.

## 9. Project Files

- Packet Tracer project: `Project/TechNova_Enterprise_Network.pkt`
- Verification screenshots: Repository screenshot files.

## 10. Skills Demonstrated

Cisco Networking | Routing and Switching | VLANs | STP | DHCP | DNS | ACL | NAT/PAT | SSH | Network Troubleshooting | Cisco Packet Tracer

## 11. Learning Outcome

This project provided practical experience in designing, configuring, securing and troubleshooting a multi-location enterprise network using Cisco Packet Tracer.

---

**Tools Used:** Cisco Packet Tracer  
**Project Type:** Enterprise Networking Lab  
**Repository:** GitHub

