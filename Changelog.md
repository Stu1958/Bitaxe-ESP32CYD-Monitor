# Changelog

## Core Improvements
- Most frequently accessed settings now moved to Web page. These can be changed on the fly without rebooting to setup. (Beta)
- Added Work Mode scheduling for those who have off peak electricity tariff's. (Beta)
- Full **Nano 3 & Nano 3S** support *(auto-detects model)*
- **Unified gentle PID fan control** for smoother temperature regulation
- **Model-aware hashrate gauge scaling**
  - **7 TH/s** for Nano **3S**
  - **5 TH/s** for **Nano 3**
- **Model-specific reboot commands**
- **String-based best share storage** (supports values >4.29G without overflow)

## Web Interface
- **Professional web interface** with clean utility-style buttons
- Fully **mobile responsive design**
- **Web-based ASIC Status page**
  - View **individual chip temperatures, voltages, and status**
  - Accessible directly from a web browser
- **Enhanced ASIC Status styling**
  - Gradient headers
  - Color-coded temperature ranges *(green / yellow / orange / red)*
  - Status icons *(✓ / ⚡ / 🛡)*
- **ASIC Status auto-refresh** *(updates every 5 seconds)*
- **Live chip monitoring**
  - Real-time voltage delta detection
  - Firmware thermal management alerts
- **Optional TMax ± controls** on ASIC Status page *(toggle via WiFiManager)*

## System & Connectivity
- **WiFi auto-reconnect** after network drops
- **All WiFiManager settings persist** and pre-populate on restart
- **Dual RSSI display**
  - Shows **Nano WiFi signal**
  - Shows **CYD WiFi signal**
  - Each with independent colour coding

## Hardware & Display Support
- Full compatibility with additional **CYD displays**:
  - **ST7789**
  - **ILI9341**
- Added **Invert Colours** option
- Added **Backlight GPIO configuration** *(available in setup)*

## Display & UI Options
New setup options allow customisation of the display:

- **Extended statistics display**
- **Digital clock**
- **Combined mode** *(cycles between stats and clock)*

Additional display controls:

- **Optional clock toggle** *(clock or data-only mode)*
- **Configurable centre display cycle time** *(5–60 seconds)*

Statistics display includes:
- **Shares Accepted / Rejected**
- **Uptime (days / hours)**
- **Nano → Pool ping display**
  - Alternates with uptime on **Nano 3S**
  - Dedicated **Stats2 display on Nano 3**

## Touchscreen Configuration
Two new setup options for touch orientation correction:

- **Flip X**
- **Flip Y**

If the touch input appears **rotated 180° relative to the LCD**, enable **both options**.

## Power & Cooling
- **Minimum fan speed increased to 15%**
- **Fan control improved**
  - Replaced fixed **5% step control**
  - Now uses **smooth proportional PID control**

## Screen Behaviour
- **Screen timeout / stealth mode**
  - Display automatically dims after a configurable time
  - **Double-tap to enter sleep mode**

## Startup Screen Improvements
Startup screen is now more **verbose** and displays:

- **WiFi connection status**
- **NTP connection status**
- **License state**

Holding the button for **12 seconds** will:

- Clear **WiFi settings**
- Reboot into **setup mode**

All **other settings remain unchanged**.

## Licensing / Trial Mode
- Added **Trial Mode**
  - **1 hour unrestricted use**
  - After expiry, **fake chip data is displayed**

## Firmware Update Procedure (from 03/03/2026)

- The **GitHub Web Flasher** is intended **for initial installation only**
- For **first-time installation**, use the **Web Flasher linked in the README**
- After installation, use the **app’s built-in Firmware Updater** for the latest and all future updates
- Download **`UpdateOnly.bin`** from the repository and upload it using the **app’s web updater**

This method is **simpler** and **preserves all configured data**, including:

- Settings
- License information

## Bug Fixes

### Fixed – Tmax Display Corruption
If the **Nano rebooted**, `Tmax` could become **negative due to corrupted data**.

- The **CYD** would correctly resync once the Nano reconnected
- However, a **“–” symbol could remain on the display** even though logic restarted correctly

**Resolution**
- Adjusted **erase width during display refresh** to properly clear the artifact.
