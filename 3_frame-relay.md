# Frame Relay

---

## **1. Core Idea of Frame Relay**

### **Q1. What is Frame Relay?**

Frame Relay is a Layer 2 WAN technology used to:

- Connect multiple sites over a shared provider network
- Transmit data using virtual circuits

---

### **Q2. Why was Frame Relay widely used?**

Because it:

- Is cheaper than leased lines
- Uses fewer physical resources
- Scales well for multiple sites
- Supports efficient multi-site connectivity

---

### **Q3. Which OSI layer does Frame Relay operate on?**

Layer 2 (Data Link Layer)

---

## **2. Frame Relay Basic Concept**

### **Q4. Key idea behind Frame Relay**

Instead of physical links, Frame Relay uses:

- Virtual Circuits (VCs)

---

### **Q5. What is a Virtual Circuit (VC)?**

A logical connection between two devices that:

- Acts like a dedicated link
- Runs over a shared provider network

---

### **Q6. Advantages of virtual circuits**

- Lower cost
- Efficient bandwidth usage
- Scalable multi-site connectivity

---

## **3. Frame Relay Encapsulation**

### **Q7. What is Frame Relay encapsulation?**

Process of:

- Wrapping Layer 3 packets inside Frame Relay frames
- Using DLCI for addressing

---

### **Q8. What is inside a Frame Relay frame?**

- IP packet (data payload)
- DLCI (virtual circuit identifier)
- Control information
- FCS (error detection)

---

## **4. DLCI (Critical Exam Topic)**

### **Q9. What is DLCI?**

Data Link Connection Identifier:

- A number that identifies a virtual circuit

---

### **Q10. Role of DLCI**

It tells the provider network:

- Which path to use to reach the destination

---

### **Q11. Is DLCI global or local?**

DLCI is locally significant:

- Only meaningful between router and provider switch

---

## **5. Frame Relay Topologies**

### **Q12. Topologies used in Frame Relay**

- Hub-and-spoke
- Partial mesh
- Full mesh

---

### **Q13. Why is hub-and-spoke common?**

Because it:

- Reduces cost
- Simplifies design
- Uses a central hub for routing

---

### **Q14. Problem with hub-and-spoke**

- Hub becomes bottleneck
- Spokes cannot directly communicate

---

## **6. NBMA Concept**

### **Q15. What is Frame Relay considered as?**

NBMA (Non-Broadcast Multi-Access)

---

### **Q16. What does NBMA mean?**

- No broadcast capability
- Multiple destinations exist
- No automatic Ethernet-like broadcast behavior

---

## **7. LMI (Local Management Interface)**

### **Q17. What is LMI?**

Protocol between:

- Router (DTE)
- Frame Relay switch (provider)

---

### **Q18. What does LMI do?**

- Checks VC status
- Sends updates
- Maintains connectivity information

---

### **Q19. Why is LMI important?**

- Confirms PVC status
- Detects failures

---

## **8. Inverse ARP**

### **Q20. What is Inverse ARP?**

Mechanism that:

- Maps DLCI → IP address automatically

---

### **Q21. Why is Inverse ARP needed?**

Because:

- Frame Relay knows DLCI
- But routing requires IP mapping

---

### **Q22. What problem does it solve?**

Automatic DLCI-to-IP mapping

---

## **9. Static Frame Relay Mapping**

### **Q23. What is static mapping?**

Manual configuration of:

- IP address ↔ DLCI

---

### **Q24. When is static mapping used?**

- Inverse ARP disabled
- Troubleshooting complex networks

---

## **10. PVC (Permanent Virtual Circuit)**

### **Q25. What is a PVC?**

Permanent Virtual Circuit:

- Preconfigured logical path
- Always available

---

### **Q26. PVC vs SVC**

- PVC → permanent
- SVC → temporary (rare in modern networks)

---

## **11. Configuration Concepts**

### **Q27. What is required for Frame Relay configuration?**

- Enable Frame Relay encapsulation
- Configure DLCI
- Configure mapping (static or dynamic)

---

### **Q28. What is dynamic mapping?**

Uses Inverse ARP automatically.

---

### **Q29. What is static mapping used for?**

Manual binding of:

- IP addresses to DLCIs

---

## **12. Reachability Issues (Very Important)**

### **Q30. Major Frame Relay problem**

Split horizon limitation in hub-and-spoke setups.

---

### **Q31. What is split horizon?**

A rule that:

- Prevents routing updates from being sent back on the same interface

---

### **Q32. Why is split horizon a problem?**

Because:

- Multiple virtual circuits share one physical interface
- Spokes cannot learn routes from other spokes via hub

---

### **Q33. How is it solved?**

- Using subinterfaces
- Or disabling split horizon (less recommended)

---

## **13. Subinterfaces**

### **Q34. What is a subinterface?**

Logical division of a physical interface:

- Each acts as a separate interface

---

### **Q35. Why are subinterfaces used?**

- Solve split horizon issues
- Improve routing between sites

---

### **Q36. Types of subinterfaces**

- Point-to-point
- Multipoint

---

### **Q37. Why is point-to-point preferred?**

- Avoids NBMA complexity
- Eliminates split horizon issues

---

## **14. Bandwidth and Flow Control**

### **Q38. What is Frame Relay bandwidth control?**

Controls how much traffic a VC can use.

---

### **Q39. What is flow control?**

Manages congestion in the network.

---

## **15. Congestion Control Bits**

### **Q40. What are FECN and BECN?**

Congestion notification bits.

---

### **Q41. What is FECN?**

Forward Explicit Congestion Notification:

- Notifies receiver of congestion

---

### **Q42. What is BECN?**

Backward Explicit Congestion Notification:

- Notifies sender to slow down

---

### **Q43. What is DE bit?**

Discard Eligible bit:

- Marks low-priority traffic
- Can be dropped during congestion

---

## **16. Verification Commands**

### **Q44. Interface status**

show interfaces

---

### **Q45. LMI status**

show frame-relay lmi

---

### **Q46. PVC status**

show frame-relay pvc

---

### **Q47. DLCI mapping**

show frame-relay map

---

## **17. Troubleshooting**

### **Q48. Main troubleshooting command**

debug frame-relay lmi

---

### **Q49. Common Frame Relay issues**

- DLCI mismatch
- LMI failure
- Missing mapping
- Split horizon issues
- PVC down

---

## **18. Summary (High-Yield Core)**

### **Q50. Why was Frame Relay important?**

- Reduced cost vs leased lines
- Used virtual circuits instead of physical links
- Supported multi-site WANs

---

### **Q51. Key concepts to remember**

- DLCI → virtual circuit ID
- LMI → status monitoring
- Inverse ARP → automatic mapping
- NBMA → no broadcast support
- PVC → permanent connection
- Subinterfaces → fix routing issues

---

### **Q52. Why is Frame Relay obsolete today?**

Replaced by:

- MPLS
- Ethernet WAN
- Internet VPNs
