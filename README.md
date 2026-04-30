# ZavetSec OPSEC Checklist

<div align="center">

![Version](https://img.shields.io/badge/version-2.0-00ff88?style=flat-square&labelColor=0a0d10)
![Language](https://img.shields.io/badge/language-RU%20%2F%20EN-00ff88?style=flat-square&labelColor=0a0d10)
![License](https://img.shields.io/badge/license-MIT-00ff88?style=flat-square&labelColor=0a0d10)
![Categories](https://img.shields.io/badge/categories-12-00ff88?style=flat-square&labelColor=0a0d10)
![Items](https://img.shields.io/badge/items-68%2B-00ff88?style=flat-square&labelColor=0a0d10)
![Offline Ready](https://img.shields.io/badge/offline-ready-00ff88?style=flat-square&labelColor=0a0d10)
![No Tracking](https://img.shields.io/badge/tracking-none-00ff88?style=flat-square&labelColor=0a0d10)

**A self-contained OPSEC assessment framework available in two independently adapted editions — one for Russia/CIS threat environments, one for US/EU/International environments.**

[🇷🇺 Russian edition](index.html) · [🇬🇧 International edition](index.en.html) · [Live demo →](https://zavetsec.github.io/opsec-checklist)

</div>

---

![ZavetSec OPSEC Checklist Preview](docs/preview.png)

---

## Which edition is right for you?

| Edition | File | Best for |
|---------|------|----------|
| 🇷🇺 **Russian / CIS** | `index.html` | Russia, Belarus, Kazakhstan — SORM, ТСПУ/DPI, regional services |
| 🇬🇧 **US / EU / International** | `index.en.html` | USA, EU, UK, Canada, Five Eyes — GDPR, CCPA, Western platforms |

## Why this exists

Most security advice assumes a single threat landscape — usually Western. In practice, users in Russia and CIS operate under fundamentally different legal, technical, and surveillance conditions than users in the US or EU. This project provides two purpose-built editions: same structure, same depth, different operational context.

## Two editions — same framework, different adversary models

This is not a translation. Each edition is independently adapted to its target environment: tools, services, legal references, threat actors, and bypass techniques are specific to each region.

### 🇷🇺 Russian / CIS Edition (`index.html`)

Built around the operational realities of Russia and CIS:

| Area | Coverage |
|------|----------|
| **Censorship & DPI** | VLESS+Reality, Shadowsocks-2022, Tor bridges (Snowflake, obfs4) for ТСПУ/Roskomnadzor blocking |
| **Wiretapping** | SORM-aware recommendations for voice calls and messengers |
| **SIM-swap** | Carrier store social engineering — practical threat vector in Russia |
| **Financial OPSEC** | Explicit distinction: virtual cards (Tinkoff/Alfa) = fraud protection only, NOT anonymity; real anonymity via Monero, LocalMonero cash routes |
| **Legal** | 152-FZ right to data deletion, Yandex search removal requests |
| **Local tools** | Kaspersky, 3x-ui — common in Russian security stacks |
| **Data brokers** | Russian aggregator removal via 152-FZ and Yandex feedback forms |

### 🇬🇧 US / EU / International Edition (`index.en.html`)

Built around the operational realities of US, EU, and international environments:

| Area | Coverage |
|------|----------|
| **Surveillance** | NSA/GCHQ mass surveillance, Five Eyes context, ISP-level tracking |
| **SIM-swap** | Call center impersonation — dominant vector in US/UK |
| **Financial OPSEC** | Privacy.com (US) single-use virtual cards; Revolut/Wise (EU); Monero for actual anonymity |
| **Legal** | GDPR right to erasure (EU), CCPA data deletion (California), Fifth Amendment biometrics at US borders |
| **Data brokers** | DeleteMe, Incogni — automated removal from Spokeo, Whitepages, BeenVerified, Radaris, 100+ US brokers |
| **Tools** | Bitdefender, ESET, Malwarebytes, Little Snitch (macOS), LuLu — no Kaspersky |
| **Platform** | Apple Privacy (Advanced Data Protection, Hide My Email), iCloud E2EE, FaceTime |

## Categories

Both editions share the same 12-category structure (68+ items total):

| # | Category |
|---|----------|
| 01 | Digital Identity & Anonymity |
| 02 | Threat Modeling |
| 03 | Devices & Physical Security |
| 04 | Network & Traffic |
| 05 | Communications & Messengers |
| 06 | Data & Storage |
| 07 | Social Engineering & Phishing |
| 08 | Browser & Web Privacy |
| 09 | Digital Footprint & De-anonymization |
| 10 | Financial OPSEC |
| 11 | Travel Security & Border Crossing |
| 12 | Incident Response & Canary Tokens |

## Features

Both editions share the same interactive feature set:

- **Threat model profiles** — select *Privacy* or *Full Anonymity* to highlight relevant items
- **Progress tracking** — state saved locally in browser, survives page reload
- **Search** — full-text search across all items (Ctrl+F)
- **Export** — generate a standalone HTML report of current state
- **Deep links** — direct link to any individual item via anchor
- **Print-friendly** — clean print stylesheet included
- **Zero dependencies** — single self-contained HTML file, no external requests\*

> \* Except Google Fonts loaded at render time. For fully offline use, the font import can be removed — system fonts are used as fallback.

## Usage

Download the edition relevant to your threat environment and open in any browser. No server required.

```bash
git clone https://github.com/zavetsec/opsec-checklist
cd opsec-checklist

# Russian / CIS edition
# macOS:   open index.html
# Linux:   xdg-open index.html
# Windows: start index.html

# US / EU / International edition
# macOS:   open index.en.html
# Linux:   xdg-open index.en.html
# Windows: start index.en.html
```

Or place on any static hosting or GitHub Pages.

## Threat model profiles

**◐ Privacy** — protection from tracking, data brokers, and opportunistic threats. Relevant for most users: journalists, activists, privacy-conscious individuals.

**◉ Full Anonymity** — protection from targeted attacks, state-level adversaries, border searches. Relevant for security researchers and high-risk individuals.

## Disclaimer

This material is provided for **educational purposes only** and reflects the author's personal stance in support of every individual's right to privacy, digital security, and freedom of personal life.

We believe **privacy is a fundamental right**, not a privilege. All recommendations are aimed at protecting legitimate interests: personal data, communications, financial information, and digital identity from unauthorized access, surveillance, and leaks.

The author assumes **no liability** for any use of the information presented that violates the laws of the user's jurisdiction. Users are solely responsible for ensuring their actions comply with applicable laws and regulations.

All tools, services, and technologies mentioned are **publicly available** and used by millions of people worldwide for lawful purposes. Their mention does not constitute encouragement of any unlawful activity.

## Not for

This checklist is not a silver bullet, military-grade doctrine, or guarantee against nation-state compromise. It will not protect you if a government agency is specifically targeting you, has physical access to your devices, or is willing to use legal pressure and advanced technical capabilities against you personally.

It is designed as a practical framework for materially reducing your attack surface and improving operational discipline against realistic threats. OPSEC is a continuous process of reducing unnecessary exposure — not a one-time configuration.

## Philosophy

> *"Erase your personal history."*
> — Carlos Castaneda, Journey to Ixtlan

Security is not a product, it's a practice. This checklist is a starting point — not a guarantee. Your threat model is unique. Read every item, understand the *why*, and implement what applies to your actual situation.

## Contributing

Issues and PRs welcome. If you find outdated information (service availability changes, new tools, deprecated recommendations for either edition) — open an issue or submit a fix.

## License

MIT — free to use, modify, and distribute. Attribution appreciated but not required.

---

<div align="center">
<sub>Built by <a href="https://github.com/zavetsec">ZavetSec</a> · Open source security toolkit</sub>
</div>

<!-- keywords: OPSEC, privacy, anonymity, Russia, CIS, USA, EU, threat modeling, digital security, DPI bypass, SORM, ТСПУ, operational security, infosec, surveillance, censorship, VPN, Tor, Signal, VeraCrypt, KeePass, GDPR, CCPA, data brokers, Privacy.com, Monero, Five Eyes -->
