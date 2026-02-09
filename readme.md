# Meshtastic  Auto-Builds

This repository automatically builds the **Meshtastic firmware** for special boards every night.

## Downloads
- Go to the [Actions tab](../../actions) → click the latest run for the desired booard → download the artifact.
- Each artifact includes:
  - `firmware.bin`
  - `firmware.factory.bin`

## Flashing
Example (Linux/macOS):
```bash
esptool.py --chip esp32 --port /dev/ttyUSB0 write_flash -z 0x0 firmware.factory.bin
```
Example (Windows):  

got to:
https://esptool.spacehuhn.com/  
Click connect and follow the prompts.

# Heltec WIreless Stick lite v2.1

needed because not in the official repo.  

# Heltec Vision Master e213 with joystick and 2 butttons:

## Pin declaration

| **ACTION** | **PIN** |
|:-:|:-:|
| BUTTON | 48 |
| CANCEL | 47 |
| UP | 42 |
| DOWN | 45 |
| LEFT | 46 |
| RIGHT | 40 |
| PRESS | 41 |
