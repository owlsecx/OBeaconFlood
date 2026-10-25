# 🦉 OBeaconFlood

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-Security-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0-cyan?style=flat-square"/>
</p>

> **OBeaconFlood** — part of the OwlSec Toolkit.

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

OBeaconFlood analyzes 802.11 packet captures to detect beacon-flood and rogue-SSID attacks. It parses radiotap and 802.11 frames to measure SSID fan-out per BSSID, beacon rates and randomised MACs. It can also write a synthetic beacon PCAP for authorised lab replay, but it never transmits a frame.

---

## ✨ Features

- Beacon-flood analyzer for pcap / pcapng captures with a full radiotap and 802.11 parser
- Detects per-BSSID SSID fan-out, abnormal beacon rates and random MAC addresses
- Offline synthetic beacon-set PCAP generator from an SSID list (no transmission)
- Findings graded A+ to F with MITRE ATT&CK mapping
- Reports in TXT / JSON / Markdown / CSV / SARIF; exits with code 3 on CRITICAL/HIGH findings

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OBeaconFlood                               # interactive menu
./OBeaconFlood --analyze capture.pcapng
./OBeaconFlood --generate --ssids ssids.txt --out lab.pcap
./OBeaconFlood --demo
```

Run `./OBeaconFlood --help` for the full list of options.

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
