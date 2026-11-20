<div align="center">

# 🌙 MoonClient

**Next-Generation Multi-Platform VPN & Per-App Proxy Client for Windows, Linux, and Android**  
*Powered by Xray-core, sing-box, and ProxyBridge (WinDivert TCP/UDP Engine)*

[![Latest Release](https://img.shields.io/github/v/release/AdamBarfii/MoonClient-Releases?style=for-the-badge&logo=github&label=Latest%20Release&color=00E5FF)](https://github.com/AdamBarfii/MoonClient-Releases/releases/latest)
[![Total Downloads](https://img.shields.io/github/downloads/AdamBarfii/MoonClient-Releases/total?style=for-the-badge&logo=github&label=Downloads&color=10B981)](https://github.com/AdamBarfii/MoonClient-Releases/releases)
[![Windows](https://img.shields.io/badge/Windows%2010%2F11-x64-0078D6?style=for-the-badge&logo=windows&logoColor=white)](https://github.com/AdamBarfii/MoonClient-Releases/releases/latest/download/MoonClient-WPF-win-x64.zip)
[![Android](https://img.shields.io/badge/Android%207.0%2B-ARM64%20%7C%20Universal-3DDC84?style=for-the-badge&logo=android&logoColor=white)](https://github.com/AdamBarfii/MoonClient-Releases/releases/latest)
[![Linux](https://img.shields.io/badge/Linux-x64-FCC624?style=for-the-badge&logo=linux&logoColor=black)](https://github.com/AdamBarfii/MoonClient-Releases/releases/latest/download/MoonClient-Avalonia-linux-x64.zip)

</div>

---

## 📥 Direct Downloads (Latest Release)

All desktop archives are **100% self-contained** — they bundle the `.NET 10` runtime, `Xray-core`, `sing-box`, `Wintun`, `geoip`/`geosite` routing databases, and the `ProxyBridge` kernel driver out of the box. **No extra runtimes required on a fresh PC.**

| Platform | Edition | Architecture | Direct Download | Notes |
| :--- | :--- | :---: | :--- | :--- |
| **Windows 10 / 11** | **MoonClient WPF** *(Recommended)* | `x64` | [**⬇ MoonClient-WPF-win-x64.zip**](https://github.com/AdamBarfii/MoonClient-Releases/releases/latest/download/MoonClient-WPF-win-x64.zip) | Native Windows UI + built-in **ProxyBridge** (TCP/UDP + Discord Voice) |
| **Windows 10 / 11** | **MoonClient Avalonia** | `x64` | [**⬇ MoonClient-Avalonia-win-x64.zip**](https://github.com/AdamBarfii/MoonClient-Releases/releases/latest/download/MoonClient-Avalonia-win-x64.zip) | Cross-platform desktop UI for Windows |
| **Android 7.0+** | **MoonClient Mobile (`arm64-v8a`)** | `ARM64` | [**⬇ Download from Latest Release**](https://github.com/AdamBarfii/MoonClient-Releases/releases/latest) | **Recommended** for all modern Android phones |
| **Android 7.0+** | **MoonClient Mobile (`universal`)** | `All ABIs` | [**⬇ Download from Latest Release**](https://github.com/AdamBarfii/MoonClient-Releases/releases/latest) | Universal APK (`arm64-v8a`, `armeabi-v7a`, `x86`, `x86_64`) |
| **Linux** | **MoonClient Avalonia** | `x64` | [**⬇ MoonClient-Avalonia-linux-x64.zip**](https://github.com/AdamBarfii/MoonClient-Releases/releases/latest/download/MoonClient-Avalonia-linux-x64.zip) | Self-contained Linux desktop build + bundled `xray` |

---

## ✨ What Makes MoonClient Different

### 🖥️ 1. Cosmic Moon Desktop Experience (Windows & Linux)
- **Connect Hero & Live Telemetry**: Instant 1-click **Connect / Disconnect**, real-time ping & jitter tracking, live **Proxy Quality** sparkline graph, and active subscription quota meter.
- **ProxyBridge (Per-App TCP & UDP Routing + Anti-WebRTC)**:
  - Powered by a kernel-level `WinDivert` driver (`ProxyBridge_CLI`), route any Windows app or game by process name (`TCP`, `UDP`, or `BOTH` → `PROXY`, `DIRECT`, or `BLOCK`) through MoonClient's local SOCKS5 (`UDP ASSOCIATE`) tunnel without enabling full-system TUN.
  - **1-Click Discord Voice + Anti-WebRTC Preset**: Routes `Discord.exe` TCP signaling and UDP voice media streams through the VPN while preventing browser WebRTC UDP leaks (`Chrome`, `Edge`, `Brave`, `Firefox`, `Opera`, `Vivaldi`, `Arc`).
- **Structured Console & One-Click Diagnostics**: Color-coded live log viewer (`Log`, `Statistics`, `Proxy Info`), regex/keyword filtering, and one-click diagnostic bundle export.
- **Unified Status Bar & System Tray**: Instant two-way sync between the bottom status bar and system tray for **System Proxy** (`Clear` / `Set` / `Unchanged` / `PAC`), **Smart Routing** (`Bypass Iran & China`), and **TUN Mode**.

### 📱 2. Flagship Android VPN Experience (Jetpack Compose Material 3)
- **4-Tab Consumer VPN Interface**:
  - **Home**: Animated **Connect Orb** with pulsing status rings, live session timer, latency badge, 1-tap **Fastest Server** selector, and real-time cross-process download/upload speed + quota card.
  - **Locations**: Clean country flag server cards, signal-strength bars, color-coded ping (`ms`), protocol tags (`VLESS`, `XHTTP`, `REALITY`, `Hysteria2`), and subscription group filters.
  - **Account**: Optional 1-tap **Telegram Bot Login** & **QR Code Login** to sync MoonVPN subscriptions, data usage, and wallet balance — plus **Access Pass Studio** to share guest QR passes.
  - **Settings**: Categorized cards for **Per-App Split Tunneling**, **Routing Rules**, **Speed / Mux & TLS Fragment Optimizer**, **Protection & LAN/Hotspot Sharing**, and **In-App Updates**.

### 🎟️ 3. Access Pass Studio (Owner-Controlled Subscription Sharing)
- Create custom guest **QR Access Passes** or share codes directly from Desktop or Android.
- Set per-guest **Data Caps (GB)**, **Expiration Timers**, and **Device Limits (`1–20`)**.
- Monitor live guest usage and **Pause, Resume, or Revoke** any shared pass instantly.

### 🔓 4. Open & Flexible (Custom Configs + Optional MoonVPN Sync)
- Use MoonClient as a **standalone universal VPN client** with any custom share link, QR code, or subscription URL (`VLESS`, `VMess`, `Trojan`, `Hysteria2`, `Shadowsocks`, `WireGuard`, `TUIC`, `Socks`, `HTTP`), **or** link your MoonVPN Telegram account for automatic cloud syncing.

---

## 🚀 Quick Start Guide

### Windows
1. Download [**`MoonClient-WPF-win-x64.zip`**](https://github.com/AdamBarfii/MoonClient-Releases/releases/latest/download/MoonClient-WPF-win-x64.zip) and extract it to any folder (e.g. `C:\MoonClient`).
2. Run **`MoonClient.exe`** *(run as Administrator if you plan to use **TUN Mode** or **ProxyBridge**)*.
3. Import your servers via **Clipboard (`Ctrl+V`)**, **QR Scan**, **Subscription URL**, or click **MoonVPN** in the sidebar to sign in with Telegram.
4. Select a server (or click **⚡ Fastest**) and click **Connect**.
5. **For Discord Voice / Per-App Gaming**: Open **ProxyBridge** in the sidebar → click **Discord Voice + Anti-RTC** (or select your apps/games) → click **Apply ProxyBridge**.

### Android
1. Download **`v2rayNG_<version>_arm64-v8a.apk`** from the [**Latest Release**](https://github.com/AdamBarfii/MoonClient-Releases/releases/latest) and install it.
2. Open **MoonClient**, import a config/subscription in **Locations** (or link your Telegram account in **Account**).
3. Tap the central **Connect Orb** on the **Home** tab, or tap **⚡ Fastest Server** to automatically benchmark and connect to the lowest-latency node.

### Linux
1. Download [**`MoonClient-Avalonia-linux-x64.zip`**](https://github.com/AdamBarfii/MoonClient-Releases/releases/latest/download/MoonClient-Avalonia-linux-x64.zip) and extract:
   ```bash
   unzip MoonClient-Avalonia-linux-x64.zip -d MoonClient
   cd MoonClient/MoonClient-Avalonia
   chmod +x MoonClient bin/xray/xray
   ./MoonClient
   ```

---

## 🔄 In-App Auto-Updater

MoonClient includes a built-in updater linked directly to this repository (`AdamBarfii/MoonClient-Releases`):
- **Windows / Linux**: Click the **Update (`↻`)** button in the top hero bar (or open **Settings → Check for Updates**) to automatically download and apply the latest release via `AmazTool`.
- **Android**: Open **Settings → Check for Updates** to check and download the newest signed APK.

---

<div dir="rtl" align="right">

## 🇮🇷 راهنمای سریع فارسی (MoonClient)

**MoonClient** یک کلاینت نسل جدید، سریع و کامل برای **ویندوز، اندروید و لینوکس** است که هسته‌های `Xray-core`، `sing-box` و موتور تفکیک ترافیک `ProxyBridge` را به صورت یکپارچه و بدون نیاز به نصب هیچ پیش‌نیازی در اختیار شما قرار می‌دهد.

### امکانات کلیدی:
- **ظاهر مدرن Cosmic Moon در ویندوز و اندروید**: اتصال تک‌کلیدی، نمایش لحظه‌ای کیفیت اتصال (`Proxy Quality`)، سرعت دانلود/آپلود و حجم باقی‌مانده اشتراک.
- **قابلیت ProxyBridge در ویندوز (مخصوص دیسکورد و بازی‌ها)**: هدایت ترافیک `TCP` و `UDP` برنامه‌های انتخابی از طریق VPN بدون نیاز به روشن کردن TUN کل سیستم + پیش‌تنظیم **Discord Voice + Anti-WebRTC** برای رفع کامل مشکل `RTC Connecting` در ویس دیسکورد.
- **انتخاب هوشمند سریع‌ترین سرور (⚡ Fastest Server)** و بهینه‌ساز **TLS Fragment & Mux** برای عبور از محدودیت‌های اینترنت ایران (همراه اول، ایرانسل، مخابرات و فیبر نوری).
- **استودیو اشتراک‌گذاری (Access Pass Studio)**: ساخت کارت دعوت QR با محدودیت حجم، زمان و تعداد دستگاه برای دوستان و خانواده با قابلیت توقف یا لغو آنی.
- **پشتیبانی همزمان از کانفیگ‌های شخصی و حساب تلگرام MoonVPN**: امکان افزودن هرگونه لینک سابسکریپشن یا کانفیگ شخصی، یا اتصال یک‌کلیدی به ربات تلگرام جهت همگام‌سازی خودکار.

</div>
