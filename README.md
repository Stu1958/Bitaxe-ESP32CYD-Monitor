# Avalon Nano 3 / 3S Ultra Controller 🚀
### Precision Thermal Management & Tmax (hotspot) Control runs on cheap ESP32 (CYD)

[![Free Trial](https://img.shields.io/badge/FREE_Trial-Flash_Now-blue?style=for-the-badge&logo=google-chrome)](https://stu1958.github.io/Avalon-Nano-Ultra-Controller/)
[![eBay Shop](https://img.shields.io/badge/Pre--Built-eBay_(UK_Only)-orange?style=for-the-badge&logo=ebay)](https://www.ebay.co.uk/itm/206084391636)
[![License](https://img.shields.io/badge/Full_License-$5_USD-green?style=for-the-badge)](https://www.paypal.com/paypalme/stub1958/5USD)

## ** No cloning required! Use the Free trial Web flasher link above or below! **
<p align="left">
  <img src="hero3.png?v=2" width="450"> &nbsp; <img src="inuse.jpg?v=2" width="450">
</p>

## **Protect your ASIC chips and extend your Nano3's lifespan with precision thermal monitoring.** This project transforms a $15 ESP32-CYD into a professional-grade thermal hub for your Avalon Nano 3/3S. 
## **NEW Update procedure see Update.md for details

---

## 🛡️ Why This Controller? (ASIC Protection)
Standard Avalon firmware often prioritizes "quiet" operation, allowing internal temperatures to climb toward **85°C – 95°C**. For 5nm silicon chips, constant high heat is the primary cause of hardware failure and hashrate degradation.

* **Absolute Peak Monitoring (Tmax):** Monitors the *hottest single chip* in the array. 
* **Stable Temps:** Target temperature is maintained regardless of ambient temperature (within thermal limits)!
* **The "Longevity" Target:** Dropping operating temps by 10°C+ can significantly extend your hardware's lifespan.
* **Persistent Best Share:** Track your Best Share across miner reboots.
* **Dashboard:** Real-time Hashrate (with meter), Work Mode, Best Share, Target Tmax, Shares Accepted / Rejected, Uptime and Power in Watts.
* **Touchscreen Control:** On-screen buttons for changing Target Temp and Workmode.
---

## ⚡ Quick Start (No Cloning Required)
**Test the full interface for free.** The trial offers 100% functionality so you can verify the thermal improvements before you buy.

1.  **Open the [FREE Web Installer](https://stu1958.github.io/Avalon-Nano-Ultra-Controller/)** in Chrome, Edge, or Opera.
2.  Connect your **CYD** via USB and click **Install** folow prompts and flash the CYD in the usual way (hold boot then reset etc)
3.  When installed connect to the **NanoCtrl-AP** WiFi (Password: `config123`) Open a browser to 192.168.4.1 and click Configure WiFi.
4.  Enter your WiFi credentials, Nano name and IP address press save and the CYD will reboot and start managing your Nano's Tmax immediately.
5.  **60-Minute Stress Test:** The controller will manage your Tmax automatically. Reset the trial as many times as you like for continued testing!

### Scroll down for full instructions.
---

## 📦 Choose Your Option

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

## 📘 Full Setup Instruction

When you first power on the device (or after a WiFi reset), it will create an access point for configuration.

## Connecting to Setup

1. **Disable cellular data** on your phone/PC (ensures captive portal works correctly)
2. Connect to WiFi network: **NanoCtrl-AP**
3. Password: **config123**
4. Your browser should automatically open the setup page
5. If not, manually navigate to: **192.168.4.1**

## Configuration Parameters

### Essential Settings

| Parameter | Description | Example |
|-----------|-------------|---------|
| **Miner Name** | Display name for your miner | "Garage Nano" |
| **Nano IP** | IP address of your Avalon Nano 3/3S | 192.168.0.25 |
| **Target Temp C** | Maximum chip temperature (60-85°C) | 70 |
| **Offset from UTC/GMT** | Your timezone offset in hours | 0 (UK), -5 (EST), +1 (CET) |

### Optional Settings

| Parameter | Description | Default |
|-----------|-------------|---------|
| **Previous Best Difficulty** | Import your all-time best share (e.g. 2.26G, 850M) | (empty) |
| **Enable Temp Buttons** | Show temperature control buttons (1=yes, 0=no) | 1 |
| **Enable Mode Buttons** | Show workmode control buttons (1=yes, 0=no) | 1 |
| **License Key** | Leave blank for 1-hour trial mode | (empty) |

### Hardware Settings (Advanced)

**For pre-configured hardware units, these are already set correctly. Only change if display/touch issues occur.**

| Parameter | Description | Default | When to Change |
|-----------|-------------|---------|----------------|
| **Display Driver** | 0=ILI9341, 1=ST7789 | 1 | If display shows garbled/no image |
| **Backlight Pin** | GPIO 21 or 27 | 21 | If backlight doesn't turn on |
| **Color Invert** | 0=normal, 1=inverted | 0 | If colors look negative/reversed |
| **Flip Touch X** | Flip X axis (both=180°) | 0 | If touch is misaligned horizontally |
| **Flip Touch Y** | Flip Y axis (both=180°) | 0 | If touch is misaligned vertically |

### Touch Alignment Issues

If touch input is misaligned (e.g., touching top-right triggers bottom-left):

- **180° rotation**: Set **both** Flip Touch X = 1 **and** Flip Touch Y = 1
- **Horizontal flip only**: Set Flip Touch X = 1, Flip Touch Y = 0
- **Vertical flip only**: Set Flip Touch X = 0, Flip Touch Y = 1

Test each button after saving to verify alignment.

### Licensing

- **Trial Mode**: Leave License Key blank for 1-hour unrestricted trial
- **Licensed Mode**: Enter your license key for unlimited use
- **Device ID**: Read-only field showing your unique hardware identifier (used for license generation)

## After Configuration

1. Click **Save**
2. Device will reboot and connect to your WiFi
3. Display shows boot progress:
   - WiFi Connected
   - License validation (Trial or Licensed)
   - Time sync
   - Connecting to Nano
4. Main gauge display appears

## Troubleshooting

**Cannot access 192.168.4.1:**
- Ensure cellular data/other WiFi is disabled
- Try disconnecting and reconnecting to NanoCtrl-AP
- Manually type the IP address in browser

**Display issues:**
- Try Display Driver = 0 (ILI9341)
- Try Backlight Pin = 27
- Try Color Invert = 1

**Touch not working:**
- Enable both Flip Touch options (set to 1)
- If still wrong, try different combinations

**Cannot connect to Nano:**
- Verify Nano IP address is correct
- Ensure Nano is powered on and on same network
- Check router DHCP hasn't changed Nano's IP

## Resetting WiFi

To reconfigure or clear settings:

- **Touch method**: Hold screen for 10 seconds anywhere
- **Hardware method**: Hold BOOT button for 10 seconds during operation
- Device will clear WiFi and reboot to setup mode
---

## ⚖️ Disclaimer
*Use at your own risk. This software is provided "as-is." The developer (Stu1958) is not liable for hardware damage, lost profits, or mining downtime. Please monitor equipment during initial setup.*

**Developed by Stu1958. Proprietary software. All rights reserved.**
