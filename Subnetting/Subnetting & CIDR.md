# 🧩 Subnetting & CIDR – Introduction

---

## 🌐 What is Subnetting?
- **Subnetting** = Splitting one big network into **smaller subnetworks**.  
- ✅ Benefits:
  - Easier **network management** (smaller, organized groups).  
  - Better **efficiency** (traffic stays local, less congestion).  

**Analogy**:  
Imagine a large apartment building 🏢. Subnetting is like dividing it into **floors** or **sections** so each group of residents has their own mailbox area, making delivery easier 📬.

---

## 📏 CIDR (Classless Inter-Domain Routing)
- A method of **allocating IP addresses** and **routing IP packets**.  
- **Format**: `IP Address / Prefix Length`

👉 Example:  
`192.168.1.0/24`  

- **192.168.1.0** → Network address  
- **/24** → First 24 bits = **network part**  
- Remaining (32 - 24 = 8 bits) = **hosts**  

---

## 🧮 How / Prefix Works
- `/24` → Network: 24 bits | Host: 8 bits | Hosts available = **2⁸ – 2 = 254**  
- `/16` → Network: 16 bits | Host: 16 bits | Hosts = **65,534**  
- `/8`  → Network: 8 bits | Host: 24 bits | Hosts = **16,777,214**  

⚠️ Subtract 2 because:
- 1 address = **Network address**  
- 1 address = **Broadcast address**

---

## ✅ Quick Recap
- **Subnetting** = Dividing networks for efficiency & organization.  
- **CIDR Notation** = `IP / prefix` → defines how many bits belong to network vs host.  
- Smaller prefix (e.g., /30) = fewer hosts.  
- Larger prefix (e.g., /8) = more hosts.  


