# CompTIA-N10-009-Lab-Portfolio
Networking labs to showcase proficiency, with a side of fries and coke. 

**Created by:** Joe   

**Start Date:** 11/04/2025 

**End Date:** 12/31/2025 

This portfolio documents my hands-on networking projects and labs completed while studying for the **CompTIA Network+ (N10-009)** certification.  
Each week focuses on a major networking domain and demonstrates applied knowledge through virtual labs, configurations, and analysis.

---

## ⚙️ Lab Environment Overview

| Component | Tool / OS | Purpose |
|------------|------------|----------|
| Hypervisor | VirtualBox / VMware Workstation Pro / Hyper-V | Virtualization |
| Router / Firewall | Zerotier | Routing, firewall, VPN |
| Server | Ubuntu Server / Windows Server | DHCP, DNS, File Services |
| Clients | Ubuntu Desktop / Windows 10 | End-user devices |
| Tools | Wireshark, Nmap, PuTTY, GNS3 / Cisco Packet Tracer | Packet capture, simulation, testing |

---

## 🗓️ Weekly Lab Breakdown

---

### **Week 1 – Networking Fundamentals**

# 🗂️ Week 1 — Virtualization & Basic Networking Lab
This week focused on building the foundation of my Network+ home lab using multiple hypervisors (Hyper-V and VMware Workstation Pro) and verifying VM-to-VM connectivity across the same network.  

---

## 🔧 Lab Objectives
- Build a multi-hypervisor virtual environment  
- Install Ubuntu Desktop (VMware + Hyper-V)  
- Install Ubuntu Server (VMware)  
- Connect all VMs to the same network  
- Verify communication using `ip a` and `ping`  
- Document results with screenshots  

---

## 🖥️ Virtual Machines Used
| VM Name | Hypervisor | OS | Purpose |
|--------|------------|----|---------|
| `ubuntu-desktop-vmware` | VMware Workstation | Ubuntu Desktop 22.04 | Client workstation |
| `ubuntu-desktop-hyperv` | Hyper-V | Ubuntu Desktop 22.04 | Second workstation |
| `ubuntu-server` | VMware Workstation | Ubuntu Server 22.04 | Server for future labs |

---

## 🌐 Network Topology (Week 1)

[ VMware Ubuntu Desktop ]
→ Same subnet → Full connectivity
[ Hyper-V Ubuntu Desktop ] /
|
[ Ubuntu Server (VMware) ] — Added to same network, reachable by both desktops


All VMs were placed on the same broadcast domain using bridged networking + ZeroTier where needed.

---

## 📝 Network Verification

### 1️⃣ **Ubuntu Desktop #1 — IP Address (`ip a`)**
![Ubuntu Desktop IP](https://github.com/UnSloppyJoe/CompTIA-N10-009-Lab-Portfolio/blob/main/images/Ubuntu%20Client%201%20ip%20a.png)

### 2️⃣ **Ubuntu Desktop #2 — IP Address (`ip a`)**
![Ubuntu Desktop 2 IP](https://github.com/UnSloppyJoe/CompTIA-N10-009-Lab-Portfolio/blob/main/images/Ubuntu%20Hyper%20V%201%20ip%20a.png)

### 3️⃣ **Ubuntu Server — IP Address (`ip a`)**
![Ubuntu Server IP](https://github.com/UnSloppyJoe/CompTIA-N10-009-Lab-Portfolio/blob/main/images/Ubuntu%20VM%20Server%20ip%20a.png)

---

## 🔄 Connectivity Tests

### 🔹 VM → VM Ping Test (Desktop 1 → Desktop 2 & Server)
![Ping Test 1](https://github.com/UnSloppyJoe/CompTIA-N10-009-Lab-Portfolio/blob/main/images/Ubuntu%20Client%201%20ping%20to%20hyper%20v%20%26%20server.png)

### 🔹 VM → Server Ping Test (Desktop 2 → Server)
![Ping Test 2](https://github.com/UnSloppyJoe/CompTIA-N10-009-Lab-Portfolio/blob/main/images/Ubuntu%20Hyper%20V%20ping%20to%20Server.png)

### 🔹 Server → Hyper-V Desktop Ping Test (Server → Desktop 1)
![Ping Test 3](https://github.com/UnSloppyJoe/CompTIA-N10-009-Lab-Portfolio/blob/main/images/Ubuntu%20VM%20Server%20ping%20to%20UClient%201.png)

---

## 📚 What I Learned This Week
- How virtualization works across multiple hypervisors  
- Difference between bridged, NAT, and external switches  
- How to check Linux network interfaces (`ip a`)  
- How ARP/Neighbor discovery works (`ip neigh`)  
- How to verify connectivity using ICMP (`ping`)  
- How to document a lab environment professionally  

---

## 📸 Screenshots Folder Reference
All Week 1 screenshots are stored in:

/images/week1/


File naming format:

Ubuntu Client 1 ip a.png
Ubuntu Client 1 ping to hyper v & server.png
Ubuntu Hyper V 1 ip a.png
Ubuntu Hyper V ping to Server.png
Ubuntu VM Server ip a.png
Ubuntu VM Server ping to UClient 1.png


---

## ✅ Week 1 Completed
This completes the foundational environment for the coming weeks, where I will add routing, firewalls, services, VLANs, NAT, static routing, and more as part of my Network+ portfolio.


---

### **Week 2 – IP Addressing & Subnetting**

**Topics Covered:**  
- IPv4/IPv6, subnet masks, CIDR notation  

**Lab Tasks:**  
- Design 3 subnets:  
  - 192.168.10.0/24 (LAN A)  
  - 192.168.20.0/24 (LAN B)  
  - 192.168.30.0/24 (Servers)  
- Assign IPs and test connectivity  

**Deliverables:**  
- IP plan diagram  
- Subnetting table  
- Ping verification screenshot  

**Notes / Reflection:**  
_Example: Practiced calculating subnet boundaries and verified proper routing between subnets._

---

### **Week 3 – Routers, Switches, and Routing**

**Topics Covered:**  
- Default gateways, routing tables, static vs dynamic routing  

**Lab Tasks:**  
- Install **pfSense** or **VyOS** as router  
- Configure static routes between LANs  
- Verify with `traceroute`  

**Deliverables:**  
- pfSense interface screenshot  
- Routing table  
- Connectivity proof  

---

### **Week 4 – DHCP & DNS**

**Topics Covered:**  
- DHCP lease process (DORA)  
- DNS resolution and record types  

**Lab Tasks:**  
- Configure **DHCP** and **DNS** on Ubuntu Server  
- Capture DHCP handshake using Wireshark  

**Deliverables:**  
- DHCP leases screenshot  
- DNS query results  
- Wireshark capture  

---

### **Week 5 – Network Services & File Sharing**

**Topics Covered:**  
- SMB, FTP, HTTP basics  

**Lab Tasks:**  
- Create a Samba share  
- Configure Apache/Nginx web server  
- Access services from clients  

**Deliverables:**  
- Screenshot of shared folder or web page  
- Configuration summary  

---

### **Week 6 – Network Security**

**Topics Covered:**  
- Firewalls, ACLs, and VPNs  

**Lab Tasks:**  
- Create firewall rules in pfSense  
- Test with **Nmap** scans  
- (Optional) Configure site-to-site VPN  

**Deliverables:**  
- Firewall rules screenshot  
- Nmap output  
- VPN connection proof (if configured)  

---

### **Week 7 – Network Troubleshooting**

**Topics Covered:**  
- Common CLI tools: `ping`, `ipconfig`, `traceroute`, `nslookup`, `netstat`  

**Lab Tasks:**  
- Break network intentionally (disable DHCP, wrong IP, etc.)  
- Troubleshoot and fix  
- Document the process  

**Deliverables:**  
- Before/after screenshots  
- Troubleshooting summary  
