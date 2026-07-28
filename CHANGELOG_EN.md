# Changelog

- **Document Version:** v0.2 Final Draft
- **Language:** English
- **Document Role:** Provisional English Draft / Future Official Translation
- **Status:** Draft — Pending Public Release
- **Planned Authoritative Version:** Japanese version to be published during final document alignment
- **Project:** Project: Code-NOAH
- **Product:** G.E.N.E
- **Maintained By:** GeneSIS

> **This changelog is a public-release preparation draft.**  
> It does not, by itself, indicate that G.E.N.E Alpha v1.0 has entered public distribution.  
> The Japanese version is planned to become the original and authoritative version during final document alignment.

This file records public release-level changes for G.E.N.E.

Internal development activity, private source history and every intermediate build are not necessarily included.

## Change Classification

This changelog uses the following categories where applicable:

- **Added:** New public functions, packages, documents or supported behavior.
- **Changed:** Changes to existing public behavior, structure or conditions.
- **Fixed:** Confirmed defects corrected in the release.
- **Deprecated:** Functions or behavior planned for removal.
- **Removed:** Functions, files or behavior removed from the public release.
- **Security:** Publicly disclosable Security-related changes.
- **Documentation:** Public Documentation additions or revisions.
- **Release Metadata:** Build, archive and verification-record information.

An item is included only when GeneSIS has sufficient information to describe it publicly.

## [Unreleased]

No later public release changes are recorded at this time.

Future changes will be added here after they are confirmed for public documentation.

## [G.E.N.E Alpha v1.0] — Pending Public Release

### Release Metadata

| Item | Value |
|---|---|
| Product | `G.E.N.E Alpha v1.0` |
| Platform | `Windows x64` |
| Build | `G.E.N.E_Alpha_v1.0_R10-4D-4_Build-005` |
| Archive | `G.E.N.E_Alpha_v1.0_Windows_x64.zip` |
| File Size | `79,504,332 bytes` |
| Archive SHA-256 | `420db62dbb6763aebe01a5e0ab0225ebdafdb9bc6ec471e45098d2e812d3ffea` |
| Release Identity SHA-256 | `1ac70e76edc2225e69f80d33b4bb60c2d01bb8fd135b14e4cdb8bae7367cbcc9` |
| Release Record Signed Date | `2026-07-21` |
| Release Archive Verification Status | `PASS` |
| Public Release Date | Pending |
| Distribution Channel | Official GeneSIS BOOTH |
| Price | Free |
| Source Code | Not publicly released |

`PASS` means that the canonical release archive record and the recorded archive-copy verification completed successfully.

It does not mean that the Alpha release is defect-free, compatible with every environment or suitable for every purpose.

The Release Record Signed Date refers to the GeneSIS release-evidence record associated with this archive.

It does not, by itself, indicate Microsoft Authenticode or another operating-system code-signing status.

The values in this changelog are recorded as a historical release summary.

For archive identity, file size, SHA-256 values and verification procedures,  
[Release Verification](./docs/RELEASE_VERIFICATION.md) is the authoritative technical record.

### Added

- Prepared the initial G.E.N.E Alpha v1.0 release package for Windows x64.
- Established G.E.N.E as a local AI dialogue environment that connects to a separately managed external local LLM environment.
- Established the initial public Release identity and archive-verification record.
- Established free access to the same official G.E.N.E application package without payment-based feature restrictions.
- Established the initial public Documentation structure for Release, verification, limitations, Support, Security, Privacy and Founder-related conditions.

### Product Position

G.E.N.E Alpha v1.0 is an Alpha-stage local AI dialogue environment.

G.E.N.E is not a Large Language Model and does not generate AI responses by itself.

A separately installed and configured external local LLM environment and compatible model are required.

The central product concept is:

> AIが変わっても、あなたの対話と思考まで失う必要はない。  
> 人間側に、AIとの継続性を作る。

G.E.N.E is intended to create continuity on the user-controlled side.

Stored context and settings do not guarantee identity equivalence, identical output or identical behavior between different models.

### Distribution

The G.E.N.E Alpha v1.0 application package is planned for free distribution through the official GeneSIS BOOTH channel.

Founder Support is optional and does not change or unlock functions in the corresponding G.E.N.E application package.

BOOTH purchase records are used for Founder qualification where applicable.

GitHub is used for official Release information, verification values, Documentation and public technical policies.

The official BOOTH product URL will be added before public distribution begins.

### Documentation

The following public Documentation has been prepared or established for this release:

- Repository README
- Security Policy
- Contact and Support
- Common Support Policy
- Founder Support Terms
- Privacy Notice
- Release Verification
- Release Information
- Known Limitations
- Changelog

Some documents remain Drafts and do not become effective merely because they are present in the Repository.

Applicable dates, public URLs and final language-version relationships will be completed during final release alignment.

### Known Limitations

G.E.N.E Alpha v1.0:

- targets Windows x64;
- requires an external local LLM environment;
- does not guarantee compatibility with every model, runtime version or hardware configuration;
- does not guarantee identical output or behavior across models;
- does not provide GeneSIS-operated cloud backup for local G.E.N.E data;
- may contain defects, incomplete behavior or untested conditions associated with Alpha-stage software;
- does not guarantee full backward compatibility with future versions.

See [Known Limitations](./docs/KNOWN_LIMITATIONS.md) for the detailed current position.

### Security and Verification

Users should verify the downloaded ZIP before extraction or execution.

See [Release Verification](./docs/RELEASE_VERIFICATION.md) for the official archive values and verification procedure.

A matching SHA-256 confirms consistency with the hash published for the official release archive.

Users should also confirm that the distribution page and verification document were reached through official GeneSIS channels.

Unpatched vulnerabilities and other non-public Security concerns must not be posted in public GitHub Issues.

See [Security Policy](./SECURITY.md).

### No Separate Public Pre-Release Fix List

For this initial Alpha release, no separate public list is provided for fixes made during the non-public development period before general release.

This does not mean that no changes occurred during private development.

It means that this changelog does not publish unverified or incomplete internal development history. Future public releases may include normal `Fixed` entries when confirmed information is available.

## Versioning and Future Entries

Future entries should identify:

- public Version and Build;
- public release date;
- major additions and changes;
- confirmed fixes;
- compatibility changes;
- Security changes that can be publicly disclosed;
- migration requirements;
- new or removed limitations;
- archive-verification values or links.

Fixed Archive values must not be silently replaced in an existing release entry.

A rebuilt or changed package must be recorded as a distinct Build or Release with its own verification record.

## Related Documents

> This provisional English document is installed as `CHANGELOG_EN.md`. The Japanese authoritative changelog will be added as `CHANGELOG.md` during final language alignment.

- [G.E.N.E Repository README](./README.md)
- [Release Information](./docs/RELEASE_INFORMATION.md)
- [Release Verification](./docs/RELEASE_VERIFICATION.md)
- [Known Limitations](./docs/KNOWN_LIMITATIONS.md)
- [Contact and Support](./docs/CONTACT_AND_SUPPORT.md)
- [G.E.N.E / GeneSIS Common Support Policy](./docs/SUPPORT_POLICY.md)
- [G.E.N.E Phase 1 Founder Support Terms](./docs/FOUNDER_TERMS.md)
- [Privacy Notice](./docs/PRIVACY_NOTICE.md)
- [Security Policy](./SECURITY.md)

---

Copyright © 2026 GeneSIS: Concept Engineer's HQ. All rights reserved.
