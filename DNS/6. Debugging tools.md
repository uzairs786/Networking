# 🛠️ DNS Debugging Tools – `nslookup` & `dig`

Two common tools to query DNS records and debug issues:  
- 🔹 `nslookup` → Simple, widely available  
- 🔹 `dig` → More detailed & flexible  

---

## 🔎 1. nslookup
- Basic tool to query DNS.  
- Installed by default on most systems (Windows, macOS, Linux).  

### 🖥️ Syntax
```bash
nslookup domain.com
````

### 📌 Example

```bash
nslookup google.com
```

**Output breakdown:**

* **Server** → The DNS server used for the query (usually your router/ISP).
* **Address** → IP of that DNS server, uses **port 53** (DNS).
* **Non-authoritative answer** → Response came from a **cache**, not the original authoritative server.
* **Name & Address** → The resolved IP(s) of the domain.

---

## 🔎 2. dig (Domain Information Grouper)

* More advanced and flexible than `nslookup`.
* Shows detailed sections (Question, Answer, Query time, etc.).
* Installed by default on Linux/macOS (can be added on Windows).

### 🖥️ Syntax

```bash
dig domain.com
```

### 📌 Example

```bash
dig google.com
```

**Output breakdown:**

* **QUESTION SECTION** → What you asked for (domain queried).
* **ANSWER SECTION** → The actual record(s) returned (e.g., IPs).
* **Query time** → How long the DNS lookup took.

---

## ⚡ Useful dig Options

* **Short output (just answer):**

  ```bash
  dig +short google.com
  ```

  ➝ Returns only IP addresses.

* **Find nameservers:**

  ```bash
  dig +short NS google.com
  ```

  ➝ Returns authoritative nameservers.

---

## ✅ Quick Summary

* 🔹 **nslookup** → Quick & simple DNS queries.
* 🔹 **dig** → Advanced, flexible, detailed queries.
* Both are **essential tools** for network engineers & DevOps to troubleshoot DNS issues.



