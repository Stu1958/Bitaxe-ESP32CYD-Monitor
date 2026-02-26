# WiFiManager Configuration Guide

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
