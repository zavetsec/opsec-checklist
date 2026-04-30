# ZavetSec OPSEC Checklist

<div align="center">

![Version](https://img.shields.io/badge/version-2.0-00ff88?style=flat-square&labelColor=0a0d10)
![Language](https://img.shields.io/badge/language-RU%20%2F%20EN-00ff88?style=flat-square&labelColor=0a0d10)
![License](https://img.shields.io/badge/license-MIT-00ff88?style=flat-square&labelColor=0a0d10)
![Categories](https://img.shields.io/badge/categories-12-00ff88?style=flat-square&labelColor=0a0d10)
![Items](https://img.shields.io/badge/items-68-00ff88?style=flat-square&labelColor=0a0d10)
![Offline Ready](https://img.shields.io/badge/offline-ready-00ff88?style=flat-square&labelColor=0a0d10)
![No Tracking](https://img.shields.io/badge/tracking-none-00ff88?style=flat-square&labelColor=0a0d10)

**A self-contained OPSEC assessment framework for individuals operating under real-world surveillance, censorship, and targeted threat conditions — designed for Russian and CIS operational environments.**

[🇷🇺 Русская версия](index.html) · [🇬🇧 English version](index.en.html) · [Live demo →](https://zavetsec.github.io/opsec-checklist)

</div>

---

![ZavetSec OPSEC Checklist Preview](docs/preview.png)

---

## Why this exists

Most security advice assumes Western infrastructure, services, and threat models. This project exists because OPSEC guidance should reflect the legal, technical, and surveillance realities users actually operate under — not a generic baseline written for a different threat landscape.

## What is this

Most OPSEC checklists are generic. This one isn't.

68 actionable items across 12 categories, built specifically for the Russian and CIS threat environment: SORM wiretapping infrastructure, DPI-based blocking (ТСПУ), SIM-swap via carrier stores, and regional service availability. Each item includes a threat description explaining *why* it matters and a step-by-step implementation guide with specific tools and commands.

Select a threat model profile to prioritize items relevant to your situation. Track progress. Export a report. Share a link to any specific item.

## Categories

| # | Category | Items |
|---|----------|-------|
| 01 | Digital Identity & Anonymity | 7 |
| 02 | Threat Modeling | 2 |
| 03 | Devices & Physical Security | 10 |
| 04 | Network & Traffic | 6 |
| 05 | Communications & Messengers | 6 |
| 06 | Data & Storage | 6 |
| 07 | Social Engineering & Phishing | 6 |
| 08 | Browser & Web Privacy | 3 |
| 09 | Digital Footprint & De-anonymization | 5 |
| 10 | Financial OPSEC | 3 |
| 11 | Travel Security & Border Crossing | 4 |
| 12 | Incident Response & Canary Tokens | 4 |

## Features

- **Threat model profiles** — select *Privacy* or *Full Anonymity* to highlight relevant items
- **Progress tracking** — state saved locally in browser, survives page reload
- **Search** — full-text search across all items (Ctrl+F)
- **Export** — generate a standalone HTML report of current state
- **Deep links** — direct link to any individual item via anchor
- **Print-friendly** — clean print stylesheet included
- **Zero dependencies** — single self-contained HTML file, no external requests\*

> \* Except Google Fonts loaded at render time. For fully offline use, the font import can be removed — system fonts are used as fallback.

## Usage

Download `index.html` and open in any browser. No server required.

```bash
git clone https://github.com/zavetsec/opsec-checklist
cd opsec-checklist

# macOS
open index.html

# Linux
xdg-open index.html

# Windows
start index.html
```

Or place on any static hosting or GitHub Pages.

## Threat model profiles

**◐ Privacy** — protection from tracking, data brokers, and opportunistic threats. Relevant for most users: journalists, activists, privacy-conscious individuals.

**◉ Full Anonymity** — protection from targeted attacks, state-level adversaries, border searches. Relevant for security researchers and high-risk individuals.

## Regional specifics (Russia / CIS)

Unlike generic English-language checklists, this one explicitly covers the operational realities of Russian and CIS environments:

- **DPI bypass** — VLESS+Reality, Shadowsocks-2022, Tor bridges (Snowflake, obfs4) for ТСПУ environments
- **SORM** — voice and messaging recommendations account for Russian lawful intercept infrastructure
- **SIM-swap** — specific guidance for Russia where carrier store social engineering is a practical threat vector
- **Financial OPSEC** — clear distinction between fraud protection (Russian virtual cards) and actual anonymity (Monero, LocalMonero cash routes); no US-only services like Privacy.com
- **Legal references** — 152-FZ right to data deletion, Yandex removal requests
- **Local tools** — Kaspersky, 3x-ui, and other tools common in Russian security stacks

## Not for

This checklist is not a silver bullet, military-grade doctrine, or guarantee against nation-state compromise. It will not protect you if your threat model involves a dedicated state adversary with physical access, legal compulsion, or zero-day capabilities against your specific infrastructure.

It is designed as a practical framework for materially reducing your attack surface and improving operational discipline against realistic threats. OPSEC is a continuous process of reducing unnecessary exposure — not a one-time configuration.

## Philosophy

> *"Erase your personal history."*
> — Carlos Castaneda, Journey to Ixtlan

Security is not a product, it's a practice. This checklist is a starting point — not a guarantee. Your threat model is unique. Read every item, understand the *why*, and implement what applies to your actual situation.

## Contributing

Issues and PRs welcome. If you find outdated information (service availability changes, new tools, deprecated recommendations) — open an issue or submit a fix.

## License

MIT — free to use, modify, and distribute. Attribution appreciated but not required.

---

<div align="center">
<sub>Built by <a href="https://github.com/zavetsec">ZavetSec</a> · Open source security toolkit</sub>
</div>

<!-- keywords: OPSEC, privacy, anonymity, Russia, CIS, threat modeling, digital security, DPI bypass, SORM, ТСПУ, operational security, infosec, surveillance, censorship, VPN, Tor, Signal, VeraCrypt, KeePass -->
