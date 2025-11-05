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
| Hypervisor | VirtualBox / VMware Workstation / Proxmox | Host VMs |
| Router / Firewall | pfSense / VyOS / MikroTik CHR | Routing, firewall, VPN |
| Server | Ubuntu Server / Windows Server | DHCP, DNS, File Services |
| Clients | Ubuntu Desktop / Windows 10 | End-user devices |
| Tools | Wireshark, Nmap, PuTTY, GNS3 / Cisco Packet Tracer | Packet capture, simulation, testing |

---

## 🗓️ Weekly Lab Breakdown

---

### **Week 1 – Networking Fundamentals**

**Topics Covered:**  
- OSI & TCP/IP models  
- MAC vs IP addressing  
- Subnetting basics  

**Lab Tasks:**  
- Create two VMs with static IPs  
- Test connectivity using `ping` and `traceroute`  
- Capture ICMP traffic in **Wireshark**  

**Deliverables:**  
- Wireshark capture screenshot  
- Topology diagram  
- Summary paragraph  

**Notes / Reflection:**  
_Example: Learned how each layer of OSI interacts during a ping request and confirmed IP-to-MAC address resolution._

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
