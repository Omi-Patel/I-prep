# Computer Networks (CN): Interview Preparation Guide

## Table of Contents
1. [Introduction to Computer Networks](#introduction-to-computer-networks)
2. [Important Networking Concepts](#important-networking-concepts)
3. [Network Devices](#network-devices)
4. [Network Topologies](#network-topologies)
5. [Data Link Layer and MAC Addressing](#data-link-layer-and-mac-addressing)
6. [Transport Layer Protocols](#transport-layer-protocols)
7. [Application Layer Protocols](#application-layer-protocols)
8. [Security in Networking](#security-in-networking)
9. [Common Interview Questions and Answers](#common-interview-questions-and-answers)

---

## 1. Introduction to Computer Networks

### Definition
A computer network is a system of interconnected devices (nodes) that can share data and resources. It enables communication between computers and other devices.

### Types of Networks
- **LAN (Local Area Network)**: Covers a small geographic area like a building.
- **WAN (Wide Area Network)**: Covers a large geographic area, such as a country or continent.
- **MAN (Metropolitan Area Network)**: Covers a city or a large campus.
- **PAN (Personal Area Network)**: A small network for personal devices.

### Network Models
- **OSI Model (Open Systems Interconnection)**: Conceptual framework for understanding network communication divided into 7 layers (Physical, Data Link, Network, Transport, Session, Presentation, Application).
- **TCP/IP Model**: A practical framework consisting of 4 layers (Network Interface, Internet, Transport, Application).

---

## 2. Important Networking Concepts

### Protocols
Rules that govern data communication. Common protocols include:
- **HTTP/HTTPS**: Web communication.
- **TCP/IP**: Transmission Control Protocol/Internet Protocol.
- **FTP**: File Transfer Protocol.
- **SMTP**: Email transfer protocol.

### IP Addressing
- **IPv4**: 32-bit address space (e.g., 192.168.1.1).
- **IPv6**: 128-bit address space (e.g., 2001:0db8::85a3).

### Subnetting
Divides a network into smaller sub-networks, improving performance and security.

### DNS (Domain Name System)
Translates domain names (like www.example.com) into IP addresses.

### TCP vs UDP
- **TCP (Transmission Control Protocol)**: Reliable, connection-oriented.
- **UDP (User Datagram Protocol)**: Faster, connectionless, less reliable.

### Ports and Sockets
- **Port**: A virtual point where network connections start and end (e.g., HTTP uses port 80).
- **Socket**: Combination of IP address and port number.

---

## 3. Network Devices

- **Router**: Routes data between networks.
- **Switch**: Connects devices in a network and uses MAC addresses to forward data.
- **Hub**: Broadcasts data to all devices.
- **Firewall**: Protects the network by controlling incoming and outgoing traffic.

---

## 4. Network Topologies

- **Bus Topology**: All devices connected to a single communication line.
- **Star Topology**: Devices connected to a central hub.
- **Ring Topology**: Devices connected in a circular loop.
- **Mesh Topology**: Devices are interconnected, providing redundancy.

---

## 5. Data Link Layer and MAC Addressing

### Ethernet
A common LAN technology used for data transmission.

### MAC Address
A 48-bit hardware address unique to each network device (e.g., 00:1B:44:11:3A:B7).

### ARP (Address Resolution Protocol)
Used to map an IP address to a MAC address within a local network.

---

## 6. Transport Layer Protocols

### TCP (Transmission Control Protocol)
- **Three-Way Handshake**: SYN, SYN-ACK, ACK to establish a connection.
- **Flow Control**: Manages the rate of data transmission.
- **Congestion Control**: Prevents network congestion by adjusting the rate.

### Error Detection
- **Checksum**: Verifies data integrity.
- **Parity Bit**: Adds an extra bit to check for errors.

---

## 7. Application Layer Protocols

- **HTTP/HTTPS**: Used for web communication.
- **FTP (File Transfer Protocol)**: Used to transfer files between systems.
- **SMTP (Simple Mail Transfer Protocol)**: Used for sending emails.
- **SNMP (Simple Network Management Protocol)**: Used for managing devices on IP networks.

---

## 8. Security in Networking

### Cryptography
- **Symmetric Encryption**: Same key is used to encrypt and decrypt data.
- **Asymmetric Encryption**: Public and private keys are used for encryption and decryption.

### VPN (Virtual Private Network)
Provides secure communication over a public network.

### Common Network Attacks
- **DDoS (Distributed Denial of Service)**: Overwhelms a network with traffic.
- **Phishing**: Fraudulent attempt to obtain sensitive information.
- **Man-in-the-Middle Attack**: Attacker intercepts communication between two parties.

---

## 9. Common Interview Questions and Answers

### 1. What is the OSI Model?
The OSI (Open Systems Interconnection) model is a conceptual framework used to understand and implement network protocols. It has seven layers:
   1. Physical
   2. Data Link
   3. Network
   4. Transport
   5. Session
   6. Presentation
   7. Application

### 2. Difference between TCP and UDP?
- **TCP**: Connection-oriented, reliable, ensures data delivery (e.g., HTTP, FTP).
- **UDP**: Connectionless, faster but less reliable (e.g., DNS, VoIP).

### 3. What is Subnetting?
Subnetting is the process of dividing a large network into smaller, more manageable sub-networks (subnets) to optimize IP address usage and improve security.

### 4. Explain DNS and how it works.
DNS (Domain Name System) is a hierarchical system that translates human-readable domain names (like www.example.com) into IP addresses used by computers to identify each other on the network.

### 5. How does NAT work?
NAT (Network Address Translation) allows multiple devices on a private network to access the public Internet using a single public IP address by translating private IPs into public ones.

### 6. What is a Firewall? Different types of Firewalls?
A firewall is a security system that monitors and controls incoming and outgoing network traffic based on predetermined security rules. Types include:
   - **Packet Filtering Firewall**
   - **Stateful Inspection Firewall**
   - **Proxy Firewall**

### 7. How does HTTP work?
HTTP (Hypertext Transfer Protocol) is an application layer protocol for transferring hypermedia documents, such as HTML. It follows a request-response model where clients (browsers) send requests and servers respond.

### 8. Difference between IPv4 and IPv6?
- **IPv4**: 32-bit address space (~4.3 billion addresses).
- **IPv6**: 128-bit address space (virtually unlimited number of addresses).

### 9. What is ARP and how does it work?
ARP (Address Resolution Protocol) is used to map a 32-bit IP address to a 48-bit MAC address in a local area network, allowing communication between devices.

### 10. What is the TCP 3-Way Handshake?
The TCP three-way handshake is the process used to establish a reliable connection:
   1. **SYN**: Client sends a synchronize request.
   2. **SYN-ACK**: Server acknowledges and responds.
   3. **ACK**: Client sends an acknowledgment, and the connection is established.

---

This guide is a comprehensive preparation tool for understanding the basics of computer networks and preparing for technical interviews.
