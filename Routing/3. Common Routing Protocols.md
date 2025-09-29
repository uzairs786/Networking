# 🌐 Common Routing Protocols

Routing protocols = the **rules/algorithms** routers use to **find the best path** for data.  
Instead of admins manually setting routes, these protocols do the **heavy lifting** 🤖.  

---

## 🔑 Why They Matter
- 📡 **Automate routing updates** → no need to manually change routes.  
- ⚡ **Improve efficiency** → choose the fastest, least congested paths.  
- 🔄 **Increase resilience** → find new paths if one link goes down.  

---

## 🚀 Two Common Routing Protocols

### 1️⃣ OSPF (Open Shortest Path First)
- **Used for**: Large organizations (inside a company’s network).  
- **How it works**: Finds the **shortest path** using "link state info" (status of network links).  
- **Key feature**: **Fast convergence** → quickly recalculates routes if something changes.  
- **Analogy**: Like a delivery driver using **real-time traffic updates** to always take the fastest road 🛣️.

---

### 2️⃣ BGP (Border Gateway Protocol)
- **Used for**: Between large networks (e.g., ISPs, cloud providers).  
- **How it works**: Uses **path vectors** → keeps track of entire paths across the internet.  
- **Key feature**: Lets admins set **policies** (e.g., prefer one route over another).  
- **Analogy**: Like airlines ✈️ deciding flight routes between countries → policies & agreements decide which path to take.

---

## ⚔️ OSPF vs BGP Quick Glance

| Feature             | 🛣️ OSPF                              | 🌍 BGP                               |
|---------------------|---------------------------------------|--------------------------------------|
| **Scope**           | Inside organizations (internal)       | Between organizations (global)       |
| **Focus**           | Shortest path (speed) ⚡              | Policy control (who goes where) 🛂    |
| **Convergence**     | Fast 🚀                              | Slower (because it’s global) 🐢      |

---

## ✅ Recap
- **OSPF** → Fast, shortest path, used inside companies.  
- **BGP** → Policy-based, global scale, connects the internet together.  


