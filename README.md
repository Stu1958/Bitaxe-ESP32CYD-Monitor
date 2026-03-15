<h1 align="center">Avalon Nano 3 / 3S Ultra Controller 🚀</h1>
<h3 align="center">Precision Thermal Management & Tmax (hotspot) Control runs on cheap ESP32 (CYD)</h3>

[![Free Trial](https://img.shields.io/badge/FREE_Trial-Flash_Now-blue?style=for-the-badge&logo=google-chrome)](https://stu1958.github.io/Avalon-Nano-Ultra-Controller/)
[![eBay Shop](https://img.shields.io/badge/Pre--Built-eBay_(UK_Only)-orange?style=for-the-badge&logo=ebay)](https://www.ebay.co.uk/itm/206126149086)
[![License](https://img.shields.io/badge/Full_License-$5_USD-green?style=for-the-badge)](https://www.paypal.com/paypalme/stub1958/5USD)

## **No cloning required! Use the Free trial Web flasher link above or below!**
<p align="left">
  <img src="main.gif?v=2" width="400"> &nbsp; 
  <img src="inuse.jpg?v=2" width="400"> &nbsp;
</p>

---

## 🛡️ Protect Your ASIC Chips — Extend Your Nano 3 / 3S Lifespan

Standard Avalon firmware often prioritizes "quiet" operation, allowing temperatures to reach **85°C – 95°C**.  
For 5nm silicon, **constant high heat is the primary cause of degradation and hardware failure**.  

This project transforms a $15 ESP32-CYD into a **professional-grade 24/7 thermal management hub** for your Avalon Nano 3/3S.  

> 🔒 **Set-and-Forget Operation**  
> 📉 **Reduce Operating Temps by 10°C+**  
> ⏳ **Extend ASIC Lifespan**  

---
## 🔥 Key Features

* **Tmax Thermal Control:** Actively monitors the *hottest ASIC chip* and maintains a target temperature regardless of ambient conditions.  
* **Reduce ASIC Temps:** Typically lowers peak chip temperatures by **10°C+**.  
* **Per-ASIC Diagnostics:** Monitor **all 12 ASIC chips individually** (temperature, voltage, throttling status).  
* **Persistent Best Share:** Keeps track across miner reboots.  
* **Real-Time Dashboard:** Hashrate meter, Work Mode, Best Share, Target Tmax, Shares Accepted/Rejected, Uptime, Power usage.  
* **Touchscreen Controls:** Adjust Target Temperature and Work Mode directly on the CYD display.  
* **Web Interface:** Access diagnostics and controls from any phone or PC browser.  

---

## 🆕 New: Web interface-Easy Updates-System control-ASIC monitor

After the initial flash from GitHub, the CYD now hosts a **built-in web updater**:

* Update firmware from any phone or PC browser  
* Upload `.bin` file directly over your network!
* No USB connection needed no fiddly holding Boot / Reset etc.
* Retains all license and configuration data  
* Takes 15–45 seconds depending on WiFi  
---
<p align="left">

  <img src="Asic.png?v=2" width="400"> &nbsp;
</p>

## 🔬 Per-ASIC Monitoring & Diagnostics

The Ultra Controller now includes **full per-chip status** for the Avalon Nano.

View detailed information for **all 12 ASIC chips** directly from the built-in web interface.

### Live ASIC Data

| Field | Description |
|------|-------------|
| ID | Chip number (0-11) |
| Temp | Individual chip temperature |
| Voltage | Operating voltage (mV) |
| Delta | Voltage difference from baseline |
| Status | OK / OPTIMISED / PROTECTED |

### Color Status Indicators

🟢 **OK**  
Chip operating normally.

⚪ **Optimised**  
Chip has reached thermal or voltage limits  
(≥68°C or ≥10 mV delta).

🔴 **Protected**  
Firmware heavily limiting the chip  
(≥15 mV delta).

This allows you to quickly identify:

* weak ASIC chips
* thermal imbalance
* voltage instability
* early hardware degradation---

## ⚡ Quick Start (No Cloning Required)

The **trial is 100% functional**, but resets every **60 minutes**.  
This proves the system works — the license unlocks **true 24/7 protection**.

### Steps:

1. Open the **[FREE Web Installer](https://stu1958.github.io/Avalon-Nano-Ultra-Controller/)** in Chrome, Edge, or Opera.  
2. Connect your **CYD** via USB and click **Install**. Follow prompts (hold BOOT + RESET if needed).  
3. Connect to **NanoCtrl-AP** WiFi (`config123`). Open browser → `192.168.4.1`.  
4. Enter:
   * WiFi credentials  
   * Nano name  
   * Nano IP  
   * Target Tmax  
5. Click **Save** → Device reboots and begins managing Tmax.
### ⚡ **For the latest features after the initial flash download UpdateOnly.bin and use the app's own firmware updater**
#### Much easier, flashes over WiFi, no USB connection required, no pressing boot buttons, reset etc!

### 60-Minute Stress Test

Trial manages Tmax automatically.  
Reset as many times as needed.  
For permanent 24/7 protection, enter your **license key**.

---

## 📦 Choose Your Option

### 🧩 Option A: DIY License ($5 / £3.75)

Perfect if you already own an ESP32-2432S028 (CYD).  

**Steps:**

1. Flash firmware via Web Installer  
2. Note **Device ID** from setup page  
3. Pay **$5 USD / £3.75 GBP** via [PayPal](https://www.paypal.com/paypalme/stub1958/5USD)  
4. **Include Device ID in PayPal notes** — license emailed within 1 hour  

✅ Unlocks true 24/7 operation and set-and-forget ASIC protection.

---

### 🔌 Option B: Plug & Play Hardware (£25 — UK ONLY 🇬🇧)

Don’t want to flash firmware or source parts?  

* Buy fully assembled, licensed, tested unit on **[eBay](https://www.ebay.co.uk/itm/206126149086)**  206126149086
* Hardware + permanent license included  
* Ready to deploy  
* UK shipping only

---

## 📘 Full Setup Instructions

First power-on (or WiFi reset) → device creates **NanoCtrl-AP** network.

### Connecting to Setup

1. Disable cellular data  
2. Connect to WiFi: **NanoCtrl-AP**  
3. Password: `config123`  
4. Browser auto-opens → If not, enter: `192.168.4.1`

---

### Configuration Parameters

**Essential**

| Parameter | Description | Example |
|-----------|-------------|---------|
| Miner Name | Display name | Garage Nano |
| Nano IP | Nano IP | 192.168.0.25 |
| Target Temp C | Max chip temp | 70 |
| Offset from UTC/GMT | Timezone | 0 (UK), -5 (EST), +1 (CET) |

**Optional**

| Parameter | Description | Default |
|-----------|-------------|---------|
| Previous Best Difficulty | Import all-time best | (empty) |


| License Key | Leave blank for trial | (empty) |
|-----------|-------------|---------|

**Advanced Hardware Settings**

| Parameter | Default | Change If |
|-----------|---------|------------|
| Display Driver | 1 (ST7789) | Garbled/no image |
| Backlight Pin | 21 | Backlight off |
| Color Invert | 0 | Colors reversed |
| Flip Touch X | 0 | Touch misaligned X |
| Flip Touch Y | 0 | Touch misaligned Y |

**Touch Alignment Quick Fix**

- 180° rotation → Flip X=1 **and** Flip Y=1  
- Horizontal flip → Flip X=1 only  
- Vertical flip → Flip Y=1 only  

---

## 🔐 Licensing

**Trial Mode:** Fully functional, resets every 60 mins.  
**Licensed Mode:** Unlimited runtime, true 24/7 protection.  

Device ID required for license.

---

## 🔄 Resetting WiFi

**Touch:** Hold screen 10s  
**Hardware:** Hold BOOT 10s  
→ Reboots into setup (other settings retained)

---

## 🛠 Troubleshooting

- **Cannot access 192.168.4.1:** Disable mobile data, reconnect, or manually enter IP  
- **Display issues:** Try Display Driver=0, Backlight=27, Color Invert=1  
- **Touch issues:** Enable Flip options  
- **Cannot connect to Nano:** Verify IP, power, router DHCP

---

## ⚖️ Disclaimer

Use at your own risk.  
Provided “as-is.” Stu1958 not liable for damage, downtime, or lost profits.

---

**Developed by Stu1958**  
Proprietary Software — All Rights Reserved


