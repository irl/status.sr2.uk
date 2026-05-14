---
title: Dirty Frag (CVE-2026-43284, CVE-2026-43500)
date: 2026-05-08 09:00:00
# Possible severity levels: down, disrupted, notice
severity: notice
informational: true
section: issue
---

Similar to the recent [copy.fail incident](https://status.sr2.uk/issues/2026-04-29-copy-fail/), another local
privilege escalation vulnerability had been
[discovered in the Linux Kernel](https://www.openwall.com/lists/oss-security/2026/05/07/8).
We learned of this via our threat intelligence feeds on the 8th of May.

None of our systems had the affected kernel modules loaded and so exploitation was not possible.
To verify this we use Ansible:

```yaml
    - name: Verify CVE-2026-43284 and CVE-2026-43500 mitigation
      ansible.builtin.command: "lsmod | grep -E '^{{ item }}\\s'"
      loop:
        - esp4
        - esp6
        - rxrpc
      register: module_check
      failed_when: module_check.rc != 1
      changed_when: false
      check_mode: false
```

Our server systems are patched weekly and so we expect the affected modules to be updated in due course.

As always, if you have any concerns please [contact our helpdesk](https://www.sr2.uk/support).
