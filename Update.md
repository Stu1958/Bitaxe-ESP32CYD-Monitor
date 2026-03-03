# 🌐 ESP32 Updater User Guide

This interface allows you to update your **Avalon Nano Ultra Controller** wirelessly from your phone or computer.

### 1. Accessing the Updater
*   Ensure your phone or computer is on the same WiFi network as the Controller.
*   In your browser, navigate to: `http://[CONTROLLER_IP]/update`
*   You will see a dark-themed interface with the heading **"Firmware Update"**.

### 2. Selecting the Firmware
*   Click the **"Choose File"** (or "Browse") button.
*   Locate and select the UpdateOnly.bin file you downloaded from the Github files section.
  

### 3. Starting the Update
*   Click the bright yellow **"START UPDATE"** button.
*   **Warning**: Do not close the browser tab or refresh the page while the update is in progress.

### 4. Monitoring Progress
*   **Visual Bar**: A green progress bar will appear and fill from left to right as the file is sent to the ESP32.
*   **Percentage**: A text counter will display the live percentage (0% to 100%).
*   The process typically takes between **15 to 45 seconds** depending on your WiFi signal strength.

### 5. Completion & Reboot
*   When the transfer hits 100%, the browser will display: **"Update Success! Rebooting..."**
*   The CYD screen will go black for a moment as the ESP32 restarts.
*   The device will then boot into your new firmware automatically.

---
**Troubleshooting:**
*   **Button doesn't respond?** Ensure you have selected a file before clicking.
*   **Stuck at 0%?** Check your WiFi connection or try moving closer to the router.

*   **Update Failed?** Refresh the page and ensure you are uploading a valid `.bin` file for the ESP32.

