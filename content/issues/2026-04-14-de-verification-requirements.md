---
title: Updated .de verification requirements
date: 2026-04-14 00:00:00
#resolved: true
#resolvedWhen: 2017-12-17 16:58:00
# Possible severity levels: down, disrupted, notice
severity: notice
informational: true
affected:
  - Other Registries
section: issue
---

In order to comply with NIS2, DENIC, the registry for .de, has introduced new registrant verification requirements,
effective April 14, 2026.

## What’s changing

**Risk-based verification can result in domain deletion.**

DENIC will begin flagging potentially invalid or suspicious registrant data and require it to be verified.

Here's how the process will work:

When a registrant's data is flagged, they will receive an email requesting that they use the link provided to upload the verification documents.
If they don't provide the verification documents within 30 days:

- Their domain(s) will be suspended (DNS will stop working).
- Their domain(s) will enter a 90-day quarantine period.

During the 90-day quarantine, they can complete verification to lift the suspension and reactivate their domain.
If verification is not completed within 90 days, all associated domain names **will be permanently deleted**.

## How to correct inaccurate data

Once a registrant has been flagged for verification, any inaccurate data can be corrected by processing:

- an owner change (in cases where the email address must be changed or the registrant name must be substantially modified)
- a contact update (in cases where a minor change to the registrant name or other data must be made)

Once the data has been updated, the new data must be verified within the original 30-day period.
Failed email verification may trigger risk-based verification.

Starting April 14, 2026, if a registrant fails to complete email verification, it may trigger an expedited risk-based verification process:

- The registrant will have 7 days (rather than 30) to provide the requested verification documents.
- After 7 days, the domain will be suspended and enter the 90-day quarantine period if verification has not been completed.
- At the end of the 90-day quarantine period, all associated domain names will be permanently deleted.

## Get support

If you receive an email asking you to verify your details and do not know how to proceed, reach out to our support service
by emailing contact@sr2.uk.