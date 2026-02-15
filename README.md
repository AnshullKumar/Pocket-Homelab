
# Pocket Homelab


A personal Linux homelab built on an Android phone using Termux.

This project is focused on learning backend, Linux, and systems fundamentals by running real services under strict constraints (no Docker, no systemd, limited resources).

## Goals
- Understand how backend services actually run
- Learn process management and observability
- Practice Git and documentation as part of development
- Build everything step-by-step

## Current State
- Git initialised and connected to GitHub
- Environment documented
- More services coming next

## Why Termux?
Using Termux removes abstractions and forces understanding of:
- process
- ports
- failures
- supervision

This is intentional.

---

## Milestone: Pocket Remote Homelab Access

This session extended the homelab beyond a single-device experiment into a remotely accessible development environment.

### What Was Built

- Configured an SSH server on the laptop (Windows + WSL).
- Managed firewall rules for secure shell access (port 22).
- Diagnosed client isolation on campus WiFi.
- Implemented a private VPN tunnel using Tailscale (WireGuard-based).
- Established secure remote access from Android (Termux) to the laptop.

### Architecture

Android (Termux)  
→ Encrypted Tailscale tunnel  
→ Windows host  
→ WSL Linux environment  
→ Development tools (Node, Git, Gemini)

### Outcome

Using Tailscale and SSH, the homelab can now be accessed securely from a phone.

This effectively creates a **pocket-accessible homelab**, where the Android device acts as a secure remote terminal while computation runs on the laptop.

### Concepts Reinforced

- SSH enables encrypted remote process execution.
- Firewalls control inbound network traffic.
- Client isolation blocks peer-to-peer communication in managed networks.
- VPN tunneling creates a private overlay network across restrictive environments.
- Remote compute separates execution from interface.

---


