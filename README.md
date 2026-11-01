# MiniScreen Firmware (OTA Releases)

Precompiled binary distribution repository for the **GeekMagic SmallTV Ultra** (ESP8266 + 240×240 ST7789 TFT).

## Latest Version

* **Current Release**: `v2.2.0`
* **Binary**: [`miniscreen.bin`](https://raw.githubusercontent.com/oh2fxd/miniscreen-fw/main/miniscreen.bin)
* **Metadata**: [`firmware.json`](https://raw.githubusercontent.com/oh2fxd/miniscreen-fw/main/firmware.json)

## Flashing over Network (OTA)

### Web Browser
1. Navigate to `http://<device-ip>/update` on the local network (e.g. `http://192.168.32.209/update`).
2. Upload `miniscreen.bin` and click **Upload & Flash**.

### CLI (curl)
```bash
curl -v -H "Content-Type: application/octet-stream" \
  --data-binary @miniscreen.bin \
  http://<device-ip>/update
```
