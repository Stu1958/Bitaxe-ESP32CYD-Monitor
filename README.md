# Avalon Nano 3 / 3S Ultra Controller 🚀
### Precision Thermal Management & Tmax Control runs on cheap ESP32 (CYD)

[![Free Trial](https://img.shields.io/badge/FREE_Trial-Flash_Now-blue?style=for-the-badge&logo=google-chrome)](https://stu1958.github.io/Avalon-Nano-Ultra-Controller/)
[![eBay Shop](https://img.shields.io/badge/Pre--Built-eBay_(UK_Only)-orange?style=for-the-badge&logo=ebay)](https://www.ebay.co.uk/itm/206084391636)
[![License](https://img.shields.io/badge/Full_License-$5_USD-green?style=for-the-badge)](https://www.paypal.com/paypalme/stub1958/5USD)

## ** No cloning required! Use the Free trial Web flasher link above or below! **
<p align="left">
  <img src="hero3.png?v=2" width="450"> &nbsp; <img src="inuse.jpg?v=2" width="450">
</p>

**Protect your ASIC with precision monitoring.** This project transforms a $15 ESP32-CYD into a professional-grade thermal hub for your Avalon Nano 3/3S. 

---

## ⚡ Quick Start (No Cloning Required)
**Test the full interface for free.** The trial offers 100% functionality so you can verify the thermal improvements before you buy.

1.  **Open the [FREE Web Installer](https://stu1958.github.io/Avalon-Nano-Ultra-Controller/)** in Chrome, Edge, or Opera.
2.  Connect your **CYD** via USB and click **Install** folow prompts and flash the CYD in the usual way (hold boot then reset etc)
3.  When installed connect to the **NanoCtrl-AP** WiFi (Password: `config123`) Open a browser to 192.168.4.1 and click Configure WiFi.
4.  Enter your WiFi credentials, Nano name and IP address press save and the CYD will reboot and start managing your Nano's Tmax immediately.
5.  **60-Minute Stress Test:** The controller will manage your Tmax automatically. Reset the trial as many times as you like for continued testing!

---

## 🛡️ Why This Controller? (ASIC Protection)
Standard Avalon firmware often prioritizes "quiet" operation, allowing internal temperatures to climb toward **85°C – 95°C**. For 5nm silicon chips, constant high heat is the primary cause of hardware failure and hashrate degradation.

* **Absolute Peak Monitoring (Tmax):** Monitors the *hottest single chip* in the array. 
* **Stable Temps:** Target temperature is maintained regardless of ambient room heat!
* **The "Longevity" Target:** Dropping operating temps by 10°C+ can significantly extend your hardware's lifespan.
* **Persistent Best Share:** Track your Best Share across miner reboots.
* **Dashboard:** Real-time Hashrate (with meter), Work Mode, Best Share, Target Tmax, and Power in Watts.
* **Touchscreen Control:** On-screen buttons for changing Target Temp and Workmode.

---

## 📦 Choose Your Path

### Option A: DIY License ($5 / £3.75)
Perfect if you already own an ESP32-2432S028. Works on most variants.
1. Flash the firmware via the Web Installer.
2. Note your **Device ID** from the setup screen or WiFi Portal.
3. Send **$5 USD / £3.75 GBP** via [PayPal](https://www.paypal.com/paypalme/stub1958/5USD).
4. **IMPORTANT:** Include your **Device ID** in the PayPal notes. Your key is usually emailed within 1 hour.

### Option B: Plug & Play Hardware (£25) — UK ONLY 🇬🇧
Don't want to flash firmware or source parts? 
* Buy a fully built, licensed, and tested unit on **[eBay](https://www.ebay.co.uk/itm/206084391636)**.
* Includes the hardware and the permanent license pre-installed. 
* **Note:** Shipping to UK addresses only at this time.

---

## 📘 Operational Guide

| Setting | Description |
| :--- | :--- |
| **Nano IP** | Local IP of your miner (e.g., `192.168.0.25`) |
| **Target Temp** | Desired Tmax (60-85°C). System constrains to safe ranges. |
| **Previous Best** | Enter your all-time best share (e.g., `2.26G`) |
| **Timezone** | Your UTC offset (e.g., `-5`, `0`, `+1`) |

### 🎮 Pro-Tips
* **Touch Response:** The dashboard refreshes every **5 seconds**. Tap a button once and wait for the next refresh.
* **Hide Controls:** Long-press (6 seconds) the center of the screen to toggle button visibility.
* **Reset WiFi:** Continue holding (11 seconds total) to wipe WiFi settings and force the Setup portal.
* **Factory Reset:** Hold the physical **BOOT button** (GPIO 0) on the side for 10 seconds to wipe all settings.

---

## 🔍 Troubleshooting
* **🔴 Red Status Dot:** Controller cannot reach the Nano IP. Check your network.
* **🔥 Red TMax:** Hottest chip has exceeded your target by 8°C+.
* **⚠️ Trial Expired:** After 60 mins, the fan defaults to 65% for safety and the CYD re-boots to setup.

---

## ⚖️ Disclaimer
*Use at your own risk. This software is provided "as-is." The developer (Stu1958) is not liable for hardware damage, lost profits, or mining downtime. Please monitor equipment during initial setup.*

**Developed by Stu1958. Proprietary software. All rights reserved.**
