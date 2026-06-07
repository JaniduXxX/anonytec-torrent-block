<div align="center">

<img src="https://avatars.githubusercontent.com/JaniduXxX" 
     width="120" 
     style="border-radius:50%; border: 3px solid #00bcd4;" 
     alt="Janidu Emalga"/>
 
<br/>
### 👤 Janidu Emalga
`🇱🇰 Sri Lanka` &nbsp;·&nbsp; `ANONYTEC` &nbsp;·&nbsp; `Linux Security`
 
[![GitHub](https://img.shields.io/badge/GitHub-Janidu--Emalga-181717?style=flat-square&logo=github)](https://github.com/yourusername)
[![YouTube](https://img.shields.io/badge/YouTube-ANONYTEC-FF0000?style=flat-square&logo=youtube)](https://youtube.com/@yourchannel)
[![Telegram](https://img.shields.io/badge/Telegram-ANONYTEC-2CA5E0?style=flat-square&logo=telegram)](https://t.me/yourchannel)
 
---
 
```
░█████╗░███╗░░██╗░█████╗░███╗░░██╗██╗░░░██╗████████╗███████╗░█████╗░
██╔══██╗████╗░██║██╔══██╗████╗░██║╚██╗░██╔╝╚══██╔══╝██╔════╝██╔══██╗
███████║██╔██╗██║██║░░██║██╔██╗██║░╚████╔╝░░░░██║░░░█████╗░░██║░░╚═╝
██╔══██║██║╚████║██║░░██║██║╚████║░░╚██╔╝░░░░░██║░░░██╔══╝░░██║░░██╗
██║░░██║██║░╚███║╚█████╔╝██║░╚███║░░░██║░░░░░░██║░░░███████╗╚█████╔╝
╚═╝░░╚═╝╚═╝░░╚══╝░╚════╝░╚═╝░░╚══╝░░░╚═╝░░░░░╚═╝░░░╚══════╝░╚════╝░
```
 
# 🛡️ ANONYTEC — TORRENT BLOCK
 
**BitTorrent & P2P Traffic Blocker — Kernel Level Firewall**
 
[![Bash](https://img.shields.io/badge/Language-Bash-green?style=for-the-badge&logo=gnubash)](https://www.gnu.org/software/bash/)
[![Platform](https://img.shields.io/badge/Platform-Linux%20VPS-blue?style=for-the-badge&logo=linux)](https://www.linux.org/)
[![iptables](https://img.shields.io/badge/Engine-iptables-red?style=for-the-badge)](https://netfilter.org/)
[![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)](LICENSE)
[![Version](https://img.shields.io/badge/Version-v1.0-cyan?style=for-the-badge)](.)
 
*coded by **Janidu Emalga** · ANONYTEC*
 
</div>

---
 
## 📖 විස්තරය / Description
 
<table>
<tr>
<td width="50%">
### 🇱🇰 සිංහල
 
**ANONYTEC Torrent Block** යනු Linux VPS සර්වර් එකක BitTorrent සහ P2P ට්‍රැෆික් සම්පූර්ණයෙන්ම kernel level හිදී block කිරීමේ හැකියාව ඇති Bash script එකකි.
 
`iptables` භාවිතා කර port blocking, deep packet inspection (DPI) සහ DHT blocking ක්‍රම හරහා torrent ට්‍රැෆික් හඳුනාගෙන drop කරයි. Reboot වූ පසුද rules ක්‍රියාත්මක වේ.
 
</td>
<td width="50%">
### 🇬🇧 English
 
**ANONYTEC Torrent Block** is a Bash script that completely blocks BitTorrent and P2P traffic at the kernel level on a Linux VPS server.
 
It uses `iptables` for port blocking, deep packet inspection (DPI), and DHT blocking to detect and drop torrent traffic. Rules persist across reboots automatically.
 
</td>
</tr>
</table>
---
 
## ✨ Features / විශේෂාංග
 
| # | Feature | සිංහල |
|---|---------|--------|
| ✅ | Auto root privilege check | Root පරීක්ෂාව |
| ✅ | Auto install iptables, iptables-persistent, ipset | ස්වයංක්‍රීය ස්ථාපනය |
| ✅ | Block BitTorrent ports TCP/UDP | Default ports block |
| ✅ | Block P2P tracker ports  Tracker ports block |
| ✅ | DPI string matching 
| ✅ | DHT (Distributed Hash Table) blocking | DHT ට්‍රැෆික් block |
| ✅ | Permanent rules | Reboot-safe rules |

 
---
 
## ⚙️ Requirements / අවශ්‍යතා
 
```
OS       : Ubuntu / Debian (apt-get)  |  CentOS / RHEL (yum)  |  Fedora (dnf)
Access   : Root / sudo
Packages : iptables, iptables-persistent, ipset  ← auto installed
```
 
---
 
## 🚀 Installation / ස්ථාපනය
 
### 1️⃣ Download / බාගත කිරීම
 
```bash
git clone https://github.com/JaniduXxX/anonytec-torrent-block.git
cd anonytec-torrent-block
```
 
### 2️⃣ Permission / අවසර දීම
 
```bash
chmod +x ANONYTEC_TORRENT_BLOCK.sh
```
 
### 3️⃣ Run / ක්‍රියාත්මක කිරීම
 
```bash
sudo bash ANONYTEC_TORRENT_BLOCK.sh
```
 
---

 
## 🔍 How It Works / ක්‍රියාකාරිත්වය
 
<table>
<tr>
<th>Layer</th>
<th>Method</th>
<th>සිංහල විස්තරය</th>
</tr>
<tr>
<td>🔴 Layer 1</td>
<td>Port Range Block </td>
<td>BitTorrent default ports සම්පූර්ණයෙන් block කිරීම</td>
</tr>
<tr>
<td>🟠 Layer 2</td>
<td>Tracker Port Block</td>
<td>Tracker සර්වර් port block කිරීම</td>
</tr>
<tr>
<td>🟡 Layer 3</td>
<td>DPI String Matching</td>
<td>Packet ඇතුළේ torrent signatures හඳුනා drop කිරීම</td>
</tr>
<tr>
<td>🟢 Layer 4</td>
<td>DHT Protocol Block</td>
<td>Distributed Hash Table UDP ට්‍රැෆික් block කිරීම</td>
</tr>
<tr>
<td>🔵 Layer 5</td>
<td>Persistent Save</td>
<td>Reboot වූ පසුද rules active ව තිබීම</td>
</tr>
</table>
---
 

 
## ↩️ Uninstall / ඉවත් කිරීම
 
> ⚠️ සියලු iptables rules ඉවත් කිරීමට / Remove all iptables rules:
 
```bash
sudo iptables -F
sudo iptables -X
sudo netfilter-persistent save
```
 
---
 
## 📁 Project Structure / ගොනු ව්‍යුහය
 
```
anonytec-torrent-block/
│
├── ANONYTEC_TORRENT_BLOCK.sh   ← Main script (obfuscated)
├── README.md                   ← Documentation
└── LICENSE                     ← MIT License
```
 
---
 
## ⚠️ Disclaimer / වගකීම් නිෂේධනය
 
<table>
<tr>
<td>
🇱🇰 සිංහල — මෙම script එක නිදහස් භාවිතය සඳහා නිකුත් කරන ලදී. ඕනෑම හානියකට කර්තෘ වගකිව නොහේ. නිසි අවසරය ඇති server හා network හිදී පමණක් භාවිතා කරන්න.
 
</td>
</tr>
<tr>
<td>
🇬🇧 English — This script is released for free use. The author holds no responsibility for any damage caused. Use only on servers and networks you own or have explicit permission to manage.
 
</td>
</tr>
</table>
---
 
## 👤 Author / කර්තෘ
 
<div align="center">
| | |
|---|---|
| **Name** | Janidu Emalga |
| **Project** | ANONYTEC |
| **Tool** | ANONYTEC Torrent Block v1.0 |
| **Platform** | Linux VPS · iptables |
 
---
 
<div align="center">
**⭐ Star this repo if it helped you! / ප්‍රයෝජනවත් නම් Star කරන්න!**
 
*© 2026 ANONYTEC · coded by Janidu Emalga*
 
</div>
