# IP and MAC Addresses 🏡

## 1. IP Addresses
- **Definition**: Unique identifier assigned to each device on a network.  
- **Purpose**: Allows devices to locate and communicate with each other.  

### IPv4
- 32-bit address, written in **decimal format**.  
- Example: `192.168.0.5`  
- 4 groups of numbers (0–255) separated by dots.  
- ~4.3 billion unique addresses.  
- Becoming scarce due to internet growth.  

### IPv6
- 128-bit address, written in **hexadecimal format**.  
- Example: `2001:0db8:85a3:0000:0000:8a2e:0370:7334`  
- ~340 undecillion unique addresses.  
- Benefits:
  - Vastly larger address pool.
  - Simplified address assignment.
  - Improved security features.  

#### Importance
- Devices need IPs to **identify and communicate** with each other.  
- Without IP addresses, data wouldn’t know where to go.  

---

## 2. MAC Addresses
- **Definition**: *Media Access Control* address – a unique identifier assigned to a network interface.  
- **Analogy**: Like a **fingerprint** for your device.  
- Every device on a network has its own MAC address.  

#### Format
- 48-bit address, usually written in **hexadecimal**.  
- Example: `00:18:2B:...`  
- Uses digits `0–9` and letters `A–F`.  

#### Role
- Operates at the **Data Link Layer** of the OSI model.  
- Handles **node-to-node transfer** within the local network (LAN).  
- Ensures:
  - Your laptop connects to *your* router, not the neighbor’s.
  - Devices can properly communicate on the LAN.  

#### Importance
- Critical for **local network communication** and **security**.  
- Helps manage/control access and ensures packets reach the right device.  

---

### Summary
- **IP Address** = Device identity across networks (global communication).  
- **MAC Address** = Device identity within the local network (local communication).  
- Together, they ensure reliable and secure data transfer.
