# PPP

---

## **1. Foundations: Serial Communication**

### **Q1. What is serial communication and why is it fundamental to WANs?**

Serial communication sends bits one after another over a single channel.

It is fundamental because it:

- Works over long distances
- Uses less wiring
- Reduces interference (crosstalk)

---

### **Q2. Why is serial communication preferred over parallel in WANs?**

- Cheaper cabling
- Easier synchronization
- Supports long distances
- Less signal interference

---

### **Q3. What is parallel communication and why is it not used in WANs?**

Parallel communication sends multiple bits at the same time using multiple wires.

It is not used because:

- Signals desynchronize over long distances
- Only suitable for short distances

---

## **2. Serial Communication Standards**

### **Q4. Common serial communication standards**

- RS-232 → PC to modem
- V.35 → Router to CSU/DSU
- HSSI → High-speed WAN connections

---

### **Q5. What is RS-232 used for?**

Connecting computers to modems.

---

### **Q6. What is V.35 used for?**

Connecting routers to CSU/DSU in WAN links.

---

### **Q7. What is HSSI?**

A high-speed serial interface used for high bandwidth WAN connections.

---

## **3. Multiplexing**

### **Q8. What is TDM (Time Division Multiplexing)?**

A technique that:

- Shares one physical link among multiple data streams
- Assigns each stream a time slot

---

### **Q9. Why is TDM important in WANs?**

- Maximizes bandwidth usage
- Allows multiple users to share a single link efficiently

---

## **4. WAN Physical Structure**

### **Q10. What is the demarcation point?**

The boundary between:

- Customer network
- Service provider network

---

### **Q11. Difference between DTE and DCE**

- DTE → customer device (router)
- DCE → provider device (provides clocking)

---

### **Q12. Which device provides clocking?**

DCE device.

---

## **5. WAN Encapsulation**

### **Q13. What is WAN encapsulation?**

Wrapping data with headers/trailers for WAN transmission.

---

### **Q14. Main WAN encapsulation protocols**

- HDLC
- PPP

---

## **6. HDLC (Baseline Before PPP)**

### **Q15. What is HDLC?**

A Layer 2 protocol:

- Default on Cisco serial interfaces

---

### **Q16. HDLC frame types**

- Information (I-frame) → data
- Supervisory (S-frame) → control
- Unnumbered (U-frame) → management

---

### **Q17. Limitation of HDLC**

- No authentication support
- Cisco HDLC is vendor-specific

---

## **7. Introduction to PPP**

### **Q18. What is PPP?**

Point-to-Point Protocol:

- Layer 2 WAN protocol
- Supports multiple protocols
- Provides authentication and link control

---

### **Q19. Why is PPP preferred over HDLC?**

Because it supports:

- Authentication (PAP, CHAP)
- Multiple protocols
- Link quality monitoring

---

## **8. PPP Key Features**

### **Q20. What is PPP link quality management?**

PPP monitors:

- Error rate
- Link performance

If errors exceed limits:

- The link is dropped

---

### **Q21. PPP authentication methods**

- PAP
- CHAP

---

## **9. PPP Architecture**

### **Q22. Main components of PPP**

- LCP (Link Control Protocol)
- NCP (Network Control Protocol)

---

### **Q23. What is LCP?**

LCP:

- Establishes the link
- Negotiates parameters
- Tests link quality

---

### **Q24. What is NCP?**

NCP:

- Configures Layer 3 protocols (e.g., IP)
- Activates communication after LCP

---

## **10. PPP Frame Structure**

### **Q25. PPP frame fields**

- Flag → start/end
- Address → broadcast
- Control → frame type
- Protocol → payload type
- Data → actual data
- FCS → error detection

---

### **Q26. Role of Protocol field**

Identifies Layer 3 protocol (IPv4, IPv6, etc.).

---

## **11. PPP Session Phases**

### **Q27. 4 phases of PPP**

- Link establishment (LCP)
- Link quality determination
- Network configuration (NCP)
- Link termination

---

### **Q28. Link Establishment (LCP)**

Negotiates:

- Authentication method
- Compression
- Link parameters

---

### **Q29. Link Quality Determination**

Checks:

- Error rate
- Stability

---

### **Q30. NCP phase**

Configures network protocols (e.g., IP).

---

### **Q31. Can NCP handle multiple protocols?**

Yes, each protocol has its own NCP.

---

## **12. PPP Configuration**

### **Q32. Where is PPP configured?**

On router serial interfaces.

---

### **Q33. How are options exchanged in PPP?**

Through LCP frames.

---

## **13. PPP Verification & Troubleshooting**

### **Q34. show interfaces serial displays**

- Interface status
- LCP state
- NCP state
- Encapsulation type

---

### **Q35. Purpose of debug ppp**

Shows real-time PPP operations.

---

### **Q36. debug ppp authentication shows**

- PAP/CHAP process
- Success/failure messages

---

## **14. PPP Authentication**

### **Q37. What is PAP?**

- 2-way handshake
- Sends credentials in plain text

---

### **Q38. What is CHAP?**

- 3-way handshake
- Uses challenge-response hashing

---

### **Q39. Why is CHAP more secure?**

- Password is never transmitted directly
- Uses encrypted challenge-response

---

### **Q40. When is authentication performed?**

During LCP phase.

---

## **15. PAP vs CHAP**

| Feature           | PAP        | CHAP   |
| ----------------- | ---------- | ------ |
| Security          | Low        | High   |
| Handshake         | 2-way      | 3-way  |
| Password          | Plain text | Hashed |
| Re-authentication | No         | Yes    |

---

## **16. PPP Troubleshooting**

### **Q42. Common PPP issues**

- Encapsulation mismatch
- Authentication failure
- Physical link failure
- LCP not forming

---

### **Q43. Troubleshooting order**

1. Physical layer
2. Encapsulation check
3. LCP status
4. Authentication
5. NCP (IP config)

---

## **17. Big Picture**

### **Q44. Role of PPP in WANs**

PPP provides:

- Reliable serial communication
- Authentication
- Multi-protocol support

---

### **Q45. PPP vs modern WANs**

- PPP → serial / DSL (PPPoE)
- Modern WANs → Ethernet, MPLS, VPN

---

## **18. Exam-Level Insight**

### **Q46. Most tested PPP concepts**

- PPP phases order
- LCP vs NCP roles
- PAP vs CHAP
- Frame structure

---

### **Q47. Common trick question**

- LCP failure → no communication
- NCP failure → link exists but no IP connectivity

---

### **Q48. What if authentication fails?**

- Link is terminated
- No data transmission

---

## **Final Mental Model**

### **Q49. PPP process summary**

1. Physical link up
2. LCP negotiation
3. Authentication (PAP/CHAP)
4. NCP configuration
5. Data transmission
