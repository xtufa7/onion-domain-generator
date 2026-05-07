<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&height=155&text=🧅%20Onion%20Domain%20Generator&fontSize=33&fontAlignY=35&animation=fadeIn&fontColor=FFFFFF&color=0:120000,45:4A0000,100:B30000"/>

<br>

<img src="https://readme-typing-svg.herokuapp.com?font=JetBrains+Mono&weight=500&size=15&pause=1200&color=FF5C5C&center=true&vCenter=true&width=720&lines=Generate+.onion+domains+using+Tor...;Hidden+service+setup+for+beginners...;Privacy-focused+Linux+workflow..." />

<br><br>

<img src="https://img.shields.io/badge/Linux-B30000?style=for-the-badge&logo=linux&logoColor=white">
<img src="https://img.shields.io/badge/Tor-1A0000?style=for-the-badge">
<img src="https://img.shields.io/badge/Guide-B30000?style=for-the-badge">
<img src="https://img.shields.io/badge/Privacy-1A0000?style=for-the-badge">

<br><br>

<img src="https://media.tenor.com/mCyP1bjo9S0AAAAi/mocha-bear-hearts.gif" width="50">

</div>

---

# 🧅 Onion Domain Generator

A clean beginner-friendly guide for generating `.onion` domains using Tor Hidden Services.

---

## 📌 What is an Onion Domain?

An `.onion` domain is a private address inside the Tor network used for hidden services without exposing the real server identity.

Example:

```text id="p9q8xj"
abcdefghijklmnopqrstuvwxabcdefghijklmnopqrstuvwxabcdefghijkl.onion
```

---

## ⚙️ Requirements

```text id="x4f0kq"
Linux system
Tor installed
Basic terminal knowledge
```

---

# 📥 Install Tor

## Arch Linux

```bash id="e4g0yt"
sudo pacman -S tor
```

Official package:

```text id="s1m8qw"
https://archlinux.org/packages/extra/x86_64/tor/
```

---

## Ubuntu / Debian

```bash id="v4z8lo"
sudo apt update
sudo apt install tor
```

Official download:

```text id="h7b3pr"
https://www.torproject.org/download/
```

---

# 🚀 Setup

## Configure Hidden Service

```bash id="d3v8ri"
sudo nano /etc/tor/torrc
```

Add:

```bash id="z5j1on"
HiddenServiceDir /var/lib/tor/my_hidden_service/
HiddenServicePort 80 127.0.0.1:8080
```

---

## Start Tor

```bash id="u7k3ab"
sudo systemctl start tor
```

or:

```bash id="r8x0nt"
tor
```

---

## Generate Domain

```bash id="n6m0dx"
cd /var/lib/tor/my_hidden_service/
cat hostname
```

Your `.onion` domain will be generated automatically.

---

# 🧪 Testing

Run a local service on port `8080`, then open:

```text id="f8j0pw"
http://your-domain.onion
```

Use Tor Browser to access it.

---

# 🧬 Vanity Domains

Optional utility:

```text id="j9y6qa"
mkp224o
```

Notes:

* CPU intensive
* Generation speed depends on prefix complexity

---

# 📂 Directory Structure

```text id="q5w9nz"
/var/lib/tor/my_hidden_service/
├── hostname
├── private_key
```

---

# ⚠️ Security & Operational Safety

<div align="center">

<img src="https://readme-typing-svg.herokuapp.com?font=JetBrains+Mono&size=13&pause=1000&color=FF7070&center=true&vCenter=true&width=470&lines=misconfiguration+may+expose+your+real+identity...;always+test+inside+an+isolated+environment...">

<br><br>

<a href="./WARNINGS.md">
<img src="https://img.shields.io/badge/Open-WARNINGS.md-B30000?style=for-the-badge" alt="Open WARNINGS.md">
</a>

</div>


---

# ⚠️ Disclaimer

For educational and privacy-focused use only.

---

<div align="center">

<img src="https://media.tenor.com/DimzPZMypFcAAAAi/love-heart.gif" width="45">

<br><br>

<img src="https://capsule-render.vercel.app/api?type=waving&height=95&section=footer&color=0:B30000,100:120000"/>

</div>
