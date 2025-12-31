# USB HID Emulation

The device presents itself to the target system as a standard USB keyboard and mouse.

## Approach
- Linux USB Gadget mode
- HID descriptors for keyboard and mouse
- Input injected via userspace daemon

## Why This Works
Target systems treat the device as a real physical keyboard and mouse, independent of OS.
