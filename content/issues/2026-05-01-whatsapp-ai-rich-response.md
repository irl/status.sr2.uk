---
title: WhatsApp Malicious Messages
date: 2026-05-01 09:00:00
severity: notice
informational: true
section: issue
affected:
  - Link Helpdesks
---

A [WhatsApp security advisory](https://www.whatsapp.com/security/advisories/2026) announced a discovered vulnerability,
tracked as [CVE-2026-23866](https://app.opencve.io/cve/CVE-2026-23866), arises from incomplete validation of AI rich
response messages that contain Instagram Reels references within WhatsApp.

This vulnerability allows a malicious user to craft a message that triggers the victim’s device to fetch and process
media content from an external URL.
In some cases, the media content may invoke OS‑controlled custom URL scheme handlers,
potentially executing arbitrary code or launching unintended applications.
The CVSS score of 4.3 indicates moderate impact and a non‑zero but limited likelihood of exploitation.

We have confirmed via MDM that all Android handsets operated by SR2 Communications have since upgraded to unaffected
versions.

**If you self-manage your handset for your Link helpdesk's WhatsApp channel it is your responsibility to follow vendor
security advisories and ensure that the handset operating system and applications are secured and regularly patched.**

As always, if you have any concerns please [contact our helpdesk](https://www.sr2.uk/support).
