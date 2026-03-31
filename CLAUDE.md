# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is a pure documentation repository — no build system, no code, no tests. It contains a single curated Markdown resource list (`Bitcoin-Learning-Resources.md`) and a corresponding `README.md`.

## Structure

- `Bitcoin-Learning-Resources.md` — the main content file; organized into sections by topic (Essential Reading, Official Documentation, Development Resources, Lightning Network, Wallets, etc.)
- `README.md` — project overview and quick links

## Contribution Guidelines

When adding or updating resources:
- Maintain the existing section structure and heading hierarchy
- Each entry should include the resource name, a brief one-line description, and a direct URL
- Prefer well-maintained, accurate resources over quantity
- Keep the Table of Contents in sync if adding new top-level sections
- Update the "Last Updated" date at the bottom of `Bitcoin-Learning-Resources.md` when making changes

## Home Lab Infrastructure

### Network & Security
- **Router:** OPNsense on Protectli VP2420 — runs Suricata IDS, Unbound DNS, HAProxy
- **VPN:** Tailscale for remote access; Mullvad VPN on all devices

### Servers
- **TrueNAS** on Terramaster F4-423 — runs Dockge with the full ARR stack (Sonarr, Radarr, Lidarr, Prowlarr, Jellyfin, Jellyseerr, Audiobookshelf, Homarr), Nextcloud, and SMB shares
- **Bitcoin node** on Beelink (Ubuntu) — runs Bitcoin Core, Mempool.space, and Alby Hub

### Workstations
- **Primary Linux:** Beelink SER running Debian KDE
- **Primary Mac:** MacBook Pro M3 Pro

### Git Remotes
- `origin` — GitHub (mcps976)
- `truenas` — TrueNAS bare repos at `/mnt/tank/git-repos/`

### Scripting Target
Scripts should target **bash 5.x** on Debian/Ubuntu.

## License

CC0 1.0 (public domain) — no attribution required.
