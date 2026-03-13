# Changelog

## Added / Improved
- Older **Nano 3** boards are now fully supported.
- Compatibility expanded to support additional **CYD displays**:
  - ST7789
  - ILI9341
- Added **Invert Colours** option.
- Added **Backlight GPIO configuration** (available in setup).
- Minimum **fan speed increased to 15%**.
- **Fan speed adjustment** changed from fixed **5% steps** to **proportional control**.

## Display Options
New setup options to customise the display:

- Show **extended statistics**
- Show **digital clock**
- Show **both (cycling every 3–10 seconds)**

Statistics display includes:
- **Shares Accepted / Rejected**
- **Uptime (days / hours)**

## Touchscreen Configuration
Two new setup options for touch mapping:

- **Flip X**
- **Flip Y**

If the touch input appears **rotated 180° relative to the LCD**, enable **both options**.

## Startup Screen Improvements
Startup screen is now more **verbose** and displays:

- WiFi connection status
- NTP connection status
- License state

Holding the button for **12 seconds** will:

- Clear **WiFi settings**
- Reboot into **setup mode**

All **other settings remain unchanged**.

## Firmware Update Procedure (from 03/03/2026)

- The **GitHub Web Flasher** is intended **for initial installation only**.
- If installing the firmware **for the first time**, use the **Web Flasher linked in the README**.
- After the initial installation, use the **app’s built-in Firmware Updater** for the latest update and all future updates.
- For updates, download **`UpdateOnly.bin`** from the repository and upload it using the **app’s web updater**.
- This method is **simpler** and **preserves all configured data**, including **settings and license information**.

## Bug Fixes

**Issue resolved:**

If the **Nano rebooted**, `Tmax` could become negative due to corrupted data.

- The **CYD** would correctly resync once the Nano reconnected.
- However, the **“-” symbol remained on display** despite the logic restarting correctly.

Fix implemented:
- Adjusted erase width during display refresh to remove the artifact correctly.
