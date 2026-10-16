# 🦉 OWpConfX

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OWeb-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0.0-cyan?style=flat-square"/>
</p>

> **OWpConfX** — WordPress Installation Configuration Auditor

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

Offline WordPress installation configuration hardening auditor

---

## ✨ Features

- Safe PHP tokenizer for wp-config.php — define() & $var parsing, never executes PHP; comments/heredoc/getenv aware
- Debug, admin hardening, keys & salts, database creds & transport, updates / core version, cookie scope checks
- Webroot, .htaccess, wp-content, uploads, backups & dumps, plugin / theme / mu-plugin inventory, file permissions
- Score + A+…F grade, CWE + MITRE ATT&CK, TXT/MD/JSON/CSV/ SARIF, --fail-on gate, templates, salt generator, --demo

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OWpConfX
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
