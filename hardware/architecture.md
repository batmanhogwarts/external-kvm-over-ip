# Hardware Architecture

The system consists of an external KVM-over-IP device connected to a target system via HDMI and USB.

## Signal Flow
- HDMI output from target → USB HDMI capture → Raspberry Pi
- USB from Pi → target system (HID emulation)
- Network access via Ethernet or WiFi

## Design Rationale
- USB HDMI capture chosen to avoid custom HDMI PHY design
- Raspberry Pi chosen for availability and Linux support
- Entire system operates externally with no OS modification on target
