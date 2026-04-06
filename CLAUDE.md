# CLAUDE.md — bitcoin-resources

> For infrastructure context (hardware, networking, IPs, services) see ~/Git/CLAUDE.md

---

## Repository Overview

Pure documentation repository — no build system, no code, no tests.
A single curated Markdown resource list covering Bitcoin protocol, development,
Lightning Network, wallets, and related tooling.

---

## Structure

```
Bitcoin-Learning-Resources.md   # Main content — organised by topic
README.md                       # Project overview and quick links
```

---

## Contribution Guidelines

- Maintain existing section structure and heading hierarchy
- Each entry: resource name, one-line description, direct URL
- Prefer well-maintained and accurate resources over quantity
- Keep Table of Contents in sync when adding new top-level sections
- Update the "Last Updated" date at the bottom when making changes

---

## Bitcoin Node Context

When adding or verifying resources, the homelab Bitcoin stack for reference:

- **Bitcoin Core v29.3** on nodebox (10.54.30.100, Ubuntu)
  — txindex=1, Tor inbound, outbound via SOCKS5, cookie auth
- **Electrs** — built from source, port 50001, no TLS
- **Mempool.space** — self-hosted block explorer, port 4080
- **Alby Hub** — Lightning via LDK, port 8029
- **Sparrow Wallet** — on Debian, connected to own Electrs
- **Running Bitcoin Knots** by preference (not Core) — relevant when
  resources touch implementation differences, BIP-110, OP_RETURN policy,
  or mempool relay debates

## Bitcoin Knowledge Areas (already covered — avoid duplication)

- UTXO model, mempool mechanics, relay policy vs consensus rules
- BIP activation mechanisms (BIP 9, BIP 8, Speedy Trial, Taproot)
- BIP-110, Core v30 OP_RETURN policy debates
- Post-quantum: BIP-360, ML-DSA (Dilithium), SLH-DSA (SPHINCS+)
- Ordinals, BRC-20, Stamps, Runes — technical mechanisms
- Lightning Network mechanics (LDK, channel management)
- Stateless signing devices (SeedSigner, Krux, Jade), PSBT workflows
- Sparrow Wallet, Electrs, self-hosted infrastructure

---

## License

CC0 1.0 (public domain) — no attribution required.

## Git Remotes

- `origin` → git@github.com:mcps976/bitcoin-resources.git
- `truenas` → truenas:/mnt/tank/git-repos/bitcoin-resources.git
