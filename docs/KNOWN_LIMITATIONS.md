# G.E.N.E Alpha v1.0 — Known Limitations

- **Document Version:** v0.2 Final Draft
- **Language:** English
- **Document Role:** Provisional English Draft
- **Status:** Draft — Pending Public Release
- **Planned Authoritative Version:** Japanese version to be published during final document alignment
- **Published By:** GeneSIS
- **Project:** Project: Code-NOAH
- **Product:** G.E.N.E Alpha v1.0
- **Target Platform:** Windows x64
- **Build:** `G.E.N.E_Alpha_v1.0_R10-4D-4_Build-005`
- **Established:** ［正式公開時に記入］
- **Effective From:** ［公開開始時に記入］

> **This document is a public-release preparation draft.**  
> It does not, by itself, indicate that public distribution has started.  
> The Japanese version is planned to become the original and authoritative version during final document alignment. After that version is published, the Japanese version will govern any inconsistency or difference in interpretation to the extent permitted by applicable law.

## 日本語案内

本書は、G.E.N.E Alpha v1.0について、現在確認されている制約、未保証事項および利用上の注意をまとめた資料です。

G.E.N.E Alpha v1.0はWindows x64向けのAlpha段階の製品であり、外部ローカルLLM環境、利用するModel、Hardwareおよび設定によって挙動が変わります。

本書に記載されていない不具合や制限が存在しないことを保証するものではありません。

## 1. Purpose and Scope

This document describes known limitations, unsupported conditions and important operational cautions for G.E.N.E Alpha v1.0.

It is intended to help users decide whether the Alpha release is appropriate for their environment and intended use.

This document is not:

- a complete list of every possible defect;
- a guarantee that an unlisted problem does not exist;
- a substitute for the EULA or applicable official conditions;
- a promise that every limitation will be removed;
- a compatibility certification for every computer, model or local LLM environment.

Limitations may be added, revised or removed as GeneSIS confirms new information.

## Limitation Summary

| Area | Current Position |
|---|---|
| Platform | Windows x64 only |
| AI Runtime | External local LLM environment required |
| Model Compatibility | Not guaranteed for every model or runtime version |
| Performance | Depends on hardware, model and runtime |
| Dialogue Continuity | Stored context does not guarantee model identity equivalence |
| Data Backup | User-managed; no GeneSIS cloud backup |
| Future Compatibility | Full backward compatibility is not guaranteed |
| Source Code | Not publicly released |
| Support | Response or correction is not guaranteed |

## 2. Limitation Classification

This document uses the following classifications:

- **Confirmed Limitation:** A limitation confirmed in the current official build.
- **Unsupported Environment:** An environment for which GeneSIS does not currently provide official support.
- **Untested Condition:** A condition that has not received sufficient testing.
- **External Dependency:** Behavior primarily determined by an external runtime, model, operating system or hardware.
- **Operational Caution:** A precaution users should observe when operating Alpha-stage software.

An unsupported or untested environment is not necessarily known to be incompatible.

A limitation described as possible does not mean that it occurs in every environment.

## 3. Alpha-Stage Software

G.E.N.E Alpha v1.0 is an Alpha-stage release.

Users should expect that:

- defects or incomplete behavior may remain;
- unexpected termination, display problems or configuration-specific failures may occur;
- some workflows may not yet have broad testing;
- documentation may continue to be refined;
- future releases may change functions, settings, formats or behavior;
- fixes may introduce new compatibility differences.

Alpha status does not mean that the official release archive may be modified after its verification values have been established.

The official ZIP remains identified by the values in [Release Verification](./RELEASE_VERIFICATION.md).

## 4. Target Platform and Unsupported Environments

G.E.N.E Alpha v1.0 is released for:

```text
Windows x64
```

The following environments are not currently represented as officially supported by this release:

- 32-bit Windows;
- Windows on ARM;
- macOS;
- Linux;
- mobile operating systems;
- browser-only environments;
- virtualized, compatibility-layer or remote-desktop environments not specifically tested by GeneSIS.

The application may fail to start or behave differently in unsupported or untested environments.

## 5. External Local LLM Requirement

G.E.N.E is not an LLM and does not perform language generation by itself.

A separately installed and configured external local LLM environment is required for AI-generated responses.

This may include an environment such as Ollama, but G.E.N.E is not an official Ollama product and does not guarantee compatibility with every Ollama version, API behavior or model.

The external environment, models and their required resources are not included unless the official package explicitly states otherwise.

Users are responsible for:

- installing and maintaining the external local LLM environment;
- obtaining compatible models;
- complying with each model's license and conditions;
- confirming that the model is suitable for the intended language and use;
- managing the external environment's configuration and security.

## 6. Model Compatibility

Compatibility may differ between models and model versions.

A model being available through a local LLM environment does not guarantee that it will work correctly with every G.E.N.E function.

Possible differences include:

- unsupported or unexpected response formats;
- failure to follow system or dialogue instructions;
- reduced Japanese-language performance;
- context-length limitations;
- excessive response latency;
- incomplete or malformed output;
- differences in role, instruction or message handling;
- changed behavior after a model or runtime update.

GeneSIS does not guarantee identical output, personality, behavior or continuity across different models.

The purpose of G.E.N.E is to provide continuity on the human-controlled environment side; it cannot make different models internally identical.

## 7. Hardware and Performance

Performance depends on the user's computer, external local LLM environment and selected model.

Relevant factors include:

- CPU and GPU capability;
- available RAM and VRAM;
- storage speed and free space;
- model size and quantization;
- context length;
- background processes;
- thermal or power limitations;
- external runtime settings.

GeneSIS does not currently publish a single hardware specification that guarantees acceptable performance for every supported model.

Users may experience:

- slow startup;
- delayed responses;
- high memory use;
- model loading failure;
- system slowdown;
- timeouts;
- termination by the operating system or external runtime.

No fixed response time or performance level is guaranteed.

## 8. Model Output Reliability

AI-generated output is produced by the external model selected by the user.

Output may be:

- inaccurate;
- incomplete;
- internally inconsistent;
- outdated;
- fabricated;
- inappropriate;
- biased;
- unsafe for a particular context;
- different when the same request is repeated.

G.E.N.E does not independently verify every generated statement.

Users must independently verify important information before relying on it.

G.E.N.E and connected models should not be treated as the sole authority for medical, legal, financial, safety-critical or other high-impact decisions.

## 9. Dialogue Continuity

G.E.N.E is designed to help users maintain dialogue continuity on the user-controlled side.

However, continuity is subject to limitations.

Changes in the following may alter the resulting dialogue:

- connected model;
- model version;
- system instructions;
- Persona or dialogue configuration;
- context-window capacity;
- external runtime behavior;
- G.E.N.E version;
- user-edited records or settings.

G.E.N.E does not guarantee that a replacement model will reproduce the same identity, memory interpretation, emotional tone or reasoning behavior as a previous model.

Continuity of stored context does not mean identity equivalence between models.

## 10. Local Data and Backup Responsibility

G.E.N.E is intended for local operation, but Alpha-stage software should not be used as the sole storage location for irreplaceable information.

Users are responsible for maintaining appropriate backups of important G.E.N.E-related files, settings and records available in their environment.

Possible risks include:

- accidental deletion;
- storage-device failure;
- operating-system failure;
- interruption during writing or saving;
- corruption caused by an application, runtime or system failure;
- incompatibility after future updates;
- user modification of files or settings.

Unless an official migration procedure is published, compatibility of local data or settings with future G.E.N.E versions is not guaranteed.

GeneSIS does not operate a cloud backup or synchronization service for the user's local G.E.N.E data.

## 11. Network and External Component Behavior

G.E.N.E is intended for use with a local AI environment.

This does not guarantee that every external component selected by the user operates without network communication.

The following may have independent network behavior:

- external local LLM runtimes;
- model-management tools;
- model download systems;
- operating-system services;
- security software;
- third-party libraries or tools installed by the user.

Users should review the configuration, documentation, Privacy Policy and network behavior of external components.

GeneSIS does not control the independent data practices of external providers.

## 12. Security and Release Verification

The SHA-256 values published by GeneSIS allow users to check whether a downloaded ZIP matches the hash published for the official release archive.

A matching SHA-256 does not mean that:

- the Alpha release is defect-free;
- every internal component has been independently audited;
- the software is compatible with every environment;
- the file is safe for every possible use;
- a distribution page is official when reached through an untrusted route.

Users should confirm that both the distribution page and the verification document were reached through official GeneSIS channels.

The G.E.N.E source code is not publicly released.

Public Release metadata and hash verification do not constitute a public source-code audit.

See [Release Verification](./RELEASE_VERIFICATION.md) and [Security Policy](../SECURITY.md).

## 13. Windows and Security-Software Warnings

Windows, web browsers or security software may display warnings based on download reputation, archive origin, application reputation or code-signing status.

The `Release Record Signed Date` published in GeneSIS documentation refers to the GeneSIS release-evidence record.

It does not, by itself, indicate Microsoft Authenticode or another operating-system code-signing status.

Users should not bypass a warning solely because a file name appears correct.

Verify the archive SHA-256 and confirm the official distribution route before extracting or running the file.

## 14. Updates and Compatibility Changes

Future versions may change:

- user-interface behavior;
- settings;
- supported models or runtimes;
- dialogue handling;
- internal files or data formats;
- installation structure;
- documentation;
- supported and unsupported environments.

GeneSIS does not guarantee indefinite backward compatibility with every Alpha-stage file, setting or external runtime.

Users should review Release Information, Known Limitations and migration instructions before replacing an existing installation.

Do not overwrite important local data without a backup.

## 15. No Guaranteed Support Response or Fix

G.E.N.E is individually developed and operated by GeneSIS.

Support is provided within the scope, priority and capacity described in [G.E.N.E / GeneSIS Common Support Policy](./SUPPORT_POLICY.md).

GeneSIS does not guarantee:

- an immediate response;
- a response within a fixed period;
- an individual response to every report;
- reproduction of every reported issue;
- correction of every defect;
- continued support for every model or external runtime;
- support for unsupported environments.

A report may be closed, deferred or documented as a known limitation without an immediate software change.

## 16. Public Reports and Private Information

GitHub Issues are public.

Only information that can safely be published should be submitted there.

Do not post:

- personal information;
- purchase or Founder qualification information;
- private dialogue history;
- Persona information;
- Passwords, authentication codes, API Keys or private keys;
- unredacted Logs or screenshots containing private information;
- details of an unpatched vulnerability.

Use the designated private route for Security concerns and the GeneSIS official Gmail route for matters requiring personal identification or private handling.

See [Contact and Support](./CONTACT_AND_SUPPORT.md).

## 17. Unsupported and High-Risk Uses

G.E.N.E Alpha v1.0 is not certified for:

- medical diagnosis or treatment decisions;
- legal representation or definitive legal advice;
- financial trading or investment decisions;
- emergency response;
- operation of vehicles, machinery or critical infrastructure;
- access control, identity verification or authentication decisions;
- decisions where an incorrect response could directly cause serious harm.

Users who choose to use G.E.N.E in connection with high-risk activities remain responsible for independent verification, human review and appropriate safeguards.

## 18. Reporting a Limitation

For a publicly shareable technical limitation, documentation issue or reproducible defect, use the designated GitHub route described in [Contact and Support](./CONTACT_AND_SUPPORT.md).

For a non-public Security concern, use the private route described in [Security Policy](../SECURITY.md).

For purchase, Founder qualification, rights, Privacy or other individually handled matters, use the GeneSIS official Gmail route.

When reporting a technical limitation, provide only the information necessary to understand and reproduce the issue.

## 19. Related Documents

- [G.E.N.E Repository README](../README.md)
- [Release Information](./RELEASE_INFORMATION.md)
- [Release Verification](./RELEASE_VERIFICATION.md)
- [Contact and Support](./CONTACT_AND_SUPPORT.md)
- [G.E.N.E / GeneSIS Common Support Policy](./SUPPORT_POLICY.md)
- [G.E.N.E Phase 1 Founder Support Terms](./FOUNDER_TERMS.md)
- [Privacy Notice](./PRIVACY_NOTICE.md)
- [Security Policy](../SECURITY.md)

---

Copyright © 2026 GeneSIS: Concept Engineer's HQ. All rights reserved.
