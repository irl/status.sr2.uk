---
title: Onion Services outage during move to self-signed certificates and software upgrades
date: 2026-10-25T14:00:00+00:00
resolved: true
resolvedWhen: 2026-10-25T17:20:00+00:00
severity: down
affected:
  - Onion Services
section: issue
---

*Resolved* - Onion service hosting has been restored. All onion services are now served with self-signed TLS certificates on the upgraded software stack. {{< track "2026-10-25T17:20:00+00:00" >}}

*Investigating* - Onion services are unavailable while we change how TLS certificates are issued for them and upgrade the hosting software. {{< track "2026-10-25T14:00:00+00:00" >}}

## What changed

**Certificates.** Onion services now use self-signed certificates and no longer use certificates from the public WebPKI. Publicly trusted certificate lifetimes keep getting shorter, and we do not have the capacity to keep WebPKI certificates renewed reliably across our onion services. With a self-signed certificate the connection is still encrypted and authenticated end to end by the onion service protocol, because the .onion address is itself derived from the service's key. Browsers that are not Tor Browser may show a certificate warning.

**Software.** We upgraded Onionspray, together with its bundled OpenResty and the C Tor (tor) daemon, to new releases that include recent security fixes.

## Gobalance

We do not use Gobalance in this service, so the recently disclosed Gobalance vulnerability did not affect our services, or pose any risk to the Onion service private keys.