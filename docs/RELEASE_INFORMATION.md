# G.E.N.E Alpha v1.0 — Release Information

- **Document Version:** v0.2 Final Draft
- **Status:** Draft — Pending Public Release
- **Published By:** GeneSIS
- **Project:** Project: Code-NOAH
- **Product:** G.E.N.E Alpha v1.0
- **Target Platform:** Windows x64
- **Build:** `G.E.N.E_Alpha_v1.0_R10-4D-4_Build-005`
- **Official Distribution URL:** ［BOOTH正式商品URL］
- **Established:** ［正式公開時に記入］
- **Effective From:** ［公開開始時に記入］

> **This document is a public-release preparation draft.**  
> It does not, by itself, indicate that public distribution has started.

## 日本語案内

G.E.N.E Alpha v1.0は、GeneSISが個人開発したWindows x64向けのローカルAI対話環境です。

G.E.N.E自体はLLMではありません。Ollama等の外部ローカルLLM環境および利用するLLMモデルは、利用者自身が別途用意・管理します。

主な位置づけは次のとおりです。

- G.E.N.E Alpha v1.0は無料で配布されます。
- Founder参加や任意支援の有無によって、G.E.N.E本体の機能は変わりません。
- 正式配布物は、すべての利用者に対して同一の公式Release Packageです。
- 本製品はAlpha段階であり、未確認の不具合や互換性上の制限が残る可能性があります。
- G.E.N.EのSource Codeは公開されません。
- 正式なZIP配布元はGeneSIS公式BOOTHです。
- GitHub Repositoryは、Release情報、検証値、既知の制限、Support・Security・Privacy方針および公式技術文書を公開する情報拠点です。
- ダウンロードしたZIPは、利用前に[Release Verification](./RELEASE_VERIFICATION.md)のSHA-256と照合してください。

G.E.N.Eは、特定のAI提供者や単一のModelだけに対話の継続性を依存させず、利用者側で対話環境と記録を管理することを目的としています。

> AIが変わっても、あなたの対話と思考まで失う必要はない。  
> 人間側に、AIとの継続性を作る。

## 1. Release Overview

| Item | Information |
|---|---|
| Product | `G.E.N.E Alpha v1.0` |
| Developer / Brand | `GeneSIS` |
| Project | `Project: Code-NOAH` |
| Platform | `Windows x64` |
| Build | `G.E.N.E_Alpha_v1.0_R10-4D-4_Build-005` |
| Distribution Format | ZIP archive |
| Distribution Channel | Official GeneSIS BOOTH |
| Price | Free |
| Feature Restrictions | None based on payment or support status |
| Source Code | Not publicly released |

The official archive is:

```text
G.E.N.E_Alpha_v1.0_Windows_x64.zip
```

For the official file size, SHA-256 and verification procedure, see [Release Verification](./RELEASE_VERIFICATION.md).

## 2. What G.E.N.E Is

G.E.N.E is a local AI dialogue environment developed by GeneSIS.

It is intended to provide a human-controlled environment in which dialogue settings, interaction context and the continuity of AI-assisted thought can be managed independently from any single external AI provider or model.

The central concept is:

> AIが変わっても、あなたの対話と思考まで失う必要はない。  
> 人間側に、AIとの継続性を作る。

G.E.N.E is designed around the idea that the continuity of dialogue should remain under the user's control, even when the connected AI model or local AI environment changes.

## 3. What G.E.N.E Is Not

G.E.N.E is not:

- a Large Language Model;
- a cloud AI provider;
- an online AI account service;
- a model-training service;
- a replacement for the external local LLM environment required for inference;
- an official product of Ollama or any connected model provider;
- an open-source distribution of the G.E.N.E source code.

G.E.N.E provides the dialogue environment and related local application functions.

Language generation is performed by the local model environment selected and operated by the user.

## 4. External Local LLM Environment

G.E.N.E is designed to connect to an external local LLM environment, including environments such as Ollama.

The external local LLM environment, installed models and computer resources are not included in the G.E.N.E application archive unless explicitly stated otherwise.

The user is responsible for:

- installing and configuring the required external local LLM environment;
- obtaining models under the terms established by their respective providers;
- confirming that the selected model is compatible with the user's hardware and intended use;
- complying with the license and usage conditions of each external model or Service;
- securing the local computer and connected local AI environment.

Performance, output quality, language ability and behavior may differ depending on the connected environment and model.

G.E.N.E does not guarantee identical behavior across all models, model versions or hardware configurations.

## 5. Local Operation and Data Control

G.E.N.E is intended for local operation.

The connected local LLM environment and the user's computer process the dialogue according to the configuration selected by the user.

GeneSIS does not operate a G.E.N.E cloud conversation service and does not automatically receive the user's local dialogue content merely because G.E.N.E is used.

However, external software, models or Services connected by the user may have their own data-handling behavior.

Users should review the configuration, license, Privacy Policy and network behavior of every external component they choose to use.

Do not submit private dialogue history, Persona information or other sensitive local data to GitHub Issues or other public channels.

## 6. Alpha Release Position

G.E.N.E Alpha v1.0 is an Alpha-stage release.

The Alpha designation means that:

- the product is an early public-stage build;
- behavior may vary depending on the local model environment;
- some functions or environments may not yet have broad compatibility testing;
- defects, limitations or incomplete behavior may remain;
- documentation and operating procedures may continue to be refined;
- future releases may change functions, formats, compatibility or internal behavior.

Alpha does not mean that the archive may be modified after its official verification values have been established.

The official release archive is fixed by its published file size and SHA-256 record.

Known limitations and unsupported conditions will be documented separately in [Known Limitations](./KNOWN_LIMITATIONS.md) when that document is published.

## 7. Price and Access

G.E.N.E Alpha v1.0 is distributed free of charge.

The G.E.N.E application itself does not impose feature restrictions based on whether the user has made a payment, participated in Founder Support or provided any other financial support.

All users receive the same official G.E.N.E application package for the corresponding release.

No payment is required to unlock hidden G.E.N.E functions in Alpha v1.0.

## 8. Founder Support

G.E.N.E Phase 1 Founder Support is an optional framework through which participants explicitly support and participate in Project: Code-NOAH and GeneSIS activities during Phase 1.

Founder Support:

- is not required to obtain or use the corresponding G.E.N.E application;
- does not unlock exclusive functions in the G.E.N.E application package;
- does not grant status as an owner, shareholder, investor, lender or participant in GeneSIS business profits;
- does not guarantee specific completion dates or delivery dates;
- is verified through the applicable official BOOTH purchase record and the GeneSIS official contact route where confirmation is necessary.

The scope and conditions of Founder deliverables are governed exclusively by the applicable Founder Terms.

Future Founder-related deliverables are separate from the free G.E.N.E application package.

See [G.E.N.E Phase 1 Founder Support Terms](./FOUNDER_TERMS.md).

## 9. Distribution and Official Information Sources

### 9.1 Official GeneSIS BOOTH

The official GeneSIS BOOTH channel is the authoritative distribution location for the G.E.N.E release archive.

Official distribution page:

```text
［BOOTH正式商品URL］
```

Where Founder Support applies, the BOOTH purchase record is the authoritative record for Founder qualification.

### 9.2 GitHub Repository

This GitHub Repository is the official technical-information location for:

- Release information;
- verification values;
- Build identification;
- Known Limitations;
- documentation;
- Support, Security and Privacy policies;
- public technical notices;
- public routes for technical issues, documentation feedback and development feedback.

GitHub is not:

- the official purchase record;
- the Founder qualification authority;
- a payment processor;
- a customer-management store;
- the public source-code distribution location.

### 9.3 GeneSIS Official Gmail

The GeneSIS official Gmail address is the formal non-public contact route for matters requiring individual identification or private handling.

This includes:

- purchase and Founder qualification questions;
- rights and distribution-condition questions;
- Privacy requests;
- non-public technical matters;
- Security reports when the GitHub private reporting route cannot be used.

See [Contact and Support](./CONTACT_AND_SUPPORT.md).

## 10. Source Code Policy

The G.E.N.E source code is not publicly released.

The public availability of the application archive, documentation, Release metadata or verification values does not grant access to or a right to obtain the source code.

Users may use the distributed application only under the applicable EULA and official conditions included with or published for the release.

The absence of public source code does not prevent users from checking whether a downloaded ZIP matches the SHA-256 value published for the official release archive.

Users should also confirm that both the distribution page and the verification document were reached through official GeneSIS channels.

## 11. Release Verification

The official G.E.N.E Alpha v1.0 archive is identified by the verification record published in [Release Verification](./RELEASE_VERIFICATION.md).

Key values include:

| Item | Official Value |
|---|---|
| File Name | `G.E.N.E_Alpha_v1.0_Windows_x64.zip` |
| File Size | `79,504,332 bytes` |
| SHA-256 | `420db62dbb6763aebe01a5e0ab0225ebdafdb9bc6ec471e45098d2e812d3ffea` |
| Build | `G.E.N.E_Alpha_v1.0_R10-4D-4_Build-005` |
| Release Identity SHA-256 | `1ac70e76edc2225e69f80d33b4bb60c2d01bb8fd135b14e4cdb8bae7367cbcc9` |
| Release Record Signed Date | `2026-07-21` |
| Release Archive Verification Status | `PASS` |

`PASS` means that the canonical release archive record and the recorded archive-copy verification completed successfully.

It does not mean that the Alpha release is defect-free, compatible with every environment or suitable for every purpose.

The Release Record Signed Date refers to the GeneSIS release-evidence record associated with this archive.

It does not, by itself, indicate that the Windows executable has been signed through Microsoft Authenticode or another operating-system code-signing system.

The archive SHA-256 is the primary value users can calculate directly from the downloaded ZIP.

Release Identity SHA-256 identifies the official GeneSIS release record and is distinct from the SHA-256 calculated directly from the ZIP archive.

## 12. Installation and Use

Detailed installation and first-use instructions should be followed from the documentation included with the official G.E.N.E package or separately published through official GeneSIS channels.

Before extracting or running the archive:

1. obtain the ZIP from the official GeneSIS BOOTH;
2. confirm that this Repository was reached through an official GeneSIS route;
3. calculate the ZIP SHA-256;
4. compare it with [Release Verification](./RELEASE_VERIFICATION.md);
5. do not extract or run the archive if the SHA-256 does not match;
6. review the EULA and other conditions included with the official package;
7. review Known Limitations before relying on the Alpha release for important work.

Do not modify the official ZIP and continue to represent the modified file as the official GeneSIS archive.

## 13. Compatibility and Limitations

Compatibility depends on factors including:

- Windows environment;
- external local LLM environment;
- selected model and model version;
- hardware capacity;
- available memory and storage;
- local configuration;
- third-party software behavior;
- changes made by external model or Service providers.

This document does not claim compatibility with every Windows x64 system, model or configuration.

Specific known limitations, unsupported cases and operational cautions will be maintained in [Known Limitations](./KNOWN_LIMITATIONS.md).

## 14. Support and Security

G.E.N.E is individually developed and operated by GeneSIS.

Support is provided within the scope, priority and capacity described in [G.E.N.E / GeneSIS Common Support Policy](./SUPPORT_POLICY.md).

Publicly shareable technical problems and Documentation Feedback may be submitted through the designated GitHub route.

Private information, purchase matters, Founder qualification, rights questions and other individually handled matters must use the GeneSIS official contact route.

Unpatched vulnerabilities and other non-public Security concerns must not be posted in a public GitHub Issue.

See:

- [Contact and Support](./CONTACT_AND_SUPPORT.md)
- [Security Policy](../SECURITY.md)
- [Privacy Notice](./PRIVACY_NOTICE.md)

## 15. No Warranty Expansion by This Document

This Release Information document explains the identity, role and public-release position of G.E.N.E Alpha v1.0.

It does not create warranties, support obligations, compatibility guarantees, delivery guarantees or rights beyond those provided in the applicable EULA and official conditions.

If this document conflicts with the EULA included in the official G.E.N.E package regarding use of the application, the EULA governs the use of the application to the extent of that conflict.

Founder participation is separately governed by [G.E.N.E Phase 1 Founder Support Terms](./FOUNDER_TERMS.md).

## 16. Related Documents

- [G.E.N.E Repository README](../README.md)
- [Release Verification](./RELEASE_VERIFICATION.md)
- [Known Limitations](./KNOWN_LIMITATIONS.md)
- [Contact and Support](./CONTACT_AND_SUPPORT.md)
- [G.E.N.E / GeneSIS Common Support Policy](./SUPPORT_POLICY.md)
- [G.E.N.E Phase 1 Founder Support Terms](./FOUNDER_TERMS.md)
- [Privacy Notice](./PRIVACY_NOTICE.md)
- [Security Policy](../SECURITY.md)

---

Copyright © 2026 GeneSIS: Concept Engineer's HQ. All rights reserved.
