# 🔐 certinstaller

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Bash Shell](https://img.shields.io/badge/Language-Bash-green.svg)](#)

*Read this in other languages: [English](#english) | [Español](#español)*

---

## English

A colorful, easy-to-use Bash script to batch install digital certificates (`.p12` or `.pfx`) into the user's NSS database on Linux.

By adding certificates to the NSS database (`~/.pki/nssdb`), native applications like **Okular, Google Chrome, and Chromium** will automatically recognize them for digital signing and authentication. 

> **Note:** This tool does not work for Adobe Acrobat, as Adobe uses its own internal certificate store.

### 📋 Prerequisites

This script requires `pk12util` and `certutil`. On Debian/Ubuntu-based distributions, install them with:

```bash
sudo apt update
sudo apt install libnss3-tools
