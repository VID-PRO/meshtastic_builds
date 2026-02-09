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
```

Heltec Vision Master e213 with joystick and 2 butttons:

```BUTTON_PIN 48
CANCEL_BUTTON_PIN 47
#TB_UP 42
#define TB_DOWN 45
#define TB_LEFT 46
#define TB_RIGHT 40
#define TB_PRESS 41
```
