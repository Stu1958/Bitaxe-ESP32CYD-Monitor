# Changelog

## Core Improvements
- Full **Nano 3 & Nano 3S** support (auto-detects model)
- **Unified gentle PID fan control**
- **Model-aware gauge scaling**
- **Professional clean web interface** (mobile responsive)
- **Alternating PING display** *(3S only)*
- **All WiFiManager settings persist**
- **WiFi auto-reconnect**
- **String-based best share handling** (prevents overflow)
- **Model-specific reboot commands**

## Hardware Support
- Older **Nano 3** boards are now fully supported
- Compatibility expanded for additional **CYD displays**:
  - **ST7789**
  - **ILI9341**

## System Improvements
- Added **Invert Colours** option
- Added **Backlight GPIO configuration** (available in setup)
- **Minimum fan speed increased to 15%**
- **Fan speed control changed from fixed 5% steps to proportional control**

## Display Options
New setup options allow custom display modes:

- Show **extended statistics**
- Show **digital clock**
- Show **both** (automatically cycles every **3–10 seconds**)

Statistics display includes:
- **Shares Accepted / Rejected**
- **Uptime (days / hours)**

## Touchscreen Configuration
New setup options for correcting touchscreen orientation:

- **Flip X**
- **Flip Y**

If the touch input appears **rotated 180° relative to the LCD**, enable **both options**.

## Startup Screen Improvements
The startup screen is now more **verbose** and displays:

- **WiFi connection status**
- **NTP connection status**
- **License state**

Holding the button for **12 seconds** will:

- Clear **WiFi settings**
- Reboot into **setup mode**

All **other settings remain unchanged**.

## Firmware Update Procedure (from 03/03/2026)

- The **GitHub Web Flasher** is intended **for initial installation only**
- For **first-time installation**, use the **Web Flasher linked in the README**
- After installation, use the **app’s built-in Firmware Updater** for the latest and all future updates
- Download **`UpdateOnly.bin`** from the repository and upload it using the **app’s web updater**

This method is **simpler** and **preserves all configured data**, including:
- Settings
- License information

## Bug Fixes

### Fixed
**Tmax display corruption after Nano reboot**

- If the **Nano rebooted**, `Tmax` could become **negative due to corrupted data**
- The **CYD** would correctly resync once the Nano reconnected
- However, a **“–” symbol could remain on the display** even though the logic had restarted correctly

**Resolution**
- Adjusted **erase width during display refresh** to properly clear the artifact
