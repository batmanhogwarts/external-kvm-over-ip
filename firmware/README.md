# Firmware Overview

The firmware stack runs on embedded Linux and handles:

- USB HID gadget emulation
- HDMI video capture
- Network streaming
- Web UI

## Components
- Linux USB gadget framework for keyboard/mouse
- v4l2 for HDMI capture
- MJPEG streaming over HTTP (initial prototype)


The firmware runs on a Raspberry Pi CM4 using Raspberry Pi OS Lite.

## Responsibilities:
- HDMI video capture and encoding
- USB HID emulation (keyboard + mouse)
- Browser-based remote access UI
