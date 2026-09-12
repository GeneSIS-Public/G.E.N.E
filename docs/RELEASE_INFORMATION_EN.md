# G.E.N.E Alpha v1.0 — Release Information

- **Document Version:** v0.5
- **Status:** Active — Public Release
- **Published By:** GeneSIS
- **Operating Entity:** GeneSIS-Operator
- **Project:** Project: Code-NOAH
- **Phase:** Phase 1
- **Product Line:** G.E.N.E v1.x
- **Current Release:** G.E.N.E Alpha v1.0
- **Public Release Date:** `2026-07-31`
- **Target Platform:** Windows x64
- **Build:** `G.E.N.E_Alpha_v1.0_R10-4D-4_Build-005`
- **Official Distribution URL:** https://genesis-protocol.booth.pm/items/8663637
- **Established:** 2026-07-31
- **Effective From:** 2026-07-31
- **Last Updated:** 2026-09-11

> The Japanese version of this document is the original and authoritative version. If any inconsistency or difference in interpretation arises between this translation and the Japanese version, the Japanese version governs to the extent permitted by applicable law.

## 1. Release Overview

| Item | Information |
|---|---|
| Product | `G.E.N.E Alpha v1.0` |
| Project | `Project: Code-NOAH` |
| Phase | `Phase 1` |
| Product Line | `G.E.N.E v1.x` |
| Platform | `Windows x64` |
| Build | `G.E.N.E_Alpha_v1.0_R10-4D-4_Build-005` |
| Distribution Format | ZIP archive |
| Distribution Channel | Official GeneSIS BOOTH |
| Price | Free |
| Functional Difference Based on Support Status | None |
| Source Code | Not publicly released |

Official archive name:

```text
G.E.N.E_Alpha_v1.0_Windows_x64.zip
```

For the archive size, SHA-256, Release Identity, and verification procedure, use [Release Verification](./RELEASE_VERIFICATION_EN.md) as the authoritative source.

## 2. What G.E.N.E Is

G.E.N.E is a local AI dialogue environment for Windows x64 that records and operates AI dialogue as a local asset while preserving speaker identity, origin, original text, and context rather than treating dialogue as a temporary chat.

Its central concept is:

> AIが変わっても、あなたの対話と思考まで失う必要はない。  
> 人間側に、AIとの継続性を作る。

G.E.N.E provides an environment for users to manage Personas, History, Summaries, Knowledge, and References within their own environment.

G.E.N.E is not an LLM. Text generation requires a separate external local LLM environment, such as Ollama, and an available model.

## 3. External Environment and User Responsibilities

Unless expressly stated otherwise, the G.E.N.E application archive does not include an external local LLM environment, models, or the computer resources required to operate them.

Users are responsible for:

- Installing and configuring the external local LLM environment
- Obtaining and selecting models
- Confirming suitability for the user's hardware and intended use
- Complying with licenses and terms for external software and models
- Securing the local computer and connected environment
- Backing up important data

Performance, output quality, language ability, and behavior vary depending on the operating system, hardware, runtime, model, and settings.

G.E.N.E does not guarantee identical operation or answers across all combinations.

For current limitations, unverified areas, and usage notes, see [Known Limitations](./KNOWN_LIMITATIONS_EN.md).

## 4. Local Operation and Data

G.E.N.E is designed for local operation.

During ordinary use, GeneSIS does not automatically collect conversation history, Personas, Summaries, Knowledge, References, prompts, or input to and output from a connected model stored or processed through G.E.N.E.

Information voluntarily submitted for a defect report or inquiry is handled only within the scope submitted.

Connected external software, models, or services may have their own network behavior, terms, or information-handling practices.

For details, see the [Privacy Notice](./PRIVACY_NOTICE_EN.md).

## 5. Meaning of Alpha v1.0

G.E.N.E Alpha v1.0 is the first official public release in Project: Code-NOAH Phase 1.

`Alpha` does not mean an unofficial prototype, an unfinished package, or an incomplete implementation.

The minimum G.E.N.E specification defined for this release has been implemented and tested, and the official archive has been fixed.

The following areas, however, remain at an early stage:

- Operational history after public distribution
- Accumulation of supported-environment and compatibility information
- Combination testing with external runtimes and models
- Environment-specific behavior in user systems
- Maturity of public documentation and specification explanations

The following distinctions therefore apply:

```text
Implementation complete
is not the same as
the entire Project roadmap being complete.

Official release
is not the same as
defect-free or compatible with every environment.

Alpha
is not the same as
an unofficial prototype.
```

Unidentified defects, environment-specific behavior, or specifications adjusted in a later release may exist.

## 6. Free Distribution and Founder Support

The G.E.N.E Alpha v1.0 application is distributed free of charge.

Payment, Founder Support participation, BOOST, or other additional support does not change the functions, available scope, or basic support scope of the corresponding G.E.N.E application.

The G.E.N.E application archive in the free distribution and the initial Founder package has the same build and SHA-256.

Founder Support is not the purchase of an upgraded edition of G.E.N.E. It is express participation in and support for Project: Code-NOAH Phase 1.

For formal conditions concerning Founder status, price, Founder Deliverables, Supplemental / Additional Deliverables, non-guaranteed delivery timing, and other Founder conditions, use the Japanese Founder Terms TXT included in the Current Founder Initial Package as authoritative. The GitHub [Founder Terms](./FOUNDER_TERMS_EN.md) are an English Reference Translation for pre-purchase review.

Current Founder Deliverables, Supplemental / Additional Deliverables, later deliverables, and related documents are consolidated in [Founder Support Information](./FOUNDER_SUPPORT_INFORMATION_EN.md).

Founder Support product page:

https://genesis-protocol.booth.pm/items/8664431

## 7. Distribution Policy

Official distribution of G.E.N.E Phase 1 / v1.x takes place through the G.E.N.E free-product page on the official GeneSIS BOOTH shop.

```text
https://genesis-protocol.booth.pm/items/8663637
```

This product page is operated as the continuing official distribution page for G.E.N.E Phase 1 / v1.x.

Later v1.x releases will be added as separately versioned files.

An existing official archive will not be silently replaced under the same filename.

The G.E.N.E free-product page distributes official G.E.N.E v1.x releases. Founder Deliverables and Supplemental / Additional Deliverables under Founder Support are handled separately under the Founder Support terms and delivery route. Review Founder Support Information for the current delivery scope.

## 8. Official Information Sources

### BOOTH

BOOTH is the medium for official G.E.N.E distribution, Founder Support acceptance, and purchase records.

- G.E.N.E free distribution: https://genesis-protocol.booth.pm/items/8663637
- Founder Support: https://genesis-protocol.booth.pm/items/8664431

### GitHub

This Repository is the official technical medium for fixed technical information, release information, verification information, Known Limitations, and public documents concerning G.E.N.E.

GitHub is not the authoritative source for payment, purchase records, or Founder status.

### Contact

Use GitHub Issues for publicly shareable ordinary defects. Use the routes described in [Contact and Support](./CONTACT_AND_SUPPORT_EN.md) for purchases, Founder verification, rights, privacy, and other non-public matters.

Use the private route in the [Security Policy](../SECURITY_EN.md) for unresolved security issues.

## 9. Source Repository, Distribution Format, and Terms

The G.E.N.E source repository is not publicly available.

G.E.N.E is distributed as an executable application archive. Standalone Python source files, the development environment, build scripts, and internal development history are not separately provided as user-facing deliverables.

Publication of the application archive, documentation, release information, or verification values does not grant access to the source repository, a right to obtain source code, or a license to use source code.

The G.E.N.E Alpha v1.0 EULA is available [here](./EULA.md) as a pre-download review copy. The linked EULA is the Japanese authoritative text.

Use of the G.E.N.E application is governed by `EULA.txt` included in the official distribution archive. If any difference exists between the GitHub copy and the EULA in the official distribution archive, `EULA.txt` in the official distribution archive governs.

This document does not replace the EULA.

---

Copyright © 2026 GeneSIS: Concept Engineer's HQ. All rights reserved.
