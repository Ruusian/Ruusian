<div align="center">

# Hey there, I'm Abhik Sarkar 👋

### **Android Linux Engineer | Systems Programmer | Build-It-From-Scratch Hacker**

[![GitHub](https://img.shields.io/badge/-Ruusian-181717?style=for-the-badge&logo=github)](https://github.com/Ruusian)
[![Email](https://img.shields.io/badge/-abhiksarkar00@gmail.com-EA4335?style=for-the-badge&logo=gmail)](mailto:abhiksarkar00@gmail.com)
[![ASL](https://img.shields.io/badge/-ASL_Repo-00CED1?style=for-the-badge&logo=linux&logoColor=white)](https://github.com/Ruusian/ASL)

</div>

---

## 🧑‍💻 About Me

- 🔧 I build **Linux subsystems for Android** — think WSL, but running natively on your phone
- 🎮 I make **x86 games run on ARM64** phones via Box64 + Wine64 + DXVK
- 🖥️ I run **full XFCE desktops** with hardware-accelerated Vulkan rendering on mobile
- 🌐 I architect **multi-hop SSH tunnels** with sub-second connection times
- ☕ Powered by curiosity and way too much caffeine

```python
class Abhik:
    def __init__(self):
        self.role = "Android Linux Engineer"
        self.languages = ["Bash", "Python", "C"]
        self.os = ["Debian", "Arch", "Alpine", "Termux"]
        self.passion = "Turning phones into workstations"

    def current_quest(self):
        return "Building ASL — a full Linux subsystem for Android"
```

---

## 🚀 Featured Project

<div align="center">

### [**Android Subsystem for Linux (ASL)**](https://github.com/Ruusian/ASL) ⭐

*Like WSL, but for Android. A complete Linux subsystem management engine.*

[![Stars](https://img.shields.io/github/stars/Ruusian/ASL?style=social)](https://github.com/Ruusian/ASL)
[![Forks](https://img.shields.io/github/forks/Ruusian/ASL?style=social)](https://github.com/Ruusian/ASL)
[![Issues](https://img.shields.io/github/issues/Ruusian/ASL?style=social)](https://github.com/Ruusian/ASL/issues)

</div>

```
┌─────────────────────────────────────────────────────────┐
│           ANDROID SUBSYSTEM FOR LINUX (ASL)              │
├─────────────────────────────────────────────────────────┤
│  Debian 13 Trixie ARM64 + Mesa Turnip Vulkan            │
│  Box64 + Wine64 + DXVK + XFCE4 Desktop                 │
│  Modular Remote (Serveo + Oracle VPS + Ngrok + LAN)     │
│  GTK3 Control Center + 24/7 Auto-Reconnect Daemon       │
└─────────────────────────────────────────────────────────┘
```

| Feature | Description |
|:--------|:------------|
| 🐧 **Chroot Engine** | SELinux-safe mount isolation, 222+ packages, auto-repair |
| 🎮 **Gaming Stack** | Box64 v0.3.4 + Wine64 v10.0 + DXVK + MangoHud overlay |
| 🖥️ **GPU Acceleration** | Mesa Turnip Vulkan (Adreno 6xx/7xx), Zink OpenGL-over-Vulkan |
| 🌐 **Remote Access** | 4-layer failover: Oracle VPS (1s) → Serveo → Ngrok → LAN |
| 🎛️ **ASL Hub** | GTK3 Control Center with GUI for GPU, Gaming, Dev, Security |
| 🔧 **Dev Suite** | One-click Python, Node.js, GCC, Rust, Go, VS Code Server |
| 🛡️ **Security Suite** | Nmap, Wireshark/TShark, Netcat, Socat in isolated container |
| 📊 **Monitoring** | Thermal zones, MangoHud telemetry, resource manager |

---

## 📊 GitHub Stats

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=Ruusian&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0d1117&title_color=58a6ff&icon_color=79c0ff&text_color=c9d1d9" width="48%" />
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Ruusian&layout=compact&theme=tokyonight&hide_border=true&bg_color=0d1117&title_color=58a6ff&text_color=c9d1d9" width="48%" />

</div>

---

## 🛠️ Tech Arsenal

<div align="center">

| Category | Technologies |
|:---------|:-------------|
| **Languages** | ![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat&logo=gnubash&logoColor=white) ![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white) ![C](https://img.shields.io/badge/C-A8B9CC?style=flat&logo=c&logoColor=white) |
| **Linux** | ![Debian](https://img.shields.io/badge/Debian-A80030?style=flat&logo=debian&logoColor=white) ![Arch](https://img.shields.io/badge/Arch_Linux-1793D1?style=flat&logo=archlinux&logoColor=white) ![Termux](https://img.shields.io/badge/Termux-3D1F28?style=flat&logo=android&logoColor=white) |
| **GPU/Gaming** | ![Mesa](https://img.shields.io/badge/Mesa_Turnip-F57C00?style=flat) ![Box64](https://img.shields.io/badge/Box64-4CAF50?style=flat) ![Wine](https://img.shields.io/badge/Wine-8B0000?style=flat&logo=wine&logoColor=white) ![DXVK](https://img.shields.io/badge/DXVK-9C27B0?style=flat) |
| **Networking** | ![SSH](https://img.shields.io/badge/SSH-Tunnels-0097E6?style=flat) ![Ngrok](https://img.shields.io/badge/Ngrok-1F8ECE?style=flat) ![Oracle](https://img.shields.io/badge/Oracle_Cloud-F80000?style=flat&logo=oracle&logoColor=white) |
| **Desktop** | ![XFCE](https://img.shields.io/badge/XFCE4-233068?style=flat&logo=xfce&logoColor=white) ![GTK3](https://img.shields.io/badge/GTK3-4A86CF?style=flat) ![VNC](https://img.shields.io/badge/VNC-83D1E8?style=flat) |
| **DevOps** | ![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat&logo=githubactions&logoColor=white) ![ShellCheck](https://img.shields.io/badge/ShellCheck-4EAA25?style=flat) |

</div>

---

## 🏗️ Architecture

<div align="center">

```
     Android Device (Qualcomm 8-core Adreno 640v2)
     ┌──────────────────────────────────────────────┐
     │  Termux + ASL Engine                         │
     │  ┌────────────┐  ┌────────────┐  ┌────────┐ │
     │  │ Debian 13  │  │ Box64      │  │ XFCE4  │ │
     │  │ Trixie     │  │ + Wine64   │  │ Desktop│ │
     │  │ ARM64      │  │ + DXVK     │  │ + VNC  │ │
     │  └──────▲─────┘  └─────▲──────┘  └───▲────┘ │
     │         │              │              │      │
     │  ┌──────┴──────────────┴──────────────┴────┐ │
     │  │    Mesa Turnip Vulkan (Direct HW Accel) │ │
     │  └─────────────────────▲───────────────────┘ │
     └────────────────────────┼─────────────────────┘
                              │ /dev/kgsl-3d0
     ┌────────────────────────┴─────────────────────┐
     │           Android Kernel 4.14 (Myth)          │
     └──────────────────────────────────────────────┘
                              │
                    SSH Reverse Tunnel
                              │
     ┌────────────────────────▼─────────────────────┐
     │         Oracle Cloud VPS (Ubuntu 24.04)       │
     │         Always-On Private Relay                │
     └──────────────────────────────────────────────┘
```

</div>

---

## 📈 Recent Activity

<!-- TSR:START ACTIVITY -->
- 🔄 Loading...
<!-- TSR:END ACTIVITY -->

---

## 🎯 Current Focus

- 🔨 Optimizing ASL v1.6 — modular remote bridge, TCP tuning, sub-second SSH
- 🎮 Getting Wine + Box64 gaming working on Adreno 640v2
- 🌐 Multi-layer remote access with 1s connection times
- 📦 Packaging ASL for one-command installation

---

<div align="center">

**"Turning $200 phones into $2000 workstations, one kernel hack at a time."** ⚡

<img src="https://komarev.com/ghpvc/?username=Ruusian&color=blue&style=flat" alt="Profile views" />

</div>
