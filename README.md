<p align="center">
  <img src="hero.png" width="450">
</p>

# Avalon Nano Ultra Controller 🚀
The professional touchscreen companion for your Avalon Nano 3/3S. Protect your ASIC with precision thermal management and high-fidelity real-time stats.

[Quick Install](#-quick-install-trial-mode) | [Buy License Key](#-get-the-full-license-5) | [User Manual](#-user-manual--operational-guide)

---

## 🛡️ Why This Controller? (ASIC Protection)
Standard Avalon firmware often prioritizes "quiet" operation, allowing internal temperatures to climb as high as **85°C – 95°C**. For 5nm silicon chips, constant high heat is the primary cause of hardware failure and hashrate degradation. 

* **Absolute Peak Monitoring (Tmax):** We monitor the **hottest single chip** in the array. If one chip spikes, our controller reacts instantly.
* **The "Longevity" Target:** We default to a **65°C thermal target**. Dropping operating temps by **10°C** can significantly extend the lifespan of the silicon.
* **Persistent Analytics:** Track your **Best Share** and total hashrate performance visible on your desk 24/7.
* **Custom UI:** A premium circular dashboard designed specifically to complement the Avalon Nano aesthetic.

---

## ⚡ Quick Install (Trial Mode)
Test the full interface for free. The trial functions for 30 minutes per boot. 
> **Requirement:** Use Chrome, Edge, or Opera on a Desktop.

1. **[CLICK HERE TO OPEN THE WEB INSTALLER](https://Stu1958.github.io/Avalon-Nano-Ultra-Controller/)**
2. Connect your **ESP32-2432S028-CYD** via USB.
3. Click **Install** and select your device.
4. Once finished, connect to the **NanoCtrl-AP** WiFi network (Password: `config123`) to configure.
---

## 🔓 Get the Full License ($6.99)
To unlock permanent monitoring and remove the 30-minute trial timer:

1. Flash the **Trial Mode** firmware below.
2. Note your **Device ID** (displayed on the CYD setup screen or in the WiFi Portal).
3. Send **$6.99** via PayPal to: **stuart.binns@ntlworld.com**
4. **Important:** Include your **Device ID** in the PayPal payment notes.
5. Your unique **License Key** will be emailed to you (usually within 1 hour).
---

## 📘 User Manual & Operational Guide

### 📶 WiFi Manager Settings
When the portal opens, configure these fields for the best experience:
* **Nano IP:** The local IP of your miner (e.g., `192.168.0.25`).
* **Target Temp (60-85):** Desired heat in Celsius. The system automatically **constrains** inputs to this safe range.
* **Previous Best Diff:** Enter your all-time best share (e.g., `2.26G`) to resume your stats.
* **Timezone Offset:** Your UTC/GMT offset (e.g., `-5`, `0`, `+1`) for the clock.
* **Enable Buttons:** Set to `1` for active touchscreen controls, or `0` to lock them.

### 🎮 Pro-Tips for Savvy Miners
* **Button Response:** The dashboard refreshes every **5 seconds**. Tap a button (T+/M+) once and wait for the next refresh cycle to see the change.
* **Dynamic Fan Control:** The controller hunts for your target temp, adjusting the fan by **5%** every 5 seconds until the target is met.
* **The "Secret" Reset:** Need to change WiFi? Press and hold **anywhere on the screen for 3 seconds** to reboot into the configuration portal.
* **Hardware Factory Reset:** Hold the physical **BOOT button** (GPIO 0) on the side of the ESP32 for **10 seconds** to wipe all settings.

### 🔍 Troubleshooting & Alerts
* **🔴 Red Status Dot:** The controller cannot reach the Nano IP. Check your network or IP address.
* **🔥 Flashing TMax:** Your hottest chip has exceeded your target temperature by **8°C or more**.
* **⚠️ Trial Expired:** If you haven't entered a license, the fan will set to **65%** for safety and the screen will lock after 30 minutes.

---
*Developed by Stu1958. Proprietary software. All rights reserved.*
