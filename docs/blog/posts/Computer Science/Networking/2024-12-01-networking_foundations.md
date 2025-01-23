---
date: 2024-12-01
tags: 
      - CCNA
      - Network
---
# Networking Foundations 
## Module 1: Networking Today
### Key Concepts 
1. **Network Components**:
   - **End Devices**: Devices that originate or receive data
     - PCs 
     - Servers
     - Smartphones
   - **Intermediary Devices**: Devices that facilitate 
   communication
     - Switches 
     - Routers
     - Firewalls
   - **Network Media**: Physical pathways for data transmission 
     - Cables
     - Wireless Signals
     
2. **Network Types**:
   - **LAN (Local Area Network)**: A network within a small geographic area.
   - **WAN (Wide Area Network)**: A network that spans large geographic areas. 
   - **WLAN (Wireless LAN)**: A LAN that uses wireless communication.

3. **Network Protocols**:
   - Rules and standards that govern communication
     - TCP/IP 
     - HTTP
     - FTP
   - Protocols ensure devices can communicate regardless of their underlying hardware or software.

4. **Network Topologies**:
   - The arrangement of devices in a network (e.g., star, mesh, bus).
   - Different topologies have different strengths and **vulnerabilities**.

### Pentesting Relevance
- Identify **network boundaries** and **entry points** (e.g., routers, firewalls).
- Look for **misconfigured devices** or **weak protocols** that can be exploited.
- Example: A misconfigured router could allow unauthorized access to the network.

---

## Module 2: Basic Switch and End Device Configuration

### Key Concepts in Detail
1. **CLI (Command Line Interface)**:
   - A text-based interface for configuring network devices.
   - Common commands:
     - `enable`: Enter privileged EXEC mode.
     - `configure terminal`: Enter global configuration mode.
     - `hostname`: Set the device name.
     - `interface`: Configure specific interfaces.

2. **IP Addressing**:
   - Assigning IP addresses to devices for communication.
   - Example: `192.168.1.1` for a router or `192.168.1.10` for a PC.

3. **Passwords and Security**:
   - Set passwords for device access (e.g., console, privileged EXEC mode).
   - Enable **SSH** for secure remote access instead of insecure protocols like Telnet.

4. **Switch Port Configuration**:
   - Configure switch ports for specific devices or VLANs.
   - Example: `switchport mode access` for connecting end devices.

### Pentesting Relevance
- Test for **weak configurations** (e.g., open ports, default credentials).
- Exploit misconfigured devices to gain access.
- Example: **Default credentials** on a switch can lead to full network compromise.

---

## Module 3: Protocols and Models

### Key Concepts in Detail
1. **OSI Model**:
   - A 7-layer model for understanding network communication:
     1. **Physical**: Transmits raw bits over a physical medium.
     2. **Data Link**: Ensures reliable data transfer between devices on the same network.
     3. **Network**: Handles routing and forwarding of data between networks.
     4. **Transport**: Ensures reliable data delivery (e.g., TCP, UDP).
     5. **Session**: Manages sessions between applications.
     6. **Presentation**: Translates data into a readable format.
     7. **Application**: Provides network services to applications (e.g., HTTP, FTP).

2. **TCP/IP Model**:
   - A simplified 4-layer model:
     1. **Network Access**: Combines Physical and Data Link layers.
     2. **Internet**: Handles IP addressing and routing.
     3. **Transport**: Ensures reliable data delivery (e.g., TCP, UDP).
     4. **Application**: Combines Session, Presentation, and Application layers.

3. **Key Protocols**:
   - **HTTP/HTTPS**: Web browsing.
   - **FTP**: File transfer.
   - **DNS**: Resolves domain names to IP addresses.
   - **ARP**: Maps IP addresses to MAC addresses.

### Pentesting Relevance
- Exploit **protocol weaknesses** (e.g., DNS spoofing, FTP bounce attacks).
- Use protocol knowledge to map network services and vulnerabilities.
- Example: DNS poisoning can redirect traffic to malicious servers.

---

## Module 4: Physical Layer

### Key Concepts in Detail
1. **Network Media**:
   - **Copper Cables**: Use electrical signals (e.g., Ethernet cables).
   - **Fiber Optic Cables**: Use light pulses for high-speed, long-distance communication.
   - **Wireless**: Uses radio waves for communication (e.g., Wi-Fi).

2. **Network Devices**:
   - **Hubs**: Broadcast data to all devices in a network (outdated and insecure).
   - **Switches**: Forward data only to the intended device (more secure).

3. **Collision Domains**:
   - A network segment where data collisions can occur (e.g., in hubs).
   - Switches reduce collisions by creating separate collision domains for each port.

4. **Physical Vulnerabilities**:
   - Unsecured network ports or cables can be tapped or accessed physically.

### Pentesting Relevance
- Perform **physical attacks** (e.g., cable tapping, unauthorized access to network hardware).
- Example: Plugging into an unsecured switch port to intercept traffic.

---

## Module 5: Number Systems

### Key Concepts in Detail
1. **Number Systems**:
   - **Binary**: Base-2 (0, 1). Used in computing and networking.
   - **Decimal**: Base-10 (0-9). Commonly used by humans.
   - **Hexadecimal**: Base-16 (0-9, A-F). Used for compact representation of binary data.

2. **IP Addressing**:
   - IPv4 addresses are 32-bit numbers represented in decimal (e.g., `192.168.1.1`).
   - Subnet masks define the network and host portions of an IP address.

3. **Subnetting**:
   - Dividing a network into smaller subnets for efficient IP address allocation.
   - Example: `192.168.1.0/24` means 256 IP addresses in the subnet.

### Pentesting Relevance
- **Subnetting** helps in network mapping and identifying target IP ranges.
- Example: Calculating subnets to find live hosts during reconnaissance.

---

## Summary
- **Networking Today**: Understand how devices communicate and identify attack surfaces.
- **Basic Configuration**: Test for weak configurations and default credentials.
- **Protocols and Models**: Exploit protocol weaknesses to manipulate traffic.
- **Physical Layer**: Perform physical attacks to gain access.
- **Number Systems**: Use subnetting to map networks and identify targets.

---
