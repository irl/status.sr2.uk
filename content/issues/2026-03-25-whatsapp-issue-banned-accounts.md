---
title: WhatsApp Message Send Issue
date: 2026-03-25 03:00:00
resolved: true
resolvedWhen: 2026-03-31 16:15:00
# Possible severity levels: down, disrupted, notice
severity: notice
affected:
  - Link Helpdesks
section: issue
---

**Resolved**: This issue appears to only affect cases where no conversation history exists with the contact the message
is sent to.
Due to the nature of the helpdesk, messages are only sent to users that have already sent a message to the helpdesk, so
we do not believe this issue will affect our users.
We encourage you to get in touch if you do see any issues with your WhatsApp channel however we are no longer monitoring
this situation closely.
{{< track "2026-03-31 16:15:00" >}}

**Monitoring**: We are not aware of this issue affecting any helpdesk currently however we continue to monitor.
A fix has been found by the upstream project and will be rolled out once released formally.
{{< track "2026-03-27 15:00:00" >}}

**Monitoring**: We have been made aware of an issue with the WhatsApp integration that we use where for some accounts,
mostly accounts that have been banned and subsequently unbanned, users are noticing errors on message send.
A fix is being investigated by the integration developer.
Technical details can be followed on GitHub at https://github.com/WhiskeySockets/Baileys/issues/2441.
{{< track "2026-03-25 03:00:00" >}}
