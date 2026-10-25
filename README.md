# Abhik Sarkar

Systems & low-level software engineer focused on Android kernel internals, Linux subsystem architectures, and hardware-accelerated computing on ARM64.

Creator and maintainer of **[ASL (Android Subsystem for Linux)](https://github.com/Ruusian/ASL)** — an enterprise-grade containerization engine and XFCE4 workstation for rooted Android devices, featuring direct Qualcomm Adreno GPU hardware pass-through via open-source Mesa Turnip Vulkan and Zink OpenGL.

---

## ⚡ Primary Focus & Systems Engineering

- **Linux Kernel & Containerization**: Native chroot subsystem execution with private mount namespaces (`--make-rprivate`, `--make-rslave`), eliminating Android host partition pollution (`/system`, `/vendor`, `/apex`) and preventing kernel panics.
- **Direct Hardware Graphics (GPU)**: Direct `/dev/kgsl-3d0` node pass-through on Qualcomm Adreno 6xx/7xx/8xx GPUs with Mesa Turnip Vulkan 1.3 and Zink OpenGL 4.6, delivering 60 FPS hardware-rendered desktop graphics into Termux:X11.
- **Low-Latency Audio & Display IPC**: Shared-memory X11 display server integration paired with native PulseAudio TCP streaming (`127.0.0.1:4713`) under 15ms buffer latency.
- **Resilient Infrastructure**: Autonomous background daemons, 4-tier reverse SSH failover relays (Oracle Cloud VPS, Serveo, Ngrok, LAN), and Android 12+ Phantom Process Killer (PPK) mitigations.

---

## 🚀 Flagship Project: [Android Subsystem for Linux (ASL)](https://github.com/Ruusian/ASL)

> *Native, hardware-accelerated Linux subsystem and XFCE4 workstation for Android ARM64 devices.*

```text
 ┌────────────────────────────────────────────────────────────────────────────┐
 │                      ANDROID HARDWARE SUBSYSTEM (ARM64)                    │
 │    Qualcomm Adreno GPU  •  Octa-Core Kryo CPU  •  zRAM + Virtual Swap      │
 └─────────────────────────────────────┬──────────────────────────────────────┘
                                       │ /dev/kgsl-3d0 direct hardware bindings
 ┌─────────────────────────────────────▼──────────────────────────────────────┐
 │                    ASL CONTAINER & WORKSTATION CORE                        │
 │  ┌─────────────────────────┐  ┌─────────────────────────┐  ┌────────────┐  │
 │  │ Turnip Mesa Vulkan      │  │ XFCE4 Desktop & D-Bus   │  │ OmniRoute  │  │
 │  │ Hardware 3D Driver      │  │ (Termux:X11 Display :0) │  │ AI Gateway │  │
 │  └────────────┬────────────┘  └────────────┬────────────┘  └─────┬──────┘  │
 │               └──────────────────────┬─────┴─────────────────────┘         │
 │                                      ▼                                     │
 │        Dynamic Multi-Distro Linux Container (Debian / Ubuntu / Arch)       │
 └─────────────────────────────────────┬──────────────────────────────────────┘
                                       │ Reverse SSH Tunnels & TCP BBR Tuning
 ┌─────────────────────────────────────▼──────────────────────────────────────┐
 │                      24/7 RESILIENT REMOTE MESH RELAYS                     │
 │     Oracle Cloud VPS (Port 2222) • LAN SSH (8022) • Serveo • Ngrok         │
 └────────────────────────────────────────────────────────────────────────────┘
```

### Live Diagnostic Telemetry

```text
 ┌──[ruusian@android-workstation]─[~]
 └──$ asl doctor --strict
 ──────────────────────────────────────────────────────────────────────────
  ASL DIAGNOSTIC ENGINE • BARE-METAL LINUX SUBSYSTEM (ARM64)
 ──────────────────────────────────────────────────────────────────────────
  [PASS] Kernel Execution Mode : Native Superuser Chroot (su, uid=0)
  [PASS] SELinux Isolation     : Enforcing (Private namespace bindings)
  [PASS] Subsystem Rootfs      : Debian 13 (Trixie) mounted & hardened
  [PASS] GPU Hardware Node     : Qualcomm Adreno /dev/kgsl-3d0 active
  [PASS] Graphics Driver Stack : Mesa Turnip Vulkan 1.3 + Zink OpenGL 4.6
  [PASS] Display Server IPC    : Termux:X11 (:0) with PulseAudio TCP (4713)
  [PASS] OS Process Safeguard  : Android 12+ PPK Watchdog Disabled (max_phantom=2147483647)
  [PASS] Dynamic DNS Engine    : Auto-sync from Android net.dns* properties
  [PASS] Virtual Swap Pool     : 5.0 GB Active (zRAM + isolated swapfile)
  [PASS] Remote Bridges        : Oracle VPS Relay (2222) + LAN SSH (8022) [ONLINE]
 ──────────────────────────────────────────────────────────────────────────
```

---

## 🛠️ Technical Competencies

| Domain | Technologies & Implementations |
| :--- | :--- |
| **Kernel & Low-Level Systems** | Linux Kernel (4.14+ to 6.x) &bull; ARM64 (aarch64) &bull; Mount Namespaces &bull; Chroot Containerization &bull; SELinux Policy & Enforcing Modes &bull; Android AID Group Mappings &bull; Magisk, KernelSU, APatch Root Architectures |
| **Graphics & Acceleration** | Qualcomm Adreno KGSL (`/dev/kgsl-3d0`) &bull; Mesa Turnip Vulkan 1.3 &bull; Zink (OpenGL-over-Vulkan 4.6) &bull; Termux:X11 Display Server &bull; PulseAudio Low-Latency TCP IPC |
| **Networking & Daemons** | Persistent Reverse SSH Relays &bull; TCP BBR Congestion Control &bull; Android Netd Restrictions Bypass &bull; Serveo & Ngrok Relays &bull; Double-fork Detached Background Daemons |
| **Languages & Toolchains** | C &bull; C++ &bull; POSIX Shell / Bash &bull; Python 3 &bull; Rust &bull; Node.js / TypeScript &bull; Git &bull; Neovim |

---

## 📬 Contact & Links

- **GitHub**: [@Ruusian](https://github.com/Ruusian)
- **Flagship Project**: [Ruusian/ASL](https://github.com/Ruusian/ASL)
- **Email**: [abhiksarkar00@gmail.com](mailto:abhiksarkar00@gmail.com)
