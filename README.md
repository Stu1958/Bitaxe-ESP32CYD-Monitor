age <p align="left">
  <img src="hero3.png?v=2" width="450"> ;  <img src="inuse.jpg?v=2" width="450">
</p>

# Avalon Nano 3 / 3S Ultra Controller 🚀
### ESP32 Cheap Yellow Display (CYD) monitor and Tmax Temperature controller

Turn your **ESP32-2432S028** into a high-end thermal management hub for your Avalon Nano 3/3S. Protect your ASIC with precision monitoring and real-time stats.

[Quick Install](#-quick-install-trial-mode) | [Buy License Key](#-get-the-full-license-699) | [User Manual](#-user-manual--operational-guide)

---

## 🛡️ Why This Controller? (ASIC Protection)
Standard Avalon firmware often prioritizes "quiet" operation, allowing internal average temperatures to climb as high as **85°C – 95°C**. For 5nm silicon chips, constant high heat is the primary cause of hardware failure and hashrate degradation. 

* **Absolute Peak Monitoring (Tmax):** Monitors the **hottest single chip** in the array. Automatic fan control directly regulates Tmax based on your target temperature.
* Target temperature will be maintained regardless of ambient temperature!
* **The "Longevity" Target:** Dropping operating temps by **10°C** can significantly extend the lifespan of your hardware.
* **Persistent Best Share:** Track your **Best Share** across miner reboots.
* **Dashboard:** Real-time Hashrate (with meter), Work Mode, Best Share (Session/All-time), Target Tmax, and Power in Watts.
* **Touchscreen Control:** On-screen buttons for changing Target Temp and Workmode. Hide/reveal controls with a long press. 

## 🖥️ Required Hardware
Designed specifically for the **ESP32-2432S028-CYD**. 
* **Affordable:** Often found for under $15 / £12 or you may already own one.
* **Universal:** User-configurable for CYD versions with ILI9341 and ST7789 screens. 
* **Vibrant Display:** Nano 3S style circular dashboard for your desk.

## ⚡ Quick Install (Trial Mode)
Test the full interface for free. The trial has full functionality for **60 minutes ** before having to re-enter your data, but you can reset it as many times as you want. License is only $5 or £3.75 giving your Nano 3 / 3S 24/7 unattended protection regardless of ambient temperature.

> **Requirement:** Use Chrome, Edge, or Opera on a Desktop.

1.  **[CLICK HERE TO OPEN THE WEB INSTALLER](https://Stu1958.github.io/Avalon-Nano-Ultra-Controller/)**
2.  Connect your **CYD** via USB.
3.  Click **Install** and select your device port.
4.  Connect to the **NanoCtrl-AP** WiFi (Password: `config123`) to configure.

---

## 🔓 Get the Full License ($5 / £3.75)
Unlock permanent unattended monitoring 24/7.


1.  Flash the **Trial Mode** firmware.
2.  Note your **Device ID** (shown on the setup screen or WiFi Portal).
3.  Send **$5 USD or £3.75 GBP** via PayPal to: `stuart.binns@ntlworld.com`
4.  **⚠️ IMPORTANT:** Include your **Device ID** in the PayPal notes.
5.  Your **License Key** will be emailed (usually within 1 hour).

---

## 📘 User Manual & Operational Guide

### 📶 WiFi Manager Settings
| Setting | Description |
| :--- | :--- |
| **Nano IP** | Local IP of your miner (e.g., `192.168.0.25`) |
| **Target Temp** | Desired Tmax (60-85°C). System constrains to safe ranges. |
| **Previous Best Diff** | Enter your all-time best share (e.g., `2.26G`) |
| **Timezone Offset** | Your UTC offset (e.g., `-5`, `0`, `+1`) |

### 🎮 Pro-Tips
* **Button Response:** The dashboard refreshes every **5 seconds**. Tap a button once and wait for the next refresh to see the change.
* **WiFi reset and hide / Reveal Buttons** Hold anywhere on the central portion of the screen for **6 seconds** to toggle the buttons visibility. Hold for a further 5 seconds to clear the WiFi settings and restart to force Setup. portal.
* Press centre screen for 6 seconds to toggle visibility of Temp target and Mode change buttons - continue holding for a further 5 seconds to reboot and re-enter setup (Only WiFi credentials are erased all other settings retained)
* **Factory Reset:** Hold the physical **BOOT button** (GPIO 0) on the side for **10 seconds** to wipe all settings.

### 🔍 Troubleshooting
* **🔴 Red Status Dot:** Controller cannot reach the Nano IP. Check your network.
* **🔥 Red TMax:** Hottest chip has exceeded your target by **8°C+**.
* **⚠️ Trial Expired:** After 30 mins, the fan defaults to **65%** for safety and the CYD re-boots to setup.

---

### ⚖️ Disclaimer & Liability
> Use at your own risk. While this software includes built-in thermal safeguards, it is provided "as-is." By installing, you agree that:
> * **Hardware Responsibility:** You are responsible for the health of your Avalon Nano and ESP32.
> * **No Liability:** The developer (Stu1958) is not liable for hardware damage, lost profits, or mining downtime.
> * **Environment:** Ambient heat and dust are beyond software control. Monitor equipment during initial setup.

---
*Developed by Stu1958. Proprietary software. All rights reserved.*
