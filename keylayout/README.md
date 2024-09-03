# OUYA key layout files
Input mappings for additional controllers and gamepads.

- `Vendor_054c_Product_09cc.kl`: Sony Playstation 4 controller
- `Vendor_0810_Product_0001.kl`: Dual PSX Adaptor / Twin USB Joystick
  requires the `HID_PANTHERLORD` driver
- `Vendor_18d1_Product_9400.kl`: Google Stadia Controller via USB
- `Vendor_2563_Product_0575.kl`: Retro Fighters Defender (dongle version)
- `Vendor_2dc8_Product_3105.kl`: Google Stadia Controller via 8BitDo USB Wireless adapter 2, using "Dinput mode" (hold "..."+"dpad left" for 3 seconds)


## Installation
Put the desired key mappings into `/system/usr/keylayout/`:
```
$ adb push Vendor_0810_Product_0001.kl /sdcard/
$ adb shell
$ su
$ mount -o remount,rw /system
$ mv /sdcard/Vendor_0810_Product_0001.kl /system/usr/keylayout/
```
