---
hide:
  - navigation
  - toc
---

## The OpenDNSSEC project

OpenDNSSEC is a policy-based zone signer that automates the process of keeping track of DNSSEC keys and the signing of zones. The goal of the project is to make DNSSEC easy to deploy. The project is Open Source and intends to drive adoption of Domain Name System Security Extensions (DNSSEC) to further enhance Internet security.

## OpenDNSSEC 2.1.14

Version 2.1.14 of OpenDNSSEC has been released on 2024-08-22.

**News**

This is a mainenance release that fixes some bugs and adds robustness for HSM outages.  Apart from a minor fix to the backup keys command and export keys, it solved an issue where keys were not published soon enough in special cases in combination with <SharedKeys> directive.  In case you use shared keys, you must update.  But this is a good idea anyway.

**Download**

- https://dist.opendnssec.org/source/opendnssec-2.1.14.tar.gz
- https://dist.opendnssec.org/source/opendnssec-2.1.14.tar.gz.sig
- Checksum SHA256: 5a68d62ea0ea3a6c61e9f4946f462c7b907fbe6bccc9e8a721b7fe0f906f95d0
