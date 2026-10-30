---
title: Hypervisor reboots for Linux kernel vulnerability (CVE-2026-98432)
date: 2026-10-29 14:38:00
resolved: false
# resolvedWhen: 2026-10-29 00:00:00
# Possible severity levels: down, disrupted, notice
# Switch to "disrupted" (degraded) when remediation begins
# severity: disrupted
severity: notice
affected:
  - Link Helpdesks
  - Onion Services
  - Virtual Servers
section: issue
informational: true
---

*Update* - Having assessed this vulnerability against our infrastructure, we have determined that it is not exploitable.
The planned reboots have therefore been postponed. We will post a further update here once we have scheduled the reboots. {{< track "2026-10-30 08:40:00" >}}

---

A flaw has been disclosed in the Linux kernel's IPv4 TCP implementation ([CVE-2026-98432](https://access.redhat.com/security/cve/cve-2026-98432)) that could allow a remote attacker to crash an affected system.

To remediate this, we will need to update the kernel and reboot our virtual machine hypervisors. We anticipate that services hosted on each hypervisor may be unavailable for up to 30 minutes while it is rebooted.

We will update this issue when remediation begins.