# Cycle 1 — Simulation of Star Topology Network

# 🖧 Network Simulation using Cisco Packet Tracer

```text
Name: Ranjith Ganesh B
Reg No: 212223060222
```

## 🎯 AIM

To simulate a **Star Topology network** using Cisco Packet Tracer and verify connectivity between computers using the **ICMP Ping** protocol.

## 🛠️ EQUIPMENTS REQUIRED

- Desktop Computer
- Cisco Packet Tracer

## 📍 IP ASSIGNMENT

All PCs are configured within the same `192.168.1.0/24` network to enable communication through the central switch.

| NAME | IP ADDRESS | SUBNET MASK | NETWORK | CLASS |
|------|------------|-------------|---------|-------|
| PC0 | 192.168.1.10 | 255.255.255.0 | 192.168.1.0 | Class C |
| PC1 | 192.168.1.20 | 255.255.255.0 | 192.168.1.0 | Class C |
| PC2 | 192.168.1.30 | 255.255.255.0 | 192.168.1.0 | Class C |
| PC3 | 192.168.1.40 | 255.255.255.0 | 192.168.1.0 | Class C |
| PC4 | 192.168.1.50 | 255.255.255.0 | 192.168.1.0 | Class C |
| PC5 | 192.168.1.60 | 255.255.255.0 | 192.168.1.0 | Class C |

> **Note:** No default gateway is required because all PCs are configured within the same local network.

## ⚙️ PROCEDURE

1. Open Cisco Packet Tracer.
2. Add a **Cisco 2950 switch** to the workspace.
3. Add six PC terminals to the workspace.
4. Connect each PC to a different port of the switch using **Copper Straight-Through** cables.
5. Configure the IPv4 address and subnet mask for each PC through **Desktop → IP Configuration**.
6. Assign unique IP addresses to all PCs within the `192.168.1.0/24` network.
7. Open **Desktop → Command Prompt** on a PC.
8. Use the `ping` command to verify connectivity with other PCs.
9. Verify that the ICMP packets are successfully transmitted and received without packet loss.
10. The connectivity between the PCs is verified through the central switch, demonstrating the operation of the **Star Topology**.

## 📊 IP CONNECTIVITY TABLE

The following table represents the connectivity between the PCs using ICMP Ping.

| SENDER / RECEIVER | PC0 | PC1 | PC2 | PC3 | PC4 | PC5 |
|-------------------|-----|-----|-----|-----|-----|-----|
| **PC0** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |
| **PC1** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |
| **PC2** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |
| **PC3** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |
| **PC4** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |
| **PC5** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |

**✓ — Successful ICMP connectivity**

## 🗺️ NETWORK DIAGRAM

<img width="1920" height="1080" alt="Screenshot 2026-10-10 110817" src="https://github.com/user-attachments/assets/fc2ef52a-a17f-4109-9e60-db5ba5e1a4f8" />


## 🧾 BASIC NETWORKING COMMANDS

### 1. Display IP Configuration

#### Windows

```text
C:\> ipconfig
```

Displays the IP address, subnet mask, and other network configuration details.

#### Detailed IP Configuration

```text
C:\> ipconfig /all
```

Displays detailed network configuration including MAC address, DHCP information, DNS information, and other adapter details.

---

### 2. Self Ping

To test the local TCP/IP stack:

```text
C:\> ping 127.0.0.1
```

A PC can also ping its own configured IP address:

```text
C:\> ping 192.168.1.10
```

---

### 3. Ping a Destination

To test connectivity with another PC:

```text
C:\> ping <destination-ip-address>
```

Example:

```text
C:\> ping 192.168.1.20
```

A successful response indicates that the destination PC is reachable through the network.

---

### 4. ARP Command

The Address Resolution Protocol (ARP) is used to map IP addresses to MAC addresses.

```text
C:\> arp -a
```

This displays the ARP table containing known IP-to-MAC address mappings.

---

### 5. Trace the Network Route

The `tracert` command is used to trace the path taken by packets to a destination.

```text
C:\> tracert <ip-address>
```

Example:

```text
C:\> tracert 192.168.1.20
```

For an external destination:

```text
C:\> tracert www.saveetha.ac.in
```

## 📤 OUTPUT
<img width="1920" height="1080" alt="Screenshot 2026-10-10 111430" src="https://github.com/user-attachments/assets/86e8c810-27b7-4cbf-adb8-7c6a66637022" />


## ✅ RESULT

Thus, the **Star Topology network was successfully simulated using Cisco Packet Tracer**. Six computers were connected to a central Cisco 2950 switch, and IP addresses were configured within the same network. Connectivity between the computers was successfully verified using **ICMP Ping**, with successful responses and **0% packet loss**.
