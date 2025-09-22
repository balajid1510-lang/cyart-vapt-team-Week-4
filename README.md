# cyart-vapt-team-Week-4
cyart-vapt-team — Week 4 README

Important: Everything in this repository documents lab-only activities performed in isolated, permissioned environments (VulnHub / TryHackMe / HackTheBox). Do NOT run anything in production or against systems you do not own or have explicit written permission to test.

Overview

This folder contains deliverables for Week 4 of the VAPT engagement exercises. It includes evidence, reports, checklists, and high-level reproduction steps for the following labs:

Advanced Exploitation Lab

API Security Testing Lab

Privilege Escalation & Persistence Lab

Network Protocol Attacks Lab

Mobile Application Testing Lab

Capstone: Full VAPT Engagement

Each lab entry contains a Conceptual Test Log, non-destructive reproduction notes, evidence (screenshots, pcaps, logs), and remediation recommendations. All exploit code, PoCs, or destructive scripts must remain in a private area and must not be published publicly.

Safety, Scope & Permissions

Tests were executed only in isolated lab environments (host-only / internal networks). No external or production-facing systems were targeted.

Snapshots/checkpoints were taken before destructive actions; every destructive action was reverted after evidence collection.

Only authorized lab VMs (VulnHub/THM/HTB with valid access) were used.

Any sensitive artifacts (exploits/PoCs) are stored in the private/ folder (access-restricted) if applicable.


Note: Keep private/ folder non-public. Do not include raw exploit code in public folders.

Naming & Evidence Conventions

Filenames MUST include ISO timestamps and IDs. Example: screenshot_007_2025-09-01T15-00-00.png

PCAP files: pcap_<testID>_<timestamp>.pcap

Logs: toolname_<testID>_<timestamp>.log (e.g., linpeas_010_2025-09-02T11-20-00.log)

Reports: Final reports exported as PDF and stored under reports/.

High-level reproduction workflow (for each lab)

These are conceptual, non-actionable steps meant for lab reproduction only.

Setup

Restore clean snapshots of attacker & target VMs.

Confirm both VMs are on an isolated host-only/internal virtual network.

Ensure time sync between attacker and target for timestamp correlation.

Recon & Enumeration

Identify available services and endpoints at a high level.

Document service versions and banner information in evidence/logs/.

Proof-of-concept (non-destructive)

Design low-impact PoC or demonstration checks; capture outputs. Store any PoC notes only in private/.

Evidence capture

Take screenshots of significant results.

Capture network traffic as PCAP when relevant.

Save terminal session logs and export scanner results.

Restore & Cleanup

Revert any destructive changes by restoring snapshots.

Move evidence to the evidence/ folder and finalize reports.

Reporting

Produce an individual lab report and append to reports/.

Combine findings into the PTES-style final report and stakeholder briefing.

Reporting requirements (per lab)

Each lab report must contain:

Title and objective

Test scope & lab IPs (e.g., 192.168.x.x) and tool versions

High-level methodology (non-actionable)

Conceptual findings (do NOT include raw exploit commands)

Evidence index (screenshots, pcaps, logs) with filenames and timestamps

Severity rating and impact rationale

Remediation recommendations (patching, configuration, detection)

Checklists (what to ensure before submission)

 All evidence files are timestamped and present in evidence/.

 PTES_report.pdf exists in reports/ and follows the Executive Summary → Timeline → Remediation structure.

 Non-technical stakeholder briefing (150 words) is present and saved in reports/.

 All checklists completed and stored in checklists/.

 Repository contains a README with reproduction notes and safety statement.

Naming & Ticketing (optional team workflow)

Use Test IDs for cross-referencing: e.g., 007, 008, 010, 015, 016.

Add a short description and link to evidence in the issue tracker or team board.

Deadline & Submission

Deadline: September 30, 2025 — 17:30 (local time)

Submission steps:

Ensure all reports and evidence are in Week 4/.

Export final reports to PDF and add them to reports/.

Create a Git tag week4-final and push to the team remote repository. (If repo is private, invite reviewers.)

Contributors & Contacts

Primary owner: your-github-username (replace with repo owner)

Team reviewers: list team members and their roles (scanning, reporting, validation)

License & Distribution

This repository contains internal lab documentation and should be treated as restricted. Do not publish sensitive artifacts or exploit code publicly. Consider adding a LICENSE file appropriate to your organization (e.g., internal use only).
