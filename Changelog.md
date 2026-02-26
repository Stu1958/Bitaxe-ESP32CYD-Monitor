## Changelog

### Added
- Two new setup options for touch mapping:
  - **Flip X**
  - **Flip Y**
  > If touch input appears rotated 180° relative to the LCD, enable both options.

- Startup screen is now verbose and displays:
  - WiFi connection status  
  - NTP connection status  
  - License state  

- 7-second centre screen press toggles button visibility.  
- Holding for 12 seconds clears WiFi settings and reboots into setup  
  *(all other settings are retained)*.

- Compatibility expanded to support additional CYD's:
  - ST7789  
  - ILI9341  
  - Invert colours option  
  - Backlight GPIO configuration (available in setup)

---

### Changed
- Minimum fan speed increased to **15%**.
- Fan speed adjustment changed from fixed **5% step** to **proportional control**.

---

### Fixed
- Minor defect resolved:
  - If the Nano rebooted, `Tmax` could become negative due to corrupt data.
  - The CYD would correctly resync once the Nano reconnected.
  - However, the "-" symbol remained on display despite logic restarting cleanly.
  - Adjusted erase width during redraw to resolve the persistent display artifact.
