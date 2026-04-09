# Corporate Multi-Site Network Infrastructure
**CCNA Level Implementation | Layer 3 Switching & OSPF Routing**

## 🚀 Project Overview
This project demonstrates an intermediate-level enterprise network designed in Cisco Packet Tracer. It utilizes a **Collapsed Core Architecture** to provide high-speed Inter-VLAN routing, coupled with a secured Edge Gateway and a remote Branch office connected via OSPF.

### Key Technical Features:
* **VLAN Segmentation:** Logical isolation of departments (HR, IT, Guest, Management, and Services) using 802.1Q trunking to reduce broadcast domains.
* **Layer 3 Intelligence:** High-performance Inter-VLAN routing executed on a Multi-Layer Switch (Core-SW) via Switched Virtual Interfaces (SVIs).
* **Infrastructure Security:** * **Extended ACLs:** Granular traffic filtering to isolate the Guest network from sensitive Management and Branch segments.
    * **Management Plane Hardening:** Secured remote access via SSH (v2) with local AAA and privileged level 15 access.
    * **VLAN Security:** Implementation of a non-default Native VLAN (VLAN 777) to mitigate VLAN Hopping attacks.
* **Network Automation:** Integrated DHCP pools configured directly on the Core Switch for dynamic, zero-touch IP addressing.
* **Dynamic Routing:** OSPF (Area 0) implementation for seamless multi-site reachability, complemented by Static Default Routing for ISP egress.

## 🛠️ Topology Diagram
The diagram below illustrates the hierarchical design, featuring redundant access links and a clear separation between the Service segment and departmental VLANs.

![Network Topology](Topology.png)

## 🧪 Verification Results
### End-to-End Connectivity Test
The following screenshot validates the complete routing stack. A host in **VLAN 10 (HR)** successfully establishes an HTTP session with the **Corporate Web Server (VLAN 50)**, confirming that routing, NAT/Gateways, and ACLs are functioning as intended.

![Web Server Success](WebServerReached.png)

## 📂 How to Use
1. **Download:** Navigate to the `/Project-Files` folder and download the `.pkt` file.
2. **Software:** Open the file using **Cisco Packet Tracer (v8.2 or higher)**.
3. **Management Access:** To verify device configurations via SSH, use the following credentials:
    * **Username:** `admin`
    * **Password:** `admin123`
4. **Testing:** Use the "Simulation Mode" or the "Desktop > Web Browser" tool on any departmental PC to test connectivity across the network.

---

## 👤 Author
**David**
* **Role:** Security Professional | Aspiring Network Engineer
* **Location:** Doha, Qatar
* **Focus:** Integrated Security Systems, Network Infrastructure, and Cyber Operations

## 🎓 Professional Certification Path
This project serves as a practical demonstration of skills acquired while pursuing:
* **Cisco Certified Network Associate (CCNA)**
* **CompTIA Security+**

---
