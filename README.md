# Writeups-Reports

Full penetration test reports for retired HackTheBox machines, written in professional client-deliverable format using SysReptor.

These aren't blog posts or step-by-step tutorials. Each one is a complete report — the kind you'd hand to a client after an engagement.

---

## Format

Every report follows the same structure:

- **Statement of Confidentiality**
- **Engagement Contacts** — Assessor and client-side stakeholders
- **Executive Summary** — Approach, scope, and non-technical overview of risk and recommendations
- **Assessment Summary** — Severity distribution, findings table with CVSS scores
- **Attack Chain Walkthrough** — Full narrative of the path from initial access to full compromise, with tool output and screenshots at each step
- **Remediation Summary** — Short, medium, and long-term remediation broken out by finding, with prioritization rationale
- **Technical Findings** — Per-finding detail including CWE, CVSS 3.1 vector, root cause, impact, affected components, remediation steps with implementation guidance, references, and evidence screenshots
- **Appendices** — Host and service discovery, subdomain enumeration, exploited hosts, compromised users, cleanup/changes made, flags

---

## Reports

| Machine | OS | Difficulty |
|---|---|---|
| Trick | Linux | Easy |
| TombWatcher | Windows | Medium |
| VulnCicada | Windows | Medium |

---

## Why report format?

Most writeups are blog posts or markdown notes. These are practice deliverables — structured, evidenced, and written for a reader who needs to understand both what happened and what to do about it.

The technical work is only half the job. The report is what the client actually sees.

---

## Tools & Methodology

Engagements follow a structured methodology aligned with PTES. Reports rendered with [SysReptor](https://github.com/syslifters/sysreptor). Common tooling includes:

`nmap` · `netexec` / `crackmapexec` · `impacket` · `certipy` · `kerbrute` · `bloodyAD` · `BloodHound` · `hashcat`

---

## Related Repos

- [`Invoke-ADHostDiscovery`](https://github.com/0xWr417h/Invoke-ADHostDiscovery) — Low-noise AD host discovery, no RSAT required
- [`Show-ServiceAcl`](https://github.com/0xWr417h/Show-ServiceAcl) — Human-readable Windows service ACL parsing
- [`parse_secrets.py`](https://github.com/0xWr417h/parse_secrets.py) — Secretsdump/nxc output parser for kerbrute, hashcat, and PTH workflows
- [`recon.sh`](https://github.com/0xWr417h/recon.sh) — Two-stage recon: host discovery + targeted nmap enumeration

---

## License

MIT
