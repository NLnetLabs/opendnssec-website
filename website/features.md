---
hide:
  - navigation
  - toc
---

### Overview

- Single piece of software for signing DNS zones that can be seamlessly integrated into an existing system without needing to overhaul the entire existing infrastructure.
- Can be configured to sign zone files or to sign zones transferred in via AXFR.
- Fully automatic – once set up, no manual intervention is needed.
- Possibility of manual key rollover (emergency key rollover).
- Open source software supplied with a BSD license so suppliers of commercial products can use the open source code in them whilst retaining the IPR of their own software.

### Scalable

- Able to sign zones containing anything from a few records up to millions of records.
- Single instance of OpenDNSSEC can be configured to sign one or many zones.
- Keys can be shared between zones inorder to save space in the HSM.

### Flexible

- Able to define zone signing policy (length of key, key lifetime, signature interval etc.); can set the system up for anything between one policy to cover all zones to one policy per zone.
- Works with all different versions of the Unix operating system

### Secure

- OpenDNSSEC stores sensitive cryptographic data in an HSM, communicating with it using the industry-standard PKCS#11 interface.
- SoftHSM – a software emulation of an HSM – is available if use of an HSM is not necessary, or to set up a DNSSEC testbed before purchasing a real HSM.
- Facility to check whether HSMs are compatible with OpenDNSSEC.
- Includes an auditing function that compares the incoming unsigned zone with the outgoing signed zone, so you can check that no zone data has been lost and that the zone signatures are correct.
- Supports RSA/SHA1 and SHA2 signatures
- Denial of existence using NSEC or NSEC3
