<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&height=150&text=🧅%20Onion%20Domain%20Generator&fontSize=34&fontAlignY=35&animation=fadeIn&fontColor=FFFFFF&color=0:0F0F0F,50:1C1C1C,100:2D5BFF"/>

<br>

<img src="https://readme-typing-svg.herokuapp.com?font=JetBrains+Mono&weight=500&size=15&pause=1200&color=2D5BFF&center=true&vCenter=true&width=650&lines=Generate+.onion+domains+using+Tor...;Beginner-friendly+hidden+service+setup...;Simple+and+clean+Linux+workflow..." />

<br><br>

<img src="https://img.shields.io/badge/platform-Linux-2D5BFF?style=flat-square&logo=linux&logoColor=white">
<img src="https://img.shields.io/badge/network-Tor-1C1C1C?style=flat-square">
<img src="https://img.shields.io/badge/type-Guide-2D5BFF?style=flat-square">
<img src="https://img.shields.io/badge/focus-Privacy-1C1C1C?style=flat-square">

<br><br>

<img src="https://media.tenor.com/mCyP1bjo9S0AAAAi/mocha-bear-hearts.gif" width="50">

</div>

---

# Overview

A clean and beginner-friendly guide for generating a `.onion` domain using Tor Hidden Services.

The project focuses on:

* simplicity
* clean setup steps
* official sources
* lightweight configuration
* operational safety basics

---

# What is an Onion Domain?

An `.onion` domain is a private address inside the Tor network used for hidden services.

Example:

```text id="h2cr17"
abcdefghijklmnopqrstuvwxabcdefghijklmnopqrstuvwxabcdefghijkl.onion
```

---

# Requirements

```text id="8o3v7u"
Linux system
Tor installed
Basic terminal knowledge
```

---

# Install Tor

## Arch Linux

```bash id="twwfhl"
sudo pacman -S tor
```

Official source:

```text id="ks4j47"
https://archlinux.org/packages/extra/x86_64/tor/
```

---

## Ubuntu / Debian

```bash id="l2bd2r"
sudo apt update
sudo apt install tor
```

Official source:

```text id="s0y42v"
https://www.torproject.org/download/
```

---

# Hidden Service Setup

## Configure Tor

```bash id="uvr1sq"
sudo nano /etc/tor/torrc
```

Add:

```bash id="x7w92k"
HiddenServiceDir /var/lib/tor/my_hidden_service/
HiddenServicePort 80 127.0.0.1:8080
```

---

## Start Tor

```bash id="s9e3yb"
sudo systemctl start tor
```

or:

```bash id="umj0az"
tor
```

---

## Generate Domain

```bash id="wh8k2e"
cd /var/lib/tor/my_hidden_service/
cat hostname
```

Your `.onion` domain will be generated automatically.

---

# Testing

Run a local service on port `8080`, then open:

```text id="gwg1ei"
http://your-domain.onion
```

Use Tor Browser to access it.

---

# Vanity Domains

Optional tool:

```text id="x0j9v4"
mkp224o
```

Notes:

* CPU intensive
* May take time depending on prefix length

---

# Structure

```text id="udb0z9"
/var/lib/tor/my_hidden_service/
├── hostname
├── private_key
```

---

# Security

Operational safety guidelines are separated for clarity.

➡️ See:

```text id="a6m2i7"
WARNINGS.md
```

---

# Disclaimer

For educational and privacy-focused use only.

---

<div align="center">

<img src="https://readme-typing-svg.herokuapp.com?font=JetBrains+Mono&size=13&pause=1000&color=D5D8DE&center=true&vCenter=true&width=360&lines=privacy-focused...;lightweight+guide...;simple+hidden+service+setup..." />

<br><br>

<img src="https://media.tenor.com/DimzPZMypFcAAAAi/love-heart.gif" width="48">

<br><br>

<img src="https://capsule-render.vercel.app/api?type=waving&height=95&section=footer&color=0:2D5BFF,100:0F0F0F"/>

</div>
