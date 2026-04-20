# Acronyms

---

# 1. General Networking & OSI

### LAN — Local Area Network

A network covering a small area (home, office, campus) used to connect local devices.

### WAN — Wide Area Network

A network that connects multiple LANs over large geographical distances using service providers.

### OSI — Open Systems Interconnection Model

A 7-layer reference model that standardizes how data is transmitted over networks.

---

# 2. WAN Infrastructure Terms

### DTE — Data Terminal Equipment

Customer-side devices (like routers or computers) that send/receive data to/from the WAN.

### DCE — Data Communications Equipment

Provider-side equipment that supplies clocking and connects the DTE to the WAN.

### CPE — Customer Premises Equipment

All equipment located at the customer site (DTE + DCE).

### POP — Point of Presence

A physical access point where customers connect to the service provider network.

### CO — Central Office

Service provider facility that connects local users to the provider backbone network.

### LMI — Local Management Interface

A protocol used in Frame Relay to monitor PVC status and link health.

### PVC — Permanent Virtual Circuit

A logical, always-on connection between two endpoints in Frame Relay.

### VC — Virtual Circuit

A logical connection used in packet-switched networks like Frame Relay or MPLS.

### DLCI — Data-Link Connection Identifier

A local identifier used in Frame Relay to distinguish virtual circuits.

---

# 3. WAN Protocols & Technologies

### PPP — Point-to-Point Protocol

A Layer 2 protocol used to establish direct WAN links with authentication and multi-protocol support.

### HDLC — High-Level Data Link Control

A Cisco default Layer 2 WAN encapsulation protocol for serial links.

### MPLS — Multiprotocol Label Switching

A high-performance WAN technology that routes traffic using labels instead of IP addresses.

### ATM — Asynchronous Transfer Mode

A legacy WAN technology using fixed-size 53-byte cells for data transmission.

### FR — Frame Relay

A Layer 2 WAN technology that uses virtual circuits to transmit data over shared networks.

---

# 4. PPP Components

### LCP — Link Control Protocol

Part of PPP responsible for establishing, configuring, and testing the data link.

### NCP — Network Control Protocol

Part of PPP that configures network layer protocols (like IP) after link setup.

### PAP — Password Authentication Protocol

A simple PPP authentication method using plain-text credentials (less secure).

### CHAP — Challenge Handshake Authentication Protocol

A secure PPP authentication method using encrypted challenge-response mechanism.

---

# 5. WAN Communication & Switching

### PSTN — Public Switched Telephone Network

Traditional telephone network used for dial-up WAN connections.

### ISDN — Integrated Services Digital Network

Digital circuit-switched WAN technology offering higher speeds than PSTN.

### DSL — Digital Subscriber Line

A broadband technology using telephone lines for internet access.

### ADSL — Asymmetric DSL

DSL type with higher download speed than upload speed.

### SDSL — Symmetric DSL

DSL type with equal upload and download speeds.

### DOCSIS — Data Over Cable Service Interface Specification

Standard used for transmitting internet over cable networks.

### CMTS — Cable Modem Termination System

Provider-side system that manages cable modem connections.

---

# 6. Modern WAN & Internet Technologies

### ISP — Internet Service Provider

Company that provides internet and WAN connectivity services.

### VPN — Virtual Private Network

Encrypted tunnel over the internet used for secure communication between networks.

### MPLS — Multiprotocol Label Switching

(Repeated for importance) Label-based routing system used in modern WANs.

### FTTH — Fiber To The Home

Fiber-optic connection directly to a residential location.

### FTTB — Fiber To The Building

Fiber connection to a building, with internal wiring distributing access.

### FTTN — Fiber To The Node

Fiber connection to a neighborhood node, then copper/fiber to users.

---

# 7. Traffic Control & Congestion (Frame Relay)

### FECN — Forward Explicit Congestion Notification

Signal sent to the receiver indicating congestion in the forward direction.

### BECN — Backward Explicit Congestion Notification

Signal sent to the sender indicating congestion, requesting slowdown.

### DE — Discard Eligible

Bit used to mark low-priority traffic that can be dropped during congestion.

---

# 8. Networking Standards & Organizations

### IEEE — Institute of Electrical and Electronics Engineers

Organization that defines networking standards like Ethernet and Wi-Fi.

### ISO — International Organization for Standardization

Defines global standards including the OSI model.

### TIA/EIA — Telecommunications Industry Association / Electronic Industries Alliance

Defines standards for telecommunications and cabling.

---

# 9. Optical Networking

### SDH — Synchronous Digital Hierarchy

Global standard for high-speed fiber-optic communication.

### SONET — Synchronous Optical Networking

North American version of SDH used for optical data transport.

### DWDM — Dense Wavelength Division Multiplexing

Technology that increases fiber capacity by sending multiple light wavelengths simultaneously.

---

# 10. WAN Topologies (Not Acronyms but Key Terms)

### NBMA — Non-Broadcast Multi-Access

Network type (like Frame Relay) where broadcast is not supported naturally.
