# 🧅 Onion Domain Generator

A clean and beginner-friendly guide to generate a `.onion` domain using Tor Hidden Services.

---

## 📌 What is an Onion Domain?

An `.onion` domain is a private address inside the Tor network, used to access hidden services without exposing the server’s real identity.

Example:

```
abcdefghijklmnopqrstuvwxabcdefghijklmnopqrstuvwxabcdefghijkl.onion
```

---

## ⚙️ Requirements

* Linux system (Arch / Ubuntu / Debian)
* Tor installed
* Basic terminal knowledge

---

## 📥 Install Tor (Official Sources)

### Arch Linux

Install directly via pacman:

```bash
sudo pacman -S tor
```

Official website:
https://archlinux.org/packages/extra/x86_64/tor/

---

### Ubuntu / Debian

```bash
sudo apt update
sudo apt install tor
```

Official website:
https://www.torproject.org/download/

---

## 🚀 Step-by-Step Setup

### 1️⃣ Configure Hidden Service

Open configuration file:

```bash
sudo nano /etc/tor/torrc
```

Add:

```bash
HiddenServiceDir /var/lib/tor/my_hidden_service/
HiddenServicePort 80 127.0.0.1:8080
```

---

### 2️⃣ Start Tor

```bash
sudo systemctl start tor
```

or:

```bash
tor
```

---

### 3️⃣ Get Your Onion Domain

```bash
cd /var/lib/tor/my_hidden_service/
cat hostname
```

Your `.onion` domain will be generated automatically.

---

## 🧪 Testing

Run a local service on port `8080`, then open:

```
http://your-domain.onion
```

Use Tor Browser to access it.

---

## 🧬 Vanity Domains (Optional)

To generate custom prefixes:

* mkp224o

Note:

* May take significant time
* CPU intensive

---

## 📂 Directory Structure

```
/var/lib/tor/my_hidden_service/
├── hostname
├── private_key
```

---

## 🔐 Security & Safety

Security guidelines are separated for clarity.

➡️ See: [Security Guidelines](./WARNINGS.md)

---

## ⚠️ Disclaimer

For educational and privacy-focused use only.

---
