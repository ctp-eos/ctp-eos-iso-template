
# CTP-EOS Linux ISO Template

Welcome to **CTP-EOS Linux**, a next-generation Linux distribution powered by **CTP Energy Science**. This repository provides the complete framework for building **CTP-EOS Live ISO**, pre-configured with **XFCE**, **Calamares Installer**, and initial CTP-Energy placeholders.

---

## 📦 What is CTP-EOS Linux?

CTP-EOS Linux is a custom-built Arch Linux-based distribution designed to serve as the foundation for:

- Advanced scientific research under **CTP Energy Science**.
- Secure computing with future integration of **CTP Energy Isolation Framework (CEIF)**.
- User-friendly desktop experience with **XFCE**.
- Full live environment, allowing you to test and install from a fully functional system.
- CTP-EOS is the 'Disclosure-distro' or the 'disclosure-linux' about the UFO truth/UAP truth or the truth about UFOs/UAPs or 'CTP craft' (by name)

---

## ⚙️ Key Features

- **Arch Linux base for rolling updates and flexibility.**
- **XFCE desktop for lightweight performance.**
- **Calamares Installer pre-branded for CTP-EOS.**
- **Live user: `CTP-EOS` (password: `ctp-eos`).**
- **Customizable systemd services & nftables firewall for future CTP Energy isolation.**

---

## 📂 Directory Structure

```
ctp-eos-iso/
├── build.sh                 # One-click ISO build script
├── README.md                 # This file
├── profile/                  # Archiso profile files
│   ├── airootfs/             # Files that go into the live filesystem
│   │   ├── etc/               # Config files (hostname, nftables, etc.)
│   │   ├── home/CTP-EOS/     # Default live user home
│   │   ├── root/              # Optional root files
│   ├── packages.x86_64       # Package list for the ISO
├── branding/                 # Logos, wallpapers, and visual assets
├── calamares/                 # Installer configuration
│   ├── settings.conf         # Core Calamares settings
│   ├── branding/             # Installer branding files
│   ├── modules/              # Individual module configs (users, partitioning, etc.)
```

---

## 🛠️ Build Instructions

### 1. Install dependencies
Ensure your build environment has:
- `archiso`
- `calamares`
- Standard Arch Linux build tools (`base-devel`, `git`, etc.)

### 2. Clone Repository
```bash
git clone https://github.com/ctp-eos/ctp-eos-iso-template-preinstall
cd ctp-eos-iso-template-preinstall
```

### 3. Build the ISO
```bash
./build.sh
```
This will generate `ctp-eos-linux-x86_64.iso` in the `out/` directory.

---

## 🔧 Customization Notes

### Changing Desktop Environment
- Current default: **XFCE**.
- Swap packages in `profile/packages.x86_64` if you want **KDE, GNOME, etc.**

### Branding
- Replace images in `branding/` and `calamares/branding/` for your custom logos and wallpapers.
- Edit `calamares/modules` files to change user defaults, partitioning schemes, etc.

---

## 🔒 Security Roadmap

Future versions of **CTP-EOS Linux** will include:

- **CTP Energy Isolation Framework (CEIF)** for VM-based compartmentalization.
- **Qubes-like network isolation via nftables.**
- **CTP Energy Science systemd daemons for resource monitoring and energy data collection.**
- **Pre-hardened kernel options for scientific compute security.**

---

## 📝 Default Credentials

| User   | Password | Purpose                      |
|-------|----------|------------------|
| `CTP-EOS` | `ctp-eos` | Live session user |
| `root`    | (set during install) | Post-install system root |

---

## 🌐 Official Project Links

- **Website:** https://ctp-eos.org (CTP Energy Science Foundation project)  
- **Repository:** https://github.com/ctp-eos/ctp-eos-iso-template-preinstall 
- **Issue Tracker:** Use GitHub Issues for feedback, bugs, and feature requests.

---

## 🚀 Contributing

Contributions are welcome! Fork the repository, submit pull requests, or suggest new features to support **CTP Energy Science research**.

---

## 📜 License

© 2025 CTP Energy, LLC.  
Released under the MIT License (or your preferred license).

---

## 🛸 About CTP Energy Science

**CTP Energy Science** is a revolutionary scientific framework exploring **hyper-spatial energy systems, quantum material interactions, and extraterrestrial technology integration**. Learn more at [www.ctp-energy.com].

