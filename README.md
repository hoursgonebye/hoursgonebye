<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:1f6feb,100:2ea043&height=200&section=header&text=Aidan%20Smith&fontSize=54&fontColor=ffffff&fontAlignY=34&desc=Cybersecurity%20student%20·%20building%20a%20home%20SOC%20·%20heading%20for%20federal%20cyber&descAlignY=54&descSize=15" width="100%" alt="Aidan Smith" />

<a href="https://www.comptia.org/certifications/a"><img src="https://img.shields.io/badge/CompTIA-A%2B-E31837?style=flat-square&logo=comptia&logoColor=white" alt="CompTIA A+" /></a>
<a href="https://www.comptia.org/certifications/network"><img src="https://img.shields.io/badge/CompTIA-Network%2B-E31837?style=flat-square&logo=comptia&logoColor=white" alt="CompTIA Network+" /></a>
<a href="https://www.comptia.org/certifications/security"><img src="https://img.shields.io/badge/CompTIA-Security%2B-E31837?style=flat-square&logo=comptia&logoColor=white" alt="CompTIA Security+" /></a>
<img src="https://img.shields.io/badge/AAS_Cybersecurity-May_2027-1f6feb?style=flat-square" alt="AAS Cybersecurity, May 2027" />
<img src="https://img.shields.io/badge/National_Cyber_League-Fall_2026-2ea043?style=flat-square" alt="National Cyber League Fall 2026" />

</div>

---

I learn by building and breaking things I own. Everything below runs
continuously on hardware I own, not in a tutorial — a Proxmox hypervisor, a
SIEM watching it, a dashboard I use daily, and a handheld RF deck I have
killed two boards building.

Heading for a Computer Science transfer and a career in federal cyber defense.

<div align="center">

<img src="https://skillicons.dev/icons?i=linux,debian,docker,python,flask,sqlite,bash,js,html,css,git,raspberrypi,vim&theme=dark&perline=13" alt="Linux, Debian, Docker, Python, Flask, SQLite, Bash, JavaScript, HTML, CSS, Git, Raspberry Pi, Vim" />

</div>

---

## Things I have built

<table>
<tr>
<td width="50%" valign="top">

### 🛡️ Home SOC
**Proxmox · Wazuh · Pi-hole · Tailscale**

A single-node hypervisor running unprivileged LXC guests, with a Wazuh SIEM
and agents on the host and every container.

I enumerated the estate first, wrote up **eight severity-rated findings against
my own network**, then closed the largest — there was no centralised logging,
so the window between compromise and discovery was unbounded.

The remediation notes include the sequencing hazards, because enabling the
firewall in the wrong order locks you out of your own hypervisor.

[`Wazuh-Pihole-Deployment →`](https://github.com/hoursgonebye/Wazuh-Pihole-Deployment)

</td>
<td width="50%" valign="top">

### 📟 Cyberdeck
**Raspberry Pi 5 · SDR · sub-GHz · GPS**

A portable RF and wireless testing deck: BB Q20 keyboard on I²C behind an
out-of-tree driver, GPS on the header UART, a CC1101 transceiver on SPI, an
RTL-SDR, and an MT7612U verified in monitor mode.

Two boards died to shorts before this one. The build log documents the
failures as carefully as the successes, including why there is deliberately
no fusing anywhere in it.

[`cyberdeck →`](https://github.com/hoursgonebye/cyberdeck)

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 📊 Ops Deck
**Flask · SQLite · vanilla JS, no build step**

A self-hosted dashboard I use every day: boards, calendar, routines, a skill
tree, a finance ledger, transcript and GPA tracking, 3D printer telemetry and
a homelab inventory. Sixteen additive schema migrations and test suites that
run inside the built container image.

The rule I care most about: **nothing derivable is ever stored.** No GPA, XP
total or account balance is a column — they are queries over an append-only
ledger, so fixing one input re-derives everything downstream instead of
leaving drift behind.

[`opsdeck →`](https://github.com/hoursgonebye/opsdeck)

</td>
<td width="50%" valign="top">

### 🐍 Foundations
**Python, written to understand rather than to import**

Magic-number file type detection, a XOR stream cipher, Base64 encode/decode,
and a terminal ticket tracker.

Deliberately unpolished and kept that way — each exists because I wanted to
understand one idea by implementing it. The first practical security lesson
in the set is that a file extension is a naming convention, not a fact.

[`python-fundamentals →`](https://github.com/hoursgonebye/python-fundamentals)

</td>
</tr>
</table>

---

## Currently

| | |
|---|---|
| 🎓 | Cybersecurity AAS at Westchester Community College, graduating **May 2027** |
| 🖥️ | IT work-study on the college help desk |
| 🎯 | Studying toward a CS transfer and the **CyberCorps: Scholarship for Service** |
| 🚩 | **National Cyber League** Fall 2026 — Gymnasium, Individual and Team games |
| 🔧 | Hardening the lab: backups, firewall policy, and network segmentation next |

<div align="center">

<img src="https://img.shields.io/badge/Python-620k-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
<img src="https://img.shields.io/badge/JavaScript-310k-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript" />
<img src="https://img.shields.io/badge/CSS-89k-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS" />
<img src="https://img.shields.io/badge/C-59k-A8B9CC?style=for-the-badge&logo=c&logoColor=black" alt="C" />
<img src="https://img.shields.io/badge/Shell-12k-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white" alt="Shell" />

<sub>Bytes of code across public repositories.</sub>

<br />

<sub>Most of my work lives in the repositories above rather than in a résumé.
If something here is interesting, the commit histories and build logs are the
honest version.</sub>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:2ea043,50:1f6feb,100:0d1117&height=120&section=footer" width="100%" alt="" />

</div>
