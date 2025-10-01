# 📝 Assignment: Domain + EC2 + NGINX  

## 🎯 Task Outline  
- **Objective:**  
  Buy a custom domain and host a simple web page on an EC2 instance.  

- **Requirements:**  
  1. Buy/register a domain (AWS Route 53).  
  2. Launch an EC2 instance.  
  3. Install and run NGINX on port 80.  
  4. Configure Route 53 DNS to point the domain to the EC2.  
  5. Access the webpage via `nginx.mydomain.com`.  

---

## 🛠 Steps Taken  

### 1. Domain Setup  
- Registered a domain using **AWS Route 53**.  
- Waited for the request to be accepted and the domain to be available.  

---

### 2. Launch EC2 Instance  
- Started a new **Ubuntu EC2 instance**.  
- Allowed inbound traffic on **port 80 (HTTP)** in the **security group**.  
- Copied the **Public IPv4 address** for later use from the AWS Console

---

### 3. Install and Run NGINX  
Connected to the EC2 via SSH:  

```bash
ssh -i my-key.pem ubuntu@<EC2-Public-IP>
````

Installed and started NGINX:

```bash
sudo apt update
sudo apt install -y nginx
sudo systemctl enable nginx
sudo systemctl start nginx
```

✅ Confirmed NGINX was working by visiting:

```
http://<EC2-Public-IP>
```

---

### 4. Configure DNS (Route 53)

* Opened **Route 53 → Hosted Zones**.
* Added an **A Record**:

  * **Name:** `nginx` (for subdomain `nginx.uzairabdsamad.co.uk`).
  * **Value:** EC2’s Public IPv4 address.
  * **TTL:** 300 (default).

This enabled the `nginx` subdomain to map to the public IP Address of my EC2 Instance which had installed NGINX. 

---

### 5. Test Domain

Visited in browser:

```
http://nginx.uzairabdsamad.co.uk
```

* Page loaded successfully showing the **NGINX default welcome page** 🎉

![screenshot of nginx](


---

## ✅ Outcome

* Domain successfully linked to EC2 instance.
* NGINX is publicly accessible at `nginx.mydomain.com`.

---

## ⚡ Cost Management

* Stopped the EC2 instance after testing to avoid running costs.
* Resources can be terminated when no longer needed.


