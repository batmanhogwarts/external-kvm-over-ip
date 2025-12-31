# External KVM-over-IP Device

## Overview
This project is an external, hardware-based KVM-over-IP device that enables
remote keyboard, mouse, and display access to computers without native remote
access support.

The system operates entirely externally using HDMI video capture and USB HID
emulation, without modifying or interacting with the target system’s operating
system.

A Chromebook is used as the primary test platform due to its limited native
remote access capabilities.

## System Architecture
The device consists of:
- HDMI capture input from the target system
- USB HID emulation (keyboard + mouse)
- Raspberry Pi Compute Module 4
- Ethernet/WiFi network interface
- Browser-based remote access UI

A block diagram is provided in `hardware/block-diagram.png`.

## Current Project Status
This project is currently in the **prototype design phase**.

Completed so far:
- System architecture planning
- Hardware component selection
- Initial block diagrams
- Repository structure for hardware, firmware, PCB, and CAD

Next steps:
- Firmware development for USB HID emulation
- HDMI capture configuration
- PCB design for CM4 carrier board
- Enclosure CAD design

## Goals
- Learn how hardware KVM-over-IP systems operate at a low level
- Implement HDMI capture and network streaming
- Emulate USB HID devices using embedded Linux
- Document the full build process and limitations

## Funding Request
Funding will be used to purchase:
- CM4-based KVM board
- HDMI capture hardware
- Power and networking components
- Cables and accessories

Estimated budget and BOM are documented in `hardware/bom.md`.
