# WAN — Part 2 

---

## **1. WANs in the OSI Model**

### **Q1. Which OSI layers are most relevant to WAN technologies?**

- Layer 1 (Physical Layer)
- Layer 2 (Data Link Layer)

---

### **Q2. Why do WAN standards focus mostly on Layer 1 and Layer 2?**

Because WANs deal with:

- Physical transmission of data (cables, fiber, signals)
- Data framing and link-level communication over long distances

---

### **Q3. What is the role of Layer 1 in WANs?**

Layer 1 defines:

- Physical media (fiber, copper)
- Signal transmission (electrical, optical)
- Bit-level communication

---

### **Q4. What is the role of Layer 2 in WANs?**

Layer 2 handles:

- Data framing
- Error detection
- Logical link communication between nodes

---

## **2. Layer 1 WAN Protocols**

### **Q5. What are the main Layer 1 WAN technologies?**

- SDH (Synchronous Digital Hierarchy)
- SONET (Synchronous Optical Networking)
- DWDM (Dense Wavelength Division Multiplexing)

---

### **Q6. What is SDH?**

A global standard for transmitting data over fiber-optic networks.

---

### **Q7. What is SONET?**

A North American standard similar to SDH for high-speed optical communication.

---

### **Q8. What is DWDM?**

A technology that:

- Sends multiple data streams simultaneously
- Uses different wavelengths of light
- Greatly increases fiber capacity

---

### **Q9. Why is fiber-optic preferred over copper in WANs?**

- Lower signal loss
- Less interference
- Higher bandwidth
- Better long-distance performance

---

## **3. Layer 2 WAN Protocols**

### **Q10. What are common Layer 2 WAN technologies?**

- DSL & Cable
- Wireless WAN
- Metro Ethernet
- MPLS
- PPP
- HDLC
- Frame Relay (legacy)
- ATM (legacy)

---

### **Q11. Which Layer 2 technologies are considered legacy?**

- Frame Relay
- ATM

---

### **Q12. Which Layer 2 protocols are less used today?**

- PPP
- HDLC

---

### **Q13. What is MPLS (basic idea)?**

A high-performance WAN technology that:

- Uses labels instead of IP addresses
- Improves speed and traffic handling efficiency

---

## **4. WAN Terminology (Core Concepts)**

### **Q14. What is DTE (Data Terminal Equipment)?**

A device (like a router) that connects a customer network to a WAN.

---

### **Q15. What is DCE (Data Communications Equipment)?**

A provider-side device that:

- Connects to the WAN
- Provides clocking and signal control

---

### **Q16. What is CPE (Customer Premises Equipment)?**

All networking equipment at the customer site, including:

- DTE
- DCE

---

### **Q17. What is a POP (Point of Presence)?**

A location where customers connect to a service provider’s network.

---

### **Q18. What is the Demarcation Point?**

The boundary separating:

- Customer equipment
- Service provider equipment

---

## **5. WAN Infrastructure Components**

### **Q19. What is the Local Loop (Last Mile)?**

The physical link between:

- Customer premises
- Service provider central office

---

### **Q20. What is the Central Office (CO)?**

A provider facility where:

- Customer connections are aggregated
- Network access begins

---

### **Q21. What is the Toll Network?**

The provider’s core infrastructure:

- Long-distance fiber
- High-capacity routers and switches

---

### **Q22. What is a Backhaul Network?**

A network that connects access points (towers/nodes) to the core network.

---

### **Q23. What is a Backbone Network?**

A high-capacity core network that:

- Connects major regions
- Ensures redundancy and fast communication

---

## **6. Serial vs Parallel Communication**

### **Q24. What is serial communication?**

Data transmitted:

- One bit at a time
- Over a single channel

---

### **Q25. What is parallel communication?**

Data transmitted:

- Multiple bits at once
- Using multiple wires

---

### **Q26. Why is serial communication used in WANs?**

Because it:

- Works better over long distances
- Avoids synchronization issues

---

### **Q27. Why is parallel communication limited?**

Because:

- Signals become unsynchronized over long distances
- Only suitable for short distances

---

## **7. Circuit-Switched Communication**

### **Q28. What is circuit switching?**

A method where:

- A dedicated path is established before transmission

---

### **Q29. Key characteristics of circuit switching**

- Dedicated connection
- Fixed path
- Reserved bandwidth

---

### **Q30. Examples of circuit-switched technologies**

- PSTN
- ISDN

---

### **Q31. Major disadvantage of circuit switching**

Inefficient resource usage (path stays reserved even when idle).

---

## **8. Packet-Switched Communication**

### **Q32. What is packet switching?**

Data is:

- Split into packets
- Sent independently across the network

---

### **Q33. Advantages of packet switching**

- Lower cost
- Flexible
- Efficient bandwidth usage

---

### **Q34. Common packet-switched technologies**

- MPLS
- Metro Ethernet
- Frame Relay
- ATM

---

### **Q35. Why is packet switching widely used today?**

Because it:

- Scales efficiently
- Supports many users
- Reduces cost

---

## **9. Optical WAN Technologies**

### **Q36. How do SDH and SONET work?**

They:

- Use optical signals (laser/LED)
- Transmit voice, video, and data
- Provide reliable long-distance communication

---

### **Q37. What problem does DWDM solve?**

It increases fiber capacity by:

- Sending multiple signals simultaneously
- Using different light wavelengths

---

## **10. Traditional WAN Connectivity**

### **Q38. How did WAN connectivity start historically?**

Using:

- Leased lines
- Switched services

---

### **Q39. What is a leased line?**

A dedicated always-on connection rented from a provider.

---

### **Q40. How is leased line pricing determined?**

Based on:

- Distance
- Bandwidth

---

## **11. T-Carrier and E-Carrier Systems**

### **Q41. What is T-carrier?**

North American standard:

- T1 → 1.544 Mbps
- T3 → 43.7 Mbps

---

### **Q42. What is E-carrier?**

European standard:

- E1 → 2.048 Mbps
- E3 → 34.368 Mbps

---

## **12. Leased Lines: Pros and Cons**

### **Q43. Advantages of leased lines**

- Simple
- High quality
- Always available
- Suitable for critical applications

---

### **Q44. Disadvantages of leased lines**

- Expensive
- Not flexible

---

## **13. Circuit-Switched WAN Options**

### **Q45. What is PSTN-based dial-up?**

A WAN connection using:

- Telephone lines
- Modems

---

### **Q46. Speed limitation of PSTN dial-up**

Less than 56 kbps

---

### **Q47. What is ISDN?**

A digital circuit-switched technology:

- Faster than dial-up
- 45 kbps to 2.048 Mbps

---

## **14. Packet-Switched WAN Options (Legacy)**

### **Q48. What is Frame Relay?**

A Layer 2 WAN technology using:

- Virtual circuits (PVCs)
- DLCI identifiers

---

### **Q49. What does DLCI represent?**

Data-Link Connection Identifier used to identify a virtual circuit.

---

### **Q50. What is ATM?**

A WAN technology using:

- Fixed-size cells (53 bytes)
- Supports voice, video, and data

---

### **Q51. Difference between ATM and Frame Relay**

- ATM → fixed-size cells
- Frame Relay → variable-size frames

---

### **Q52. Why are Frame Relay and ATM obsolete?**

Because they were replaced by:

- Faster technologies
- More flexible solutions (MPLS, Ethernet, internet-based WANs)
