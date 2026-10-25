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


OWpConfX is an offline, read-only WordPress configuration and deployment auditor that parses wp-config.php via a safe tokenizer (never executing PHP) alongside .htaccess and server rules. It checks security keys/salts, database credentials, debug exposure, file-permission posture, dangerous constants and known hardening gaps. Secrets are masked, findings are mapped to CWE and MITRE ATT&CK, and reports export to TXT, Markdown, JSON, CSV or SARIF.

---

## ✨ Features


- Safe wp-config.php tokenizer (no PHP execution) plus .htaccess and server-rule review
- Security keys/salts checks: missing, default or weak AUTH_KEY/SALT definitions
- Database credential exposure (masked), table-prefix and DB-host hardening checks
- Debug/exposure review: WP_DEBUG, DISALLOW_FILE_EDIT, FORCE_SSL_ADMIN, automatic updates
- File-permission posture and dangerous constants (FS_METHOD, WP_ALLOW_REPAIR) detection
- Secrets masked, CWE+ATT&CK mapping and TXT/MD/JSON/CSV/SARIF export with --fail-on gating

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage


```bash
./OWpConfX --scan -f sarif -o wpconf.sarif
./OWpConfX --config /var/www/html/wp-config.php
./OWpConfX -r /mnt/image --fail-on high --json
./OWpConfX --demo
./OWpConfX --help
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
