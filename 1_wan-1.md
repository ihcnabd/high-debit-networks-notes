# WAN — Part 1 

---

## **1. Basic Definitions**

### **Q1. What is a WAN (Wide Area Network)?**

A WAN (Wide Area Network) is a telecommunications network that spans a large geographical area and is used to connect multiple LANs (Local Area Networks) across long distances.

### **Q2. What is a LAN (Local Area Network)?**

A LAN is a network that operates within a small geographic area, such as a home, school, or office, and connects local devices like computers, printers, and servers.

### **Q3. What is the main difference between a LAN and a WAN?**

- LAN → small area, high speed, privately owned
- WAN → large area, connects multiple LANs, managed by service providers

### **Q4. Who owns and manages LANs vs WANs?**

- LANs → owned and managed by individuals or organizations
- WANs → owned and managed by ISPs, telecom, cable, or satellite companies

### **Q5. Is there a cost difference between LAN and WAN usage?**

- LAN → no usage fee (only infrastructure cost)
- WAN → usage requires paid services

### **Q6. How do LAN and WAN differ in bandwidth?**

- LAN → typically high bandwidth (Ethernet, Wi-Fi)
- WAN → varies depending on provider and distance

---

## **2. Purpose of WANs**

### **Q7. Why do we need WANs?**

WANs are used to:

- Connect remote users
- Link different networks/sites
- Enable communication across cities, countries, or globally

### **Q8. What kind of devices/networks do WANs connect?**

- LANs
- Remote offices (branches)
- Data centers
- Remote users

---

## **3. Private vs Public WANs**

### **Q9. What is a private WAN?**

A private WAN is a dedicated network connection used by a single organization.

### **Q10. What are the advantages of a private WAN?**

- Guaranteed service level
- Consistent bandwidth
- High security

### **Q11. What is a public WAN?**

A public WAN uses shared infrastructure, typically the internet, provided by an ISP.

### **Q12. What are the disadvantages of a public WAN?**

- Variable performance
- No guaranteed bandwidth
- Lower security

### **Q13. When would a company prefer private WAN over public WAN?**

When it needs:

- High security
- Stable performance
- Guaranteed service (SLA)

---

## **4. WAN Topologies (Overview)**

### **Q14. What is a WAN topology?**

A WAN topology defines the logical layout of how sites and networks are connected.

### **Q15. What are the main WAN topologies?**

- Point-to-Point
- Hub-and-Spoke
- Dual-homed
- Fully Mesh
- Partially Mesh

### **Q16. Do real networks use only one topology?**

No. Large networks usually combine multiple topologies.

---

## **5. WAN Topologies (Detailed)**

### **Q17. What is a Point-to-Point topology?**

A topology where two endpoints are directly connected by a dedicated link.

### **Q18. What are the characteristics of Point-to-Point?**

- Uses a direct circuit
- Works at Layer 2
- Transparent to the user network

### **Q19. What is a disadvantage of Point-to-Point topology?**

It becomes very expensive when many connections are required.

---

### **Q20. What is Hub-and-Spoke topology?**

One central device (hub) connects to multiple sites (spokes).

### **Q21. How does communication work in Hub-and-Spoke?**

Spokes cannot communicate directly; all traffic passes through the hub.

### **Q22. What is a major weakness of Hub-and-Spoke?**

The hub is a single point of failure.

---

### **Q23. What is Dual-homed topology?**

A network connected to multiple networks or providers for redundancy.

### **Q24. Advantages of Dual-homed topology**

- Redundancy
- Load balancing
- Better reliability
- Backup connections

### **Q25. Disadvantages of Dual-homed topology**

- More expensive
- More complex to configure

---

### **Q26. What is a Fully Meshed topology?**

Every site is connected to every other site.

### **Q27. Main advantage of Fully Meshed topology**

Maximum fault tolerance.

---

### **Q28. What is a Partially Meshed topology?**

Some sites are directly connected, others are not fully interconnected.

### **Q29. Why use Partial Mesh instead of Full Mesh?**

To reduce cost and complexity while keeping some redundancy.

---

## **6. Carrier Connections & SLA**

### **Q30. What is an SLA (Service Level Agreement)?**

A contract defining reliability, availability, and performance expectations.

### **Q31. What is a carrier?**

A company that owns and maintains network infrastructure and provides connectivity services.

### **Q32. Is a service provider always the carrier?**

No. A service provider may use another carrier’s infrastructure.

### **Q33. What is a single-carrier connection?**

Using only one service provider.

### **Q34. Drawbacks of single-carrier**

- No redundancy
- Higher risk of downtime

### **Q35. What is a dual-carrier connection?**

Using two different service providers.

### **Q36. Advantages of dual-carrier**

- Higher availability
- Redundancy
- Better reliability

---

## **7. Evolving Networks**

### **Q37. Why do networks evolve over time?**

- Company growth
- Increased user demand
- New services and locations

### **Q38. What must a network support as a company grows?**

- Daily operations
- Scalability
- New technologies

### **Q39. What do network designers consider?**

- Technologies
- Protocols
- Service providers
- Architecture

---

## **8. Network Evolution Stages (SPAN Example)**

### **Q40. What characterizes a small network?**

- Single LAN
- Wireless router
- DSL internet
- External IT support

### **Q41. What is DSL?**

DSL (Digital Subscriber Line) is broadband internet using telephone lines.

---

### **Q42. What is a Campus Area Network (CAN)?**

A network connecting multiple LANs within a limited area like a campus or building.

### **Q43. What characterizes a campus network?**

- Multiple buildings/floors
- Internal IT staff
- Firewall protection

---

### **Q44. What is a Metropolitan Area Network (MAN)?**

A network connecting sites within a city.

---

### **Q45. What characterizes a branch network?**

- Multiple locations
- Dedicated inter-site links
- Regional connectivity

---

### **Q46. What is a distributed network?**

A large-scale network with global presence and many users/locations.

---

### **Q47. What is a VPN?**

A VPN is a secure encrypted connection over the internet for remote users or sites.

---

## **9. WAN Standards**

### **Q48. Why are WAN standards important?**

- Compatibility
- Interoperability
- Consistent design

### **Q49. What organizations define WAN standards?**

- TIA/EIA
- ISO
- IEEE

### **Q50. What does ISO stand for?**

International Organization for Standardization

### **Q51. What does IEEE stand for?**

Institute of Electrical and Electronics Engineers

### **Q52. What does TIA/EIA stand for?**

Telecommunications Industry Association / Electronic Industries Alliance
