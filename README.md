# External KVM-over-IP Device

## Overview
This project documents the design of an external, hardware-based KVM-over-IP device
that enables remote keyboard, mouse, and display access to systems without native
remote access.

The system works entirely externally using HDMI video capture and USB HID emulation,
without modifying the target system’s operating system.

A Chromebook is used as the test platform due to its limited native remote access
capabilities.

## Goals
- Learn how hardware KVM-over-IP systems work at a low level
- Capture HDMI video and stream it over a network
- Emulate USB HID devices (keyboard and mouse)
- Access the system remotely via a web interface
- Keep the design external and non-invasive

## System Architecture
- Target device: Chromebook
- Video input: HDMI
- Input emulation: USB HID
- Controller: Raspberry Pi CM4 (or equivalent)
- Network: Ethernet / Wi-Fi
- Remote access: Web-based viewer

## Status
This repository currently contains design documentation and planning.
Firmware and configuration files will be added as the project progresses.
