
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
