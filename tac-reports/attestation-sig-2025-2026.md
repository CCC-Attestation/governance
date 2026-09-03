---
footer: CCC Attestation SIG - TAC Update - Sep 2026
slidenumbers: true
autoscale: true
theme: Next
---

# Attestation SIG

## Year in review

### Confidential Computing Consortium - TAC - September 2026

---

# About the SIG

- **Mission:** advance attestation for confidential computing through open community discussion, shared understanding, and practical interoperability.
- **Cadence:** public meetings every **two weeks**, Tuesdays 9:00 AM PDT.
- **Chairs:** Chong Cai, Jim Beaney, Thomas Fossati, Greg Kostal.
- **Sources of record:**
  - [Meeting agenda & minutes](https://docs.google.com/document/d/1NkiS78knPhDO0vA9ElS-bQOHNu783gGPdmTEbbOoOOU/)
  - [Meeting materials repo](https://github.com/CCC-Attestation/meetings)
  - [Issue tracker](https://github.com/CCC-Attestation/meetings/issues)

---

# Reporting period

## August 2025 to August 2026

[.column]
### Activity at a glance
- **~25 meetings** held (1 cancelled: 2025-11-04, IETF conflict)
- **26 presentations** catalogued in the meeting-materials table
- **6 active tracks** in regular rotation
- **13 open issues** on the tracker (several multi-track)

[.column]
### Community engagement
- Consistent cross-vendor attendance (AMD, Arm, Google, Intel, Microsoft, NVIDIA, Oracle, ...)
- Recordings on the [YouTube playlist](https://www.youtube.com/playlist?list=PLmfkUJc39uMhZsNGmpx-qD-uCoQyMglIp)
- Active Slack `#attestation` and mailing list

---

# How we organise work

The SIG uses **tracks** to structure recurring themes. Presentations are tagged in the [meeting materials table](https://github.com/CCC-Attestation/meetings#meeting-materials).

| Track | Focus |
| --- | --- |
| **Information & data models** | CoRIM, EAT, endorsements, reference values, attestation results |
| **Secure channel establishment** | Attested TLS, binding properties, formal analysis |
| **Composite attesters** | Multi-RoT, layered evidence, cryptographic binding |
| **OSS software stacks** | Evidence collection, verifier tooling, kernel ABIs |
| **Emerging standards** | IETF RATS alignment, workload identity, new profiles |
| **Attestation architectures** | End-to-end deployment patterns and services |

---

# Track highlights

## Past year by theme

---

# Information & data models

*Largest share of meeting time this year.*

---

### Delivered

- **CoRIM 101** - 3-part tutorial on the data model & reference verifier (Jul–Aug 2026) - Thomas Fossati
- **CoRIM modeling, evolution & revocation** (Oct 2025) - Dhawal Kumar
- **EAT profile for device attestation** (Sep 2025) - Mathieu Poirier & Thomas Fossati
- **CoSERV** - selector for endorsements & reference values; Veraison integration (Jun–Jul 2025, follow-up Jun 2026) - Paul Howard
- **Endorsement distribution with Veraison & CoSERV** (Jun 2026) - Paul Howard
- **OCP device attestation / EAT profile** (Feb 2026) - Giri Mandyam et al.
- **Disk identity & integrity for confidential deployments** (Mar & Jun 2026) - Pushkar Chitnis
- **TrustMee** - self-verifying remote attestation evidence (Apr–May 2026) - Lachlan Gunn et al.
- **Platform ownership endorsement (PoE)** discussion started (Jun 2026) - Benny Fuhry

Note: IETF recently published RFC 9999 (RATS Conceptual Message Wrappers), which started in the SIG.

---

### In flight
- Issue **#56** - deeper CoRIM dive (optional triples, profiles, verifier algorithm)
- Issue **#51** - endorsement distribution APIs
- Issue **#40** - registering media types for attestation formats
- Issue **#67** - endorsement freshness techniques & best practices

---

# Secure channel establishment

*Continued exploration on Attested TLS and related binding questions.*


---

### Delivered
- **Attested TLS - yearly SIG project update** (Aug 2025) - Ionut Mihalcea & Thomas Fossati
- **Comprehensive formal analysis of Attested TLS** (Oct 2025) - Muhammad Usama Sardar
- **Binding properties for Attested TLS** (Dec 2025) - Muhammad Usama Sardar
- **Attested DNS** (Jul 2026) - Amaury Chamayou
- Sustained discussion threads on identity binding, post-handshake models, and open challenges (2025–2026)

New IETF SEAT WG chartered; SEAT is **the** place where to discuss attested TLS

---

# Composite attesters

*New track formalised in 2025; growing body of shared knowledge.*

---

### Delivered
- **Azure vTPM attestation & binding** (Jul 2025 + Q&A Aug 2025) - Mike Stunes
- **Binding TDISP & platform attestation reports for CVMs** (Jul 2025) - Anna Trikalinou
- **RATSD** - standard evidence-collection package; lead-attester model (Sep 2025) - Jag Raman & Ian-chin Wang
- **Cryptographic binding of evidence from multiple attesters** - community request addressed (Aug 2026, issue **#82**)

---

### In flight
- Issue **#62** - uber tracking issue; [shared document](https://docs.google.com/document/d/1eyO0oIamwYYaaingCmSpI8CNvCKmV-86Hv3GKs4Cn54) collecting patterns & gaps (now moved to IETF RATS [draft-richardson-rats-composite-attesters](https://datatracker.ietf.org/doc/draft-richardson-rats-composite-attesters/))
- Issue **#55** - Azure confidential VM composite attestation (delivered; doc ongoing)
- Issue **#29** - "standard package" for evidence collection (RATSD is first concrete step)

---

## OSS software stacks

---

### Delivered
- **RATSD** evidence-collection daemon (Sep 2025) - Oracle
- **CoSERV / Veraison** prototyping for endorsement distribution (2025–2026) - Arm
- Linux **configfs-tsm** ABI presented & closed (2024; still referenced in composite discussions)

---

### In flight
- Issue **#29** - converge on a community-endorsed evidence-collection package
- Issue **#25** - Confidential Containers attestation service (Trustee / KBS)
- Issue **#51** - endorsement distribution APIs (OSS + data-model crossover)

---

## Emerging standards & architectures

---

### Delivered
- **Trustworthy workload identity with RATS** (Nov 2025) - Mark Novak - TWI and RATS harmonisation
- **ELASTIC project** - unified remote attestation (May 2025) - Anne-Marie Praden
- **Attestation flow on s390** (architectures track, prior year; still cited in composite work)

---

### In flight
- Issue **#72** - contextual assessment of attestations / mitigating forgeries *(TAC-requested topic)*
- Issue **#21** - position paper on machine identity vs. code identity
- Issue **#23** - Intel Trust Authority deep dive (requested)
- Issue **#48** - use cases for attestation (Mike Bursell, backlog)

---

# Overlapping themes

[.column]
### Standards alignment
- Deep engagement with **IETF RATS** (CoRIM, EAT, CMW, geographic results)
- **OCP** device-attestation EAT profile
- **GRC SIG** governance-pattern documents reviewed & ACK'd (#52)

[.column]
### Operational attestation
- Endorsement **distribution**, **freshness**, and **revocation**
- **Contextual** verification (geo, network, datacenter factors)
- **Workload identity** stable across TEE migration

---

## Issue tracker snapshot

---

### Closed this period
| # | Title | Track |
| --- | --- | --- |
| 82 | Cryptographic binding of evidence from multiple attesters | Composite attesters |
| 17 | Workload identity in attestation results | Info & data models |
| 22 | Composite attester/device description | subsumed by #62 |
| 52 | GRC governance patterns review & ACK | - |
| 53 | Assurance models for machine/workload identity | - |

---

### Open & active (selected)
| # | Title | Track(s) |
| --- | --- | --- |
| 62 | Composite attesters (uber issue) | Composite |
| 56 | Deeper dive into CoRIM | Info & data models |
| 72 | Contextual assessment / forgery mitigation | TAC topic |
| 67 | Endorsement freshness best practices | Info & data models |
| 51 | Endorsement distribution APIs | Info & data models, OSS |
| 29 | Standard evidence-collection package | Composite, OSS |

---

# Governance & community

- **Co-chair transition:** Chong Cai succeeded Keith Moyer (announced Jan 2026).
- **GRC collaboration:** Attestation SIG reviewed Verifier / Endorser / Attester governance docs.
- **TAC engagement:** Issue **#72** originated from a TAC request for attestation-in-context patterns.
- **Trustee / CoCo KBS** awareness raised at TAC (Dec 2025); community feedback solicited.
- **Funding:** SIG members continue to pursue dedicated funding for cross-vendor collaboration & workshops.

---

## Planned activity

---

### Scheduled
| Date | Topic |
| --- | --- |
| **2026-09-22** | Yogesh Deshpande - **Arm CCA CoRIM profile** |

---

### Backlog (near term)
- **CoRIM 101** - optional triples and profiles (follow-up to Aug 2026)
- **Intel PoE** - Platform Ownership Endorsements standardisation path
- **Dhawal Kumar** - CoRIM modeling follow-up (started Oct 2025)
- **Composite attesters** - continue shared doc; more deployment deep-dives
- **Endorsement freshness** (#67) - community best-practices session
- **Contextual attestation patterns** (#72) - reference guidance document

---

# SIG objectives alignment

The SIG continues to pursue its standing goals:

1. **Interoperability** - common data models (CoRIM, EAT), evidence packaging (RATSD), distribution (CoSERV/Veraison)
2. **Shared understanding** - composite attesters, binding models, attestation-in-context
3. **Secure channels** - Attested TLS formalisation & reference implementations
4. **Community onboarding** - tutorial content (CoRIM 101), public recordings, open issue tracker
5. **Standards convergence** - active liaison with IETF RATS, OCP, GRC, TWI SIG

---

# Thank you

### Questions & discussion

**Attestation SIG**
- Agenda: [Google Doc](https://docs.google.com/document/d/1NkiS78knPhDO0vA9ElS-bQOHNu783gGPdmTEbbOoOOU/)
- Materials: [github.com/CCC-Attestation/meetings](https://github.com/CCC-Attestation/meetings)
- CCC Slack: [#attestation](https://confidentialcomputing.slack.com/archives/C01QZ3K1APM)
- Mailing list: [<attestation@lists.confidentialcomputing.io>](mailto:attestation@lists.confidentialcomputing.io)
