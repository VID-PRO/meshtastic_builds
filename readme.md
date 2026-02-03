# Meshtastic Heltec Wireless Stick lite V2.1 Auto-Builds

This repository automatically builds the **Meshtastic firmware** for the  
**Heltec Wireless Stick lite V2.1** board every night (development branch).

## Downloads
- Go to the [Actions tab](../../actions) → click the latest run → download the `heltec-WSLv2_1-????` artifact.
- Each artifact includes:
  - `firmware.bin`
  - `firmware.factory.bin`
- Or go to releases

## Flashing
Example (Linux/macOS):
```bash
esptool.py --chip esp32 --port /dev/ttyUSB0 write_flash -z 0x0 firmware.factory.bin
