# MiniScreen Firmware (OTA Releases)

Precompiled binary distribution repository for **MiniScreen** running on the **GeekMagic SmallTV Ultra** (ESP8266 + 240×240 ST7789 IPS TFT).

## Overview
MiniScreen turns the compact desktop cube display into a real-time home energy and weather HUD, polling Shelly 3EM 3-phase power consumption, Nordpool spot prices, and local weather sensors.

## Latest Version
* **Current Release**: `v2.2.0`
* **Binary**: [`miniscreen.bin`](https://raw.githubusercontent.com/oh2fxd/miniscreen-fw/main/miniscreen.bin)
* **Metadata**: [`firmware.json`](https://raw.githubusercontent.com/oh2fxd/miniscreen-fw/main/firmware.json)
* **Changelog**: [`CHANGELOG.md`](./CHANGELOG.md)

## Flashing over Network (OTA)

### Web Browser
1. Navigate to `http://<device-ip>/update` on the local network (e.g. `http://192.168.32.209/update`).
2. Select `miniscreen.bin` and click **Upload & Flash**.

### CLI (`curl`)
```bash
curl -v -H "Content-Type: application/octet-stream" \
  --data-binary @miniscreen.bin \
  http://<device-ip>/update
```

## License
Distributed under the [MIT License](./LICENSE). Copyright (c) 2026 OH2FXD.
