<div align="center">

# 🎯 CTF Lab: Mission of the Rotten Peel

### A Gamified Capture-The-Flag Learning Laboratory for Cybersecurity Education

![Stages](https://img.shields.io/badge/Stages-17-E8B923?style=flat-square)
![Level](https://img.shields.io/badge/Level-Beginner--Friendly-6B8E23?style=flat-square)
![Domains](https://img.shields.io/badge/Domains-Recon%20%7C%20Web%20%7C%20SocEng%20%7C%20Crypto%20%7C%20Forensics-6B4423?style=flat-square)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=flat-square)
![License](https://img.shields.io/badge/License-Educational%20Use-lightgrey?style=flat-square)

*Supervised by Dr. Mohamed Saeed*

</div>

---

## 👥 Project Team

| # | Name | Role |
|---|------|------|
| 1 | Andrew Beshay Mousa | Team Leader |
| 2 | Ahmed Ashraf Ahmed | Team Member |
| 3 | Youssef Hany Elshamly | Team Member |
| 4 | Mazen Ashraf Basha | Team Member |

---

## 📖 Table of Contents

- [Overview](#-overview)
- [Why This Project Exists](#-why-this-project-exists)
- [The Cyber Kill Chain](#-the-cyber-kill-chain)
- [Topics Covered (A–Z)](#-topics-covered-az)
- [The Story](#-the-story)
- [Instructional Design](#-instructional-design)
- [Stage-by-Stage Walkthrough](#-stage-by-stage-walkthrough)
- [Tools Summary](#-tools-summary)
- [Learning Outcomes](#-learning-outcomes)
- [Lab Setup Manual](#-lab-setup-manual)
- [Conclusion](#-conclusion)
- [References](#-references)

---

## 🧭 Overview

This repository documents the design, curriculum, and technical build of a **17-stage Capture-The-Flag (CTF) learning laboratory** created to introduce students and cybersecurity beginners to practical offensive-security concepts through a single, continuous, story-driven engagement — from the first reconnaissance scan to final evidence reporting.

Rather than a set of disconnected challenges, every stage's output (a password, a username, a hidden file) becomes the literal input required to unlock the next stage, so learners experience the same information-driven momentum as a real penetration test while staying anchored in a light, memorable narrative.

---

## 💡 Why This Project Exists

Cybersecurity education often teaches foundational material — networking, protocols, cryptography — in a way that's technically accurate but disconnected from why it actually matters in practice. This lab closes that gap by wrapping a rigorous technical curriculum inside an approachable, lightly humorous corporate-mystery storyline.

**Every stage follows the same four-part structure:**
- 📘 A plain-language technical lesson
- 🌍 A real-world case study where the same vulnerability class caused real damage
- 🎭 The in-story scenario justifying the task
- 🚩 A hands-on task with a verifiable flag or knowledge check

**Target audience:** undergraduate students, cybersecurity club members, and complete beginners — supported by on-demand hints, explicit command syntax, and knowledge checks that gate high-risk actions (like firewall changes) behind conceptual understanding.

---

## ⛓️ The Cyber Kill Chain

The lab is structured around the **Lockheed Martin Cyber Kill Chain** — a 7-phase model describing the sequence an attacker must complete to succeed. Its core lesson: an attacker must succeed at *every* phase; a defender only needs to break *one* link.

| Kill Chain Phase | Lab Stage(s) | What It Represents |
|---|---|---|
| **1. Reconnaissance** | 1, 2, 3, 14 | Identifying live services, exposed info, and OSINT before any attack begins |
| **2. Weaponization** | 4, 5, 11 | Preparing the SQLi payload, phishing pretext, or wordlist |
| **3. Delivery** | 4, 5 | Getting the payload/pretext in front of the target |
| **4. Exploitation** | 4, 6, 10, 12 | Triggering the vulnerability for unauthorized access |
| **5. Installation** | 7, 8, 13 | Establishing a persistent foothold on a compromised host |
| **6. Command & Control** | 8, 9, 10, 12, 13 | Standing control over infrastructure and hosts |
| **7. Actions on Objectives** | 13, 14, 15, 16, 17 | Exfiltrating, decrypting, and reporting the evidence |

> 💬 Reconnaissance recurs at Stage 14 as OSINT — intelligence-gathering isn't confined to the opening of an engagement. Installation/C2 use legitimate protocol abuse (SSH, pfSense) rather than malware, keeping the lab safe for beginners.

---

## 🔤 Topics Covered (A–Z)

<details>
<summary><strong>Click to expand the full topic list</strong></summary>

| Topic | Covered In |
|---|---|
| Active Directory credential abuse | Phishing / lateral-movement stages |
| AES-256 Encryption | Stage 15 |
| Asset inventory & cross-referencing | Stage 7 |
| Brute-force attacks | Stages 6, 12 |
| Command-line proficiency | All 17 stages |
| Digital forensics fundamentals | Stage 16 |
| Encryption vs. concealment | Stages 8, 15 |
| Firewall architecture & rule evaluation | Stages 9–10 |
| FTP protocol weaknesses | Stage 7 |
| GPG / GnuPG symmetric encryption | Stages 14–15 |
| HTML source-code inspection | Stage 2 |
| Incident evidence handling | Stage 17 |
| John the Ripper rule-based mutation | Stage 11 |
| Kill-chain methodology | Whole-lab structure |
| Lateral movement | Stages 8, 12, 13 |
| Multi-factor authentication (as a defence) | Brute-force stages |
| Nmap port scanning | Stage 1 |
| Open-source intelligence (OSINT) | Stage 14 |
| pfSense firewall administration | Stages 9–10 |
| Phishing & pretexting | Stage 5 |
| Post-exploitation triage | Stage 13 |
| Responsible disclosure | Stage 17 |
| SFTP-based secure exfiltration | Stage 13 |
| SMB enumeration & misconfiguration | Stage 3 |
| Social engineering psychology | Stage 5 |
| SQL Injection | Stage 4 |
| SSH tunnelling & secure remote access | Stage 9 |
| Steganography | Stage 8 |
| Threat-actor tradecraft (edit vs. add rules) | Stage 10 |
| Username enumeration | Stages 3, 7 |
| Vulnerability chaining | Whole-lab structure |
| Weak/default/predictable passwords | Stages 6, 11, 12, 15 |
| Wordlist engineering | Stage 11 |
| Zero-trust principle (by contrast) | Discussed conceptually |

</details>

---

## 🎭 The Story

The learner plays a newly onboarded security intern who notices something is wrong with the organisation's leadership and internal security posture. Routine reconnaissance escalates into a full investigation uncovering a covert scheme run by a senior executive — culminating in the collection and formal submission of evidence.

The narrative beats are engineered to align exactly with the kill chain, so **progressing the plot and progressing technical skill are the same act**. Recurring characters (a suspicious executive, a compromised staff member whose social media becomes a genuine investigative lead) give the specific vulnerabilities exploited at each stage a believable, memorable pretext. Completion awards a printable certificate and narrative epilogue — mirroring the deliverable-oriented conclusion of a real security engagement.

---

## 🛠️ Instructional Design

- 📊 A persistent progress sidebar tracking unlocked stages
- 🧩 The four-part lesson → real-world case → scenario → task structure, repeated every stage
- 💡 On-demand hints at every stage
- 🔗 Outside reference links to primary sources (OWASP, NIST, MITRE ATT&CK, CISA)
- ✅ Knowledge-check gates (Stages 9 & 15) that block progress until concepts — not just flags — are understood
- 🎓 An extended interactive tutorial in Stage 1 (drag-and-drop + true/false) for complete beginners

---

## 🚩 Stage-by-Stage Walkthrough

Each stage below is broken into **Idea → How We Applied It → Result → Connection to Next Stage**, so the whole chain reads as one continuous engagement.

<details>
<summary><strong>Stage 1 — Network Port Scanning (Nmap)</strong> · Reconnaissance</summary>

- **💡 Idea:** Before exploitation, an attacker must know which services are reachable. Nmap probes the full port range and reports state + service/version — the same technique underlying Shodan and used in the WannaCry post-mortem.
- **⚙️ Applied:** Ran `nmap -sV 10.10.10.5` from Kali; read OPEN vs CLOSED/FILTERED states; completed a drag-and-drop port-matching + true/false pre-task tutorial.
- **✅ Result:** Three open ports found — `21/tcp (FTP)`, `80/tcp (HTTP)`, `445/tcp (SMB)`.
- **🔗 Next:** Port 80 → Stage 2, Port 445 → Stage 3, Port 21 revisited in Stage 6.
</details>

<details>
<summary><strong>Stage 2 — HTTP Reconnaissance (curl)</strong> · Web Enumeration</summary>

- **💡 Idea:** curl reveals the raw HTML a browser hides — including developer comments. Same class of flaw seen in the 2020 Twitter takeover incident.
- **⚙️ Applied:** Ran `curl http://10.10.10.5`; manually searched for `<!-- -->` comment blocks.
- **✅ Result:** Credential `lets_dance_samba` found in an HTML comment.
- **🔗 Next:** This password unlocks the SMB share in Stage 3.
</details>

<details>
<summary><strong>Stage 3 — File Share Enumeration (smbclient)</strong> · SMB Enumeration</summary>

- **💡 Idea:** SMB shares are often left accessible far beyond their intended audience — the same weakness (EternalBlue) behind WannaCry's 230,000-machine outbreak.
- **⚙️ Applied:** `smbclient //10.10.10.5/MyShared -U samba`; listed and pulled files with `get <filename>`.
- **✅ Result:** FTP username `mrfile` + a password-list file recovered.
- **🔗 Next:** Feeds directly into the Stage 6 brute-force attack on port 21.
</details>

<details>
<summary><strong>Stage 4 — SQL Injection</strong> · Exploitation</summary>

- **💡 Idea:** Unsanitised input lets an attacker alter query logic. The same technique enabled the 2011 Sony PSN breach (77M accounts).
- **⚙️ Applied:** On `http://10.10.10.5/banana_portal`, submitted `' OR 1=1 --` in the username field.
- **✅ Result:** Full employee table dumped, revealing `banana.masterfirewall@gmail.com`.
- **🔗 Next:** This address is the sole target of the Stage 5 phishing email — a new parallel branch.
</details>

<details>
<summary><strong>Stage 5 — Spear-Phishing Email Construction</strong> · Social Engineering</summary>

- **💡 Idea:** Phishing exploits urgency, authority, and familiarity — the entry point for most real-world breaches, including the 2016 U.S. election-related compromise.
- **⚙️ Applied:** Drafted a spear-phishing email impersonating the target's manager, urging upload of directory credentials to the FTP server.
- **✅ Result:** Flag `flag{Learning_Fishing}` for a correctly pretexted draft.
- **🔗 Next:** Sets up the premise that makes the Stage 6 FTP brute-force meaningful.
</details>

<details>
<summary><strong>Stage 6 — Password Brute-Forcing (Hydra)</strong> · Credential Attacks</summary>

- **💡 Idea:** Automated login cracking — Hydra cracked most of LinkedIn's 6.5M leaked hashes within days in 2012.
- **⚙️ Applied:** `hydra -l mrfile -P .passwords.txt ftp://10.10.10.5`
- **✅ Result:** FTP password `duck` recovered.
- **🔗 Next:** `mrfile:duck` logs into FTP in Stage 7.
</details>

<details>
<summary><strong>Stage 7 — FTP Server Exploitation</strong> · Post-Exploitation</summary>

- **💡 Idea:** FTP is unencrypted and legacy — implicated in the 2021 Florida water-treatment facility breach.
- **⚙️ Applied:** `ftp 10.10.10.5`; downloaded Harry's note + asset list; cross-referenced name → username.
- **✅ Result:** SSH username `harrykane` derived.
- **🔗 Next:** Used to establish SSH access in Stage 8.
</details>

<details>
<summary><strong>Stage 8 — SSH Access & Steganographic Extraction</strong> · Lateral Movement</summary>

- **💡 Idea:** Steganography hides data inside ordinary files — documented in real malware hiding C2 instructions inside meme images.
- **⚙️ Applied:** SSH as `harrykane`; `find / -iname '*pfsense*'`; pulled image via SFTP; `steghide extract -sf weird_photo.jpg`.
- **✅ Result:** Flag `flag{hide_and_seek}` — confirms this account holds pfSense-related credentials.
- **🔗 Next:** Unlocks the pfSense console explored in Stages 9–10.
</details>

<details>
<summary><strong>Stage 9 — pfSense Conceptual Knowledge Check</strong> · Firewall Fundamentals</summary>

- **💡 Idea:** Firewall misconfiguration is a leading breach cause (e.g., a 2020 incident exposing ~100 GB of customer data). No live action here — theory first.
- **⚙️ Applied:** Studied SSH-tunnelled console access and rule-evaluation order (top-to-bottom, first match wins); answered 3 MCQs.
- **✅ Result:** All 3 questions answered correctly — no flag by design.
- **🔗 Next:** This theory is applied directly in Stage 10.
</details>

<details>
<summary><strong>Stage 10 — Firewall Rule Reconfiguration</strong> · Command & Control</summary>

- **💡 Idea:** Attackers often edit existing rules rather than add new ones — quieter and easier to miss in an audit.
- **⚙️ Applied:** In pfSense: `Firewall > Rules > LAN`; edited the existing block rule's Action from `Block` → `Pass`; verified with `nmap 10.10.30.13`.
- **✅ Result:** Flag `flag{M@st8r_0F_Flrew@l1l}` — Segment 10.10.30.0/24 now reachable.
- **🔗 Next:** Opens access to the host targeted in Stages 11–12.
</details>

<details>
<summary><strong>Stage 11 — Targeted Wordlist Generation (John the Ripper)</strong> · Password Cracking</summary>

- **💡 Idea:** Rule-based mutation turns one seed word into realistic candidates — John cracked ~90% of LinkedIn's leaked hashes in a week.
- **⚙️ Applied:** `echo 'Mr. peel' > base.txt` → `john --wordlist=base.txt --rules --stdout > wordlist.txt` → `wc -l wordlist.txt`.
- **✅ Result:** `3` candidate passwords generated.
- **🔗 Next:** Fed directly into the Stage 12 Hydra attack.
</details>

<details>
<summary><strong>Stage 12 — Targeted SSH Brute-Force (Hydra)</strong> · Lateral Movement</summary>

- **💡 Idea:** A small targeted wordlist beats a huge generic one — the same approach used in the 2014 "Celebgate" iCloud breach.
- **⚙️ Applied:** `hydra -l Mr.peel -P wordlist.txt ssh://10.10.30.13`
- **✅ Result:** SSH password `mrpeel` recovered.
- **🔗 Next:** Grants SSH access used to search the host in Stage 13.
</details>

<details>
<summary><strong>Stage 13 — Data Discovery & Retrieval via SFTP</strong> · Exfiltration</summary>

- **💡 Idea:** SFTP is encrypted end-to-end, unlike Stage 7's plaintext FTP — mirrors the anomaly-hunting seen in the 2020 SolarWinds compromise.
- **⚙️ Applied:** `ssh Mr.peel@10.10.30.13`; `find / -name '*.gpg'`; retrieved via `sftp` + `get`.
- **✅ Result:** Encrypted archive `You_Will_Never_Get_Me.tar.gz.gpg` recovered.
- **🔗 Next:** Cannot be opened without the passphrase found via OSINT in Stage 14.
</details>

<details>
<summary><strong>Stage 14 — Passphrase Discovery via OSINT</strong> · Cryptography / OSINT</summary>

- **💡 Idea:** Cryptography is only as strong as the human-chosen key — as in the 2016 Reality Winner case.
- **⚙️ Applied:** Recalled the clue about something the target "loves most"; searched Harry Kane's public Instagram for a recurring name.
- **✅ Result:** Passphrase `Z3tar` (the CEO's dog's name) identified.
- **🔗 Next:** Used directly to decrypt the archive in Stage 15.
</details>

<details>
<summary><strong>Stage 15 — GPG Decryption & AES-256 Knowledge Check</strong> · Decryption</summary>

- **💡 Idea:** AES-256 secures HTTPS, BitLocker, and Signal — the algorithm was never the weak point here, the passphrase was.
- **⚙️ Applied:** `gpg --decrypt You_Will_Never_Get_Me.tar.gz.gpg > You_Will_Never_Get_Me.tar.gz` using `Z3tar`; answered 3 AES-256 MCQs.
- **✅ Result:** Archive decrypted + all 3 questions correct — no separate flag by design.
- **🔗 Next:** The decrypted archive is unpacked in Stage 16.
</details>

<details>
<summary><strong>Stage 16 — Archive Extraction & Evidence Review</strong> · Digital Forensics</summary>

- **💡 Idea:** Compress-then-encrypt is the correct order; forensics often means unwinding exactly that chain.
- **⚙️ Applied:** `tar -xzf You_Will_Never_Get_Me.tar.gz`; reviewed extracted docs; `grep -i project`.
- **✅ Result:** Flag `flag{MIND_JUICE}` — internal project codename identified.
- **🔗 Next:** Forms part of the evidence package submitted in Stage 17.
</details>

<details>
<summary><strong>Stage 17 — Evidence Submission & Engagement Closure</strong> · Reporting & Disclosure</summary>

- **💡 Idea:** Documentation and responsible disclosure are what convert a technical exercise into an actionable report — as in the 2021 nuclear-contractor vulnerability disclosure, patched within 24 hours.
- **⚙️ Applied:** Compiled all evidence; uploaded via `http://10.10.10.5/cia_portal`; received a case reference number.
- **✅ Result:** Final flag `flag{th3_w0rld_is_saf3_fr0m_banan4s}` — all 17 stages complete.
- **🔗 Next:** None — this is the convergence point of every credential and finding from Stages 1–16.
</details>

---

## 🧰 Tools Summary

| Tool / Technique | Function | Stage(s) |
|---|---|---|
| `nmap` | Network scanning & service enumeration | 1 |
| `curl` | HTTP request inspection | 2 |
| `smbclient` | SMB share enumeration | 3 |
| Manual SQL injection | Auth bypass / data extraction | 4 |
| Email drafting | Social engineering / phishing | 5 |
| `hydra` | Automated credential brute-forcing | 6, 12 |
| FTP client | File retrieval over plaintext protocol | 7 |
| `ssh` / `steghide` | Remote access & steganographic extraction | 8 |
| pfSense | Firewall administration | 9, 10 |
| `john` | Rule-based wordlist generation | 11 |
| `sftp` | Secure file exfiltration | 13 |
| OSINT research | Passphrase / intelligence gathering | 14 |
| `gpg` | Symmetric decryption | 15 |
| `tar` / `gzip` | Archive extraction & forensic review | 16 |
| Evidence portal | Reporting & responsible disclosure | 17 |

---

## 🎓 Learning Outcomes

By completing all 17 stages, a learner demonstrates hands-on competency in:

- ✅ Network reconnaissance & service enumeration (nmap, curl, smbclient)
- ✅ Web application exploitation (SQL injection)
- ✅ Social-engineering pretext construction
- ✅ Automated & rule-based password attacks (Hydra, John the Ripper)
- ✅ Legacy vs. modern file transfer (FTP vs. SFTP)
- ✅ SSH remote access, steganography, and firewall administration
- ✅ Applied cryptography (GPG, AES-256)
- ✅ Open-source intelligence gathering
- ✅ Digital forensics fundamentals
- ✅ Professional evidence handling and responsible disclosure

Each stage is individually assessed — either via a validated flag, or (Stages 9 & 15) a gated knowledge check — ensuring both **procedural skill** and **conceptual understanding** are verified before progression.

---

## 🖥️ Lab Setup Manual

### Virtual Machines Required

| VM | OS | Segment | Specs | Purpose |
|---|---|---|---|---|
| Attacker Workstation | Kali Linux | A | 2 vCPU / 4 GB / 40 GB | Runs all offensive tooling |
| Web / FTP / SMB Server | Ubuntu Server 22.04 | A | 2 vCPU / 2 GB / 20 GB | Vulnerable portal, FTP, SMB share |
| pfSense Firewall | pfSense CE | A, B, C (router) | 2 vCPU / 2 GB / 10 GB | Routes & filters between segments |
| Intermediate Host (Harry) | Ubuntu/Debian | B | 1 vCPU / 1 GB / 15 GB | Steganography image + pfSense creds |
| Executive Target (Mr. Peel) | Ubuntu/Debian | C | 1 vCPU / 1 GB / 15 GB | Encrypted archive |

### Network & IP Addressing

| Machine / Interface | Segment | IP |
|---|---|---|
| Attacker Workstation | A | `10.10.10.10` |
| Web/FTP/SMB Server | A | `10.10.10.5` |
| pfSense (Segment A iface) | A | `10.10.10.1` (gateway) |
| pfSense (Segment B iface) | B | `10.10.20.1` (gateway) |
| Intermediate Host (Harry) | B | `10.10.20.10` |
| pfSense (Segment C iface) | C | `10.10.30.1` (gateway) |
| Executive Target (Mr. Peel) | C | `10.10.30.13` |

- **Segment A** `10.10.10.0/24` — attacker + web/FTP/SMB server
- **Segment B** `10.10.20.0/24` — reachable after Stages 1–7
- **Segment C** `10.10.30.0/24` — blocked until the Stage 10 firewall fix

### Mail / SPF Configuration (optional, for live Stage 5 delivery)

```
# DNS TXT record for the lab mail domain
v=spf1 mx a ip4:10.10.10.5 -all
```
Point the domain's MX record at the mail VM, install Postfix, and relay the learner's drafted email through it. Optional — the stage can also be graded purely as written work.

### Build Tools Required

- Hypervisor: VirtualBox / VMware / Proxmox
- Kali Linux ISO
- Ubuntu Server ISO
- pfSense CE ISO
- Apache/Nginx + PHP + MySQL (vulnerable login portal)
- `vsftpd` · `samba` · `openssh-server`
- `steghide` · `gnupg` (to pre-seed hidden/encrypted files)
- `postfix` (optional mail server)

### Files Required Per Server

| Server | Files / Services |
|---|---|
| Web/FTP/SMB | Web root with HTML-comment password; SQLi login form + DB; FTP root with `harry_note.txt`, `asset_list.txt`; Samba share with staff list + password list |
| Intermediate Host (Harry) | Steganography image in a giveaway-named folder; pfSense credential notes |
| pfSense | Pre-set `Block` rule, Segment B → Segment C, under `Firewall > Rules > LAN` |
| Executive Target (Mr. Peel) | `You_Will_Never_Get_Me.tar.gz.gpg` in a defiantly-named directory |
| Attacker Workstation | Clean Kali install — no pre-seeded files |

### Build Steps

1. Install the hypervisor and create all 5 VMs per the spec table above.
2. Set up pfSense first — configure 3 interfaces and the initial Block rule.
3. Build the Web/FTP/SMB server — deploy the portal, `vsftpd`, Samba, and seed files.
4. Build both internal Linux hosts — enable SSH, create accounts, seed hidden/encrypted files.
5. Build the Kali attacker VM on Segment A; confirm it can reach Segment A only.
6. Dry-run Stages 1–17 end-to-end from Kali to validate every flag and file.
7. (Optional) Configure Postfix + SPF for a live phishing exercise.
8. Snapshot every VM once validated, so the environment resets cleanly between attempts.

---

## 🏁 Conclusion

This project pairs a light, narrative-driven presentation layer with a rigorous technical curriculum spanning reconnaissance, web exploitation, social engineering, credential attacks, lateral movement, steganography, firewall administration, applied cryptography, OSINT, digital forensics, and professional reporting. Every credential recovered and every rule modified is simultaneously a plot beat *and* a verified, transferable cybersecurity skill — proof that gamification and technical rigor aren't in tension.

The stage-based architecture is built to extend: future branches (cloud misconfig, mobile security, wireless attacks) can slot into the same lesson → real-world case → scenario → task structure without redesigning the lab.

---

## 📚 References

- [Nmap Reference Guide](https://nmap.org/book/man.html)
- [IANA Port Number Registry](https://www.iana.org/assignments/service-names-port-numbers/service-names-port-numbers.xhtml)
- [curl Documentation](https://curl.se/docs/)
- [OWASP — Information Exposure via HTML Comments](https://owasp.org/www-community/attacks/Information_disclosure)
- [Samba / smbclient Docs](https://www.samba.org/samba/docs/current/man-html/smbclient.1.html)
- [OWASP SQL Injection Prevention Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/SQL_Injection_Prevention_Cheat_Sheet.html)
- [OWASP Top Ten — A03:2021 Injection](https://owasp.org/Top10/A03_2021-Injection/)
- [NIST SP 800-63B — Digital Identity Guidelines](https://pages.nist.gov/800-63-3/sp800-63b.html)
- [THC-Hydra (GitHub)](https://github.com/vanhauser-thc/thc-hydra)
- [RFC 959 — File Transfer Protocol](https://www.rfc-editor.org/rfc/rfc959)
- [steghide Documentation](https://steghide.sourceforge.net/documentation.php)
- [OpenSSH Manual](https://www.openssh.com/manual.html)
- [pfSense Documentation](https://docs.netgate.com/pfsense/en/latest/)
- [MITRE ATT&CK — T1041 Exfiltration Over C2](https://attack.mitre.org/techniques/T1041/)
- [CISA AA20-352A — SolarWinds Advisory](https://www.cisa.gov/news-events/cybersecurity-advisories/aa20-352a)
- [John the Ripper Documentation](https://www.openwall.com/john/doc/)
- [GnuPG Documentation](https://www.gnupg.org/documentation/)
- [NIST FIPS 197 — AES](https://csrc.nist.gov/pubs/fips/197/final)
- [GNU tar Manual](https://www.gnu.org/software/tar/manual/tar.html)
- [CISA — Coordinated Vulnerability Disclosure](https://www.cisa.gov/coordinated-vulnerability-disclosure-process)
- [OWASP Web Security Testing Guide](https://owasp.org/www-project-web-security-testing-guide/)

---

<div align="center">

*Built as an academic cybersecurity project under the supervision of Dr. Mohamed Saeed.*

</div>
