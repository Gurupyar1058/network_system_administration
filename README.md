# network_system_administration
 🖧 Minor Project: Departmental Network Simulation using Cisco Packet Tracer

This project simulates a structured departmental network for an organization using *Cisco Packet Tracer*. It demonstrates how multiple departments can be connected securely and efficiently using routers and switches with assigned IP addressing and gateway configurations.

---

## 📌 Table of Contents

- [Features](#features)
- [Devices Used](#devices-used)
- [Network Topology](#network-topology)
- [IP Addressing Scheme](#ip-addressing-scheme)
- [Router & Switch Configurations](#router--switch-configurations)
- [Screenshots](#screenshots)
- [How to Run](#how-to-run)
- [Results](#results)
- [Conclusion](#conclusion)

---

## 🌟 Features

- Multi-department topology with CS, HR, and IT departments.
- Centralized server and admin PC for management.
- Full IP-based routing with static IP addresses.
- Default gateway configurations for each subnet.
- Inter- and intra-department communication verified through ping tests.

---

## 🛠 Devices Used

- 🖥 13 PCs (1 Admin PC, 12 Department PCs)
- 🌐 1 Router
- 🔀 4 Switches
- 📡 Copper Straight-through Cables
- 🖧 1 Server

---

## 🗺 Network Topology

*Router Interface to Switch Connections:*

| Router Interface | Switch  | Port on Switch |
|------------------|---------|----------------|
| f1/1           | Switch0 | fa0/3         |
| f0/0           | Switch1 | fa0/5         |
| f0/1           | Switch2 | fa0/5         |
| f1/0           | Switch3 | fa0/5         |

*Switch-to-PC Connections:*

| Switch   | Connected PCs                     |
|----------|-----------------------------------|
| Switch0  | Admin PC                          |
| Switch1  | PC1, PC2, PC3, PC4 (CS Dept.)     |
| Switch2  | PC5, PC6, PC7, PC8 (HR Dept.)     |
| Switch3  | PC9, PC10, PC11, PC12 (IT Dept.)  |

---

## 🧾 IP Addressing Scheme

### CS Department (Switch1)
| PC    | IP Address     | Default Gateway |
|-------|----------------|------------------|
| PC1   | 192.168.2.2    | 192.168.2.1      |
| PC2   | 192.168.2.3    | 192.168.2.1      |
| PC3   | 192.168.2.4    | 192.168.2.1      |
| PC4   | 192.168.2.5    | 192.168.2.1      |

### HR Department (Switch2)
| PC    | IP Address     | Default Gateway |
|-------|----------------|------------------|
| PC5   | 192.168.3.2    | 192.168.3.1      |
| PC6   | 192.168.3.3    | 192.168.3.1      |
| PC7   | 192.168.3.4    | 192.168.3.1      |
| PC8   | 192.168.3.5    | 192.168.3.1      |

### IT Department (Switch3)
| PC    | IP Address     | Default Gateway |
|-------|----------------|------------------|
| PC9   | 192.168.4.2    | 192.168.4.1      |
| PC10  | 192.168.4.3    | 192.168.4.1      |
| PC11  | 192.168.4.4    | 192.168.4.1      |
| PC12  | 192.168.4.5    | 192.168.4.1      |

---

## 🔧 Router & Switch Configurations

- Router interfaces are configured with IP addresses matching each subnet's gateway.
- Static IPs manually assigned to each PC.
- Default gateways set according to router interface IPs.
- Server and Admin PC connected via Switch0.

---

## 🖼 Screenshots

> Include screenshots of:
> - Packet Tracer layout
> - IP configuration window for any PC
> - Ping test results between departments
> - Successful server communication

---

## 🚀 How to Run

1. Open Cisco Packet Tracer.
2. Load the .pkt file provided in this repository.
3. Click on any PC to verify IP configuration.
4. Use the Command Prompt tool inside PCs to perform ping tests.
5. Ensure router interfaces are turned on and configured.

---

## ✅ Results

- Successful *inter-department communication* via router.
- Server was accessible from all PCs.
- *Ping* results were positive across all configured IPs.
- *Logical segmentation* achieved without communication loss.

---

## 🧾 Conclusion

This simulation reflects a realistic network layout for small organizations, highlighting efficient departmental segmentation using switches and centralized routing. It can be further scaled by adding VLANs, firewall configurations, and dynamic routing protocols.

---

