
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

## Networking & Remote Access Layer (Today’s Work: 15th Feb 26)

Today the homelab expanded beyond local experimentation into secure remote access and private networking.

### Concepts Learned
- **SSH (Secure Shell)**  
  Understanding how remote shell sessions work over TCP (port 22), including authentication, encryption handshake, and remote process execution.

- **Firewall Behavior**  
  Learned how inbound rules control traffic and how blocked ports cause connection timeouts.

- **Client Isolation (Campus WiFi)**  
  Discovered that some networks prevent device-to-device communication even on the same subnet, requiring alternative networking strategies.

- **VPN Tunneling (WireGuard via Tailscale)**  
  Implemented a private encrypted overlay network to bypass local network restrictions securely.

- **Remote Compute Model**  
  Understood that SSH does not “move” environments — it executes processes on the remote machine while the local device acts only as input/output.

### Architecture Built

Phone (Termux)  
→ Tailscale encrypted tunnel  
→ Windows host  
→ WSL Linux environment  
→ Development tools (Node, Git, Gemini)

This setup effectively turns the laptop into a private remote development server accessible from anywhere.

### Key Takeaways

- Networking problems are layered (VPN → Firewall → Service → Shell).
- Remote systems depend on service lifecycle (sleep, process state, auto-start).
- Infrastructure should reduce friction, not increase it.


