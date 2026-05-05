# ⚠️ Security & Operational Safety Guidelines

Running a hidden service requires careful isolation and safe practices.

---

## 🔒 Isolate Your Service

* Use a virtual machine or container (e.g. Docker)
* Do not run on your main system
* Use a low-privilege user account

---

## 🌐 Network Separation

* Bind services to `127.0.0.1` only
* Do not expose ports publicly
* Keep Tor traffic isolated

---

## 🧱 Firewall & Access Control

* Use `ufw` or `iptables`
* Allow only required ports
* Disable unnecessary services

---

## 🕵️ Avoid Identity Leakage

* Do not use real identifiers
* Remove metadata from files
* Avoid linking to public accounts

---

## 🧰 Keep Software Updated

* Update Tor regularly
* Patch vulnerabilities

---

## 📂 Protect Your Keys

* Never share `private_key`
* Restrict permissions:

```bash
chmod 700 /var/lib/tor/my_hidden_service/
```

---

## 🔍 Logging & Monitoring

* Minimize logs
* Avoid sensitive data storage
* Monitor anomalies

---

## ⚡ Reverse Proxy (Optional)

* Use Nginx
* Apply rate limiting
* Hide backend details

---

## 🧪 Safe Testing

* Test locally first
* Avoid direct production deployment

---

## 🚫 Important Notice

* Misconfiguration may expose your real IP
* Anonymity is not guaranteed if used incorrectly

---
