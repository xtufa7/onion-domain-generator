<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&height=150&text=🧅%20Onion%20Domain%20Generator&fontSize=34&fontAlignY=35&animation=fadeIn&fontColor=FFFFFF&color=0:1A0000,50:520000,100:B30000"/>

<br>

<img src="https://readme-typing-svg.herokuapp.com?font=JetBrains+Mono&weight=500&size=15&pause=1200&color=FF4D4D&center=true&vCenter=true&width=700&lines=Generate+.onion+domains+using+Tor...;Hidden+service+setup+for+beginners...;Privacy-focused+Linux+workflow..." />

<br><br>

<img src="https://img.shields.io/badge/platform-Linux-B30000?style=for-the-badge&logo=linux&logoColor=white">
<img src="https://img.shields.io/badge/network-Tor-1A0000?style=for-the-badge">
<img src="https://img.shields.io/badge/type-Guide-B30000?style=for-the-badge">
<img src="https://img.shields.io/badge/privacy-focused-1A0000?style=for-the-badge">

<br><br>

<img src="https://media.tenor.com/mCyP1bjo9S0AAAAi/mocha-bear-hearts.gif" width="50">

</div>

---

# 🧅 Onion Domain Generator

A clean and beginner-friendly guide to generate a `.onion` domain using Tor Hidden Services.

---

## 📌 What is an Onion Domain?

An `.onion` domain is a private address inside the Tor network used for hidden services without exposing the server’s real identity.

Example:

```text
abcdefghijklmnopqrstuvwxabcdefghijklmnopqrstuvwxabcdefghijkl.onion
```

---

## ⚙️ Requirements

```text
Linux system
Tor installed
Basic terminal knowledge
```

---

# 📥 Install Tor

## Arch Linux

```bash
sudo pacman -S tor
```

Official source:

```text
https://archlinux.org/packages/extra/x86_64/tor/
```

---

## Ubuntu / Debian

```bash
sudo apt update
sudo apt install tor
```

Official source:

```text
https://www.torproject.org/download/
```

---

# 🚀 Step-by-Step Setup

## 1️⃣ Configure Hidden Service

```bash
sudo nano /etc/tor/torrc
```

Add:

```bash
HiddenServiceDir /var/lib/tor/my_hidden_service/
HiddenServicePort 80 127.0.0.1:8080
```

---

## 2️⃣ Start Tor

```bash
sudo systemctl start tor
```

or:

```bash
tor
```

---

## 3️⃣ Generate Your Onion Domain

```bash
cd /var/lib/tor/my_hidden_service/
cat hostname
```

Your `.onion` domain will be generated automatically.

---

# 🧪 Testing

Run a local service on port `8080`, then open:

```text
http://your-domain.onion
```

Use Tor Browser to access it.

---

# 🧬 Vanity Domains

Optional tool:

```text
mkp224o
```

Notes:

* CPU intensive
* Generation time depends on prefix complexity

---

# 📂 Directory Structure

```text
/var/lib/tor/my_hidden_service/
├── hostname
├── private_key
```

---

# ⚠️ Security & Operational Safety

<div align="center">

<img src="https://readme-typing-svg.herokuapp.com?font=JetBrains+Mono&size=13&pause=1000&color=FF6B6B&center=true&vCenter=true&width=420&lines=misconfiguration+can+expose+your+identity...;always+test+inside+an+isolated+environment..." />

<br><br>

<a href="WARNINGS.md">
<img src="https://img.shields.io/badge/⚠️%20Security%20Guidelines-B30000?style=for-the-badge&labelColor=1A0000">
</a>

</div>

---

# ⚠️ Disclaimer

For educational and privacy-focused use only.

---

<div align="center">

<img src="https://media.tenor.com/DimzPZMypFcAAAAi/love-heart.gif" width="46">

<br><br>

<img src="https://capsule-render.vercel.app/api?type=waving&height=95&section=footer&color=0:B30000,100:1A0000"/>

</div>
