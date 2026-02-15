
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

