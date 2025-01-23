---
date: 2024-12-01
tags: 
      - CCNA
      - Network
      - Cybersecurity
---
# Layers Attack 
## Module 11: IPv4 Addressing
### Key Concepts in Detail
#### 1. **IPv4 Address Structure**:
   - 32-bit addresses divided into network and host portions.
   - Subnet masks define the network size (e.g., `/24` for 256 addresses).

#### 2. **Private vs. Public IPs**:
   - Private IPs (e.g., `192.168.x.x`) are used internally.
   - Public IPs are routable on the internet.

#### 3. **Subnetting**:
   - Dividing a network into smaller subnets for efficient IP allocation.
   - Helps attackers map networks and identify targets.

### Pentesting Relevance
- Use subnetting to identify live hosts and target ranges.
- Example: Use tools like `Nmap` to scan subnets for active devices.

---

## Module 12: IPv6 Addressing

### Key Concepts in Detail
#### 1. **IPv6 Address Structure**:
   - 128-bit addresses represented in hexadecimal (e.g., `2001:0db8::1`).
   - Provides a much larger address space than IPv4.

#### 2. **Address Types**:
   - **Unicast**: One-to-one communication.
   - **Multicast**: One-to-many communication.
   - **Anycast**: One-to-nearest communication.

#### 3. **IPv6 Security**:
   - IPv6 introduces new vulnerabilities (e.g., misconfigured neighbor discovery).

### Pentesting Relevance
- Test for IPv6 misconfigurations and vulnerabilities.
- Example: Use tools like `THC-IPv6` to exploit IPv6 weaknesses.

---

## Module 13: ICMP

### Key Concepts in Detail
#### 1. **ICMP Messages**:
   - Used for network diagnostics (e.g., `ping`, `traceroute`).
   - Includes error reporting and control messages.

#### 2. **ICMP Vulnerabilities**:
   - **Ping Flood**: Overwhelm a target with ICMP echo requests.
   - **Smurf Attack**: Use ICMP to amplify traffic and flood a target.

### Pentesting Relevance
- Use ICMP for network discovery and reconnaissance.
- Example: Use `hping3` to perform ICMP-based attacks.

---

## Module 14: Transport Layer

### Key Concepts in Detail
#### 1. **TCP (Transmission Control Protocol)**:
   - Reliable, connection-oriented protocol.
   - Vulnerable to **SYN floods** and **session hijacking**.

#### 2. **UDP (User Datagram Protocol)**:
   - Unreliable, connectionless protocol.
   - Vulnerable to **UDP amplification attacks**.

#### 3. **Ports**:
   - Identify services running on a device (e.g., port 80 for HTTP).
   - Open ports can be exploited if not secured.

### Pentesting Relevance
- Exploit TCP/UDP vulnerabilities (e.g., SYN floods, UDP amplification).
- Example: Use tools like `Metasploit` to exploit open ports.

---

## Module 15: Application Layer

### Key Concepts in Detail
#### 1. **HTTP/HTTPS**:
   - Web communication protocols.
   - Vulnerable to **SQL injection**, **XSS**, and **CSRF**.

#### 2. **DNS (Domain Name System)**:
   - Resolves domain names to IP addresses.
   - Vulnerable to **DNS spoofing** and **cache poisoning**.

#### 3. **FTP (File Transfer Protocol)**:
   - Used for file transfers.
   - Vulnerable to **anonymous login** and **data interception**.

### Pentesting Relevance
- Exploit application-layer protocols (e.g., DNS poisoning, FTP exploits).
- Example: Use tools like `Burp Suite` to test web application vulnerabilities.

---

## Summary
- **IPv4/IPv6 Addressing**: Map networks and identify targets.
- **ICMP**: Use for network discovery and reconnaissance.
- **Transport Layer**: Exploit TCP/UDP vulnerabilities.
- **Application Layer**: Test for web and DNS vulnerabilities.

---