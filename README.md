## Aidan Smith

Cybersecurity student at Westchester Community College (AAS, May 2027), heading
for a Computer Science transfer and a career in federal cyber defense. CompTIA
**A+**, **Network+**, and **Security+** certified.

I learn by building and breaking things I own. Most of what is below runs
continuously on hardware I own, not in a tutorial.

---

### What I run

**Home SOC — Proxmox, Wazuh, Pi-hole**
A single-node Proxmox hypervisor running unprivileged LXC guests: a Pi-hole DNS
sinkhole, a dashboard host, and a Wazuh 4.x SIEM with agents on the hypervisor
and every container. I enumerated the whole estate first, wrote up eight
severity-rated findings against my own network, and then closed the largest one
— there was no centralised logging, so the window between compromise and
discovery was unbounded. The remediation notes include the sequencing hazards,
because enabling the Proxmox firewall in the wrong order locks you out of your
own hypervisor.

→ [`Wazuh-Pihole-Deployment`](https://github.com/hoursgonebye/Wazuh-Pihole-Deployment)

**Ops Deck — a self-hosted dashboard**
A Flask + SQLite application I use daily: boards, calendar, routines, a skill
tree, finance ledger, transcript/GPA tracking, 3D printer telemetry, and a
homelab inventory. No frontend framework and no build step — vanilla JS by
choice. Sixteen additive schema migrations, per-module blueprints, and test
suites that run inside the built container image.

The design rule I care most about: **nothing that can be derived is ever
stored.** No GPA, XP total, or account balance is a column. They are all
queries over an append-only ledger, so correcting one input re-derives every
figure downstream instead of leaving drift behind.

→ [`opsdeck`](https://github.com/hoursgonebye/opsdeck)

**Cyberdeck — a portable RF/wireless testing deck**
Raspberry Pi 5 with a battery/UPS HAT, a BB Q20 keyboard on I²C behind an
out-of-tree driver, GPS on the header UART, a CC1101 sub-GHz transceiver on
SPI, an RTL-SDR, and an MT7612U adapter verified in monitor mode. Two boards
died to shorts before this one; the build log documents the failures as
carefully as the successes.

→ [`cyberdeck`](https://github.com/hoursgonebye/cyberdeck)

---

### Competing

**National Cyber League**, Fall 2026 season — Gymnasium, Individual and Team
games. Nine categories: OSINT, cryptography, password cracking, log analysis,
network traffic analysis, forensics, scanning, web exploitation, and enumeration
and exploitation.

---

### Currently

- Cybersecurity AAS at WCC, graduating May 2027
- IT work-study on the WCC help desk
- Studying toward a CS transfer and the **CyberCorps: Scholarship for Service** program
- Working through TryHackMe and building out the lab above

### Tools I actually use

`Linux` `Proxmox` `Docker` `Wazuh` `Pi-hole` `Tailscale`
`Python` `Flask` `SQLite` `Bash` `Git` `Kali` `SDR`

---

<sub>Most of my work lives in the repositories above rather than in a résumé.
If something here is interesting, the commit histories and build logs are the
honest version.</sub>
