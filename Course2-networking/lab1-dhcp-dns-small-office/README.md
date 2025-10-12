# Lab 1 — Small Office Network with DHCP and DNS

### 🎯 Objective
Design and configure a small office network where all clients receive dynamic IP addresses (via DHCP) and resolve hostnames using a DNS server.

### 🧰 Tools
- Cisco Packet Tracer 8.2
- Router (ISR 4321)
- Switch (2960)
- 2 PCs
- 1 Server

### ⚙️ Configuration Summary
| Device | Function | Key Config |
|--------|-----------|------------|
| Router | DHCP server | Assigned IPs from 192.168.10.0/24 |
| Server | DNS | Mapped `server.local` → 192.168.10.10 |
| PCs | Clients | Auto-configured via DHCP |

### ✅ Verification
- Each PC received unique IPs from the pool  
- `ping server.local` resolved successfully  
- DNS and DHCP working end-to-end

### 📸 Screenshots
![Topology](./screenshot)

### 💭 Reflection
This lab deepened my understanding of how network services (DHCP/DNS) simplify administration in enterprise and cloud environments.  
In the cloud, these same principles appear as **VPC DHCP options** and **Cloud DNS services** — automated but conceptually identical.

---

> *“Networking is the skeleton; everything else in IT — from MySQL replication to Kubernetes — is built on it.”*

