# Avalon Nano 3S Health Monitor

No installation required other than **Python 3**.

If this tool was helpful, you can buy me a coffee or make a small donation:
[Buy me a coffee](https://www.paypal.com/paypalme/stub1958)

---

## Requirements

- Python **3.x**
- Network access to the Nano miner

Most **Linux** and **macOS** systems already include Python.  
**Windows** users may need to install it.

---

## Running the Monitor

Open a terminal / command prompt in the folder containing `nano_monitor.pyc`.

### Windows

```bash
python nano_monitor.pyc 192.168.0.25
```

### macOS / Linux

```bash
python3 nano_monitor.pyc 192.168.0.25
```

Replace `192.168.0.25` with the IP address of your **Nano 3 / 3S**.

---

## Open the Web Interface

Once running, open your browser and go to:

```
http://localhost:8080
```

You can also access it from other devices on your network using:

```
http://<your-computer-ip>:8080
```

---

## Notes

- The monitor runs **entirely locally**
- **No internet connection** is required

- It **does not modify miner settings** — it only reads statistics
