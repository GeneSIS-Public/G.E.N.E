# G.E.N.E Alpha v1.0 — Known Limitations

- **Document Version:** v0.3
- **Status:** Active — Public Release
- **Published By:** GeneSIS
- **Operating Entity:** GeneSIS-Operator
- **Applicable Release:** G.E.N.E Alpha v1.0
- **Target Platform:** Windows x64
- **Build:** `G.E.N.E_Alpha_v1.0_R10-4D-4_Build-005`
- **Established:** 2026-07-31
- **Effective From:** 2026-07-31

> The Japanese version of this document is the original and authoritative version. If any inconsistency or difference in interpretation arises between this translation and the Japanese version, the Japanese version governs to the extent permitted by applicable law.

This document describes limitations currently identified for G.E.N.E Alpha v1.0, environments for which official support is not stated, conditions that have not been sufficiently tested, and important usage precautions.

It does not guarantee that no unlisted issue exists or that every listed limitation will be removed in a future release.

## 1. Categories

This document uses the following categories:

- **Confirmed limitation:** A limitation confirmed from the specification or structure of the current official build
- **Unsupported environment:** An environment for which official support is not stated for this release
- **Untested condition:** A condition for which sufficient testing or compatibility review has not been completed
- **External dependency:** A matter primarily dependent on an operating system, hardware, runtime, model, or another external element
- **Operational precaution:** A precaution required for data protection or safe use

Unsupported or untested does not necessarily mean that the environment is known to be unable to operate.

A statement that an issue may occur does not mean that it occurs in every environment.

## 2. Summary

| Area | Current Position |
|---|---|
| Platform | Windows x64 is the only official target |
| AI Runtime | A separate external local LLM environment is required |
| Model Compatibility | Not every model or runtime version is guaranteed |
| Performance | Depends on hardware, model, runtime, and configuration |
| AI Output | Accuracy, consistency, and safety are not guaranteed |
| Dialogue Continuity | Stored context does not guarantee identity continuity between models |
| Local Data | Users must maintain their own backups |
| Cloud Backup | GeneSIS does not provide cloud backup or synchronization |
| Future Compatibility | Complete backward compatibility for data, settings, or external environments is not guaranteed |
| Public Operational History | Compatibility and defect information remains at an early stage of accumulation |

## 3. Alpha Stage

G.E.N.E Alpha v1.0 is an official release for which the minimum G.E.N.E specification defined for this release has been implemented and tested.

`Alpha` does not mean an unofficial prototype, work-in-progress package, or incomplete implementation.

Operational history after public distribution, compatibility information from user environments, combination testing with external runtimes and models, and maturity of public documentation remain at an early stage.

The following may therefore exist:

- Unidentified defects
- Startup, display, storage, or communication issues limited to particular environments
- Workflows that have not been tested broadly
- Settings, formats, or behavior adjusted in a future release
- Compatibility differences caused by corrections or updates to external environments

For the detailed meaning of Alpha, see [Release Information](./RELEASE_INFORMATION_EN.md).

## 4. Target Platform

The official target platform is:

```text
Windows x64
```

Official support is not stated for:

- 32-bit Windows
- Windows on ARM
- macOS
- Linux
- Mobile operating systems
- Browser-only environments
- Virtualized environments not individually reviewed by GeneSIS
- Compatibility layers not individually reviewed by GeneSIS
- Remote desktop environments not individually reviewed by GeneSIS

Unsupported or untested environments may fail to start or may show different display, storage, communication, or performance behavior.

## 5. External Runtime and Models

G.E.N.E is not an LLM and does not generate text by itself.

AI responses require a separate external local LLM environment, such as Ollama, and an available model.

Unless expressly stated, the official G.E.N.E package does not include an external runtime, models, or the computer resources required to operate them.

Users are responsible for:

- Installing, configuring, and updating the external runtime
- Obtaining, selecting, and storing models
- Complying with licenses and terms for each software package and model
- Confirming suitability for the hardware and intended use
- Securing the external environment and its network configuration

A model available through an external runtime may not operate correctly with every G.E.N.E function.

Possible differences include:

- Unexpected response formats
- Failure to follow instructions or roles
- Reduced Japanese-language capability
- Context-length limitations
- Response delay or timeout
- Incomplete or malformed output
- Behavioral changes after runtime or model updates

GeneSIS does not guarantee compatibility with every runtime, runtime version, model, or model version.

## 6. Hardware and Performance

Performance primarily depends on:

- CPU and GPU capability
- Available RAM and VRAM
- Storage performance and free space
- Model size and quantization
- Context length
- Background processes
- Thermal or power limitations
- External runtime configuration

At present, GeneSIS does not specify a single hardware requirement that guarantees a particular level of performance with every available model.

Depending on the environment, users may experience startup delay, response delay, high memory use, model loading failure, timeout, reduced system performance, or termination by the operating system or external runtime.

No fixed response time, generation speed, or performance level is guaranteed.

## 7. AI Output and Dialogue Continuity

AI output is generated by the external model selected by the user.

Output may be:

- Inaccurate or outdated
- Incomplete, contradictory, or fabricated
- Inappropriate or biased
- Different for the same input
- Unsafe in a particular context

G.E.N.E does not independently verify every generated result. Users should independently confirm important information.

G.E.N.E is an environment for creating continuity of dialogue records and context on the human side.

However, changes to the connected model, model version, system instruction, Persona, context capacity, runtime, or G.E.N.E version may change responses, interpretation, and behavior.

Continuity of stored context does not guarantee identical identity, memory interpretation, emotional expression, or reasoning behavior across different models.

## 8. Local Data, Backup, and Migration

G.E.N.E is designed for local operation.

Do not use it as the only storage location for irreplaceable information.

Users are responsible for backing up important conversation history, Personas, Summaries, Knowledge, References, settings, and related files.

Data may be lost, damaged, or become unavailable because of:

- Accidental deletion or overwrite
- Storage failure
- Abnormal termination of the operating system, application, or runtime
- Interrupted saving
- Security software or another external program
- Direct user modification of files or settings
- Incompatibility with a future version

GeneSIS does not operate a cloud backup or synchronization service for local G.E.N.E data.

Compatibility of data and settings with a future version is not guaranteed unless an official migration procedure or compatibility statement is published.

Create a backup of important data before updating or reinstalling.

## 9. Network and External Components

G.E.N.E is designed for use with a local AI environment.

However, GeneSIS does not guarantee that an external runtime, model-management tool, model-download feature, operating-system service, security product, or another third-party component selected by the user performs no network communication.

Users should review the settings, documentation, terms, privacy policy, and network behavior of each external component.

The GeneSIS-Operator does not control independent data processing or service changes by an external provider.

For the basic handling of G.E.N.E and personal information, see the [Privacy Notice](./PRIVACY_NOTICE_EN.md).

## 10. Archive Verification and Security Warnings

Before extracting or running an archive, verify the official distribution route, file size, and SHA-256.

Use [Release Verification](./RELEASE_VERIFICATION_EN.md) as the authoritative source for fixed values and verification procedures.

A matching SHA-256 confirms that the obtained archive is identical to the fixed official archive. It does not, by itself, guarantee:

- Defect-free software
- Safe and correct operation in every environment
- Independent audit of every internal component
- That the distribution page used to obtain the archive is itself official

Windows, a browser, or security software may display a warning based on download reputation, source, application reputation, or code-signing status.

The `Release Record Signed Date` is a date associated with the GeneSIS release record. It does not by itself indicate an operating-system code signature such as Microsoft Authenticode.

Do not ignore a warning solely because the filename appears correct. Confirm the official route and archive SHA-256.

When an unresolved security issue is suspected, do not disclose details in a public Issue or on social media. Use the private route in the [Security Policy](../SECURITY_EN.md).

## 11. Updates and Future Compatibility

A later G.E.N.E v1.x release may change:

- UI and operating procedures
- Configuration items
- Supported runtimes and models
- Dialogue processing
- Internal file and data formats
- Installation and directory structure
- Supported and unsupported environments
- Documentation

Indefinite backward compatibility with every Alpha-stage file, setting, data format, or external runtime is not guaranteed.

Before updating or replacing an existing environment, review the Release Information, Known Limitations, Changelog, and any published migration procedure for the target release.

Later releases will be distributed as separately versioned files. The fixed official G.E.N.E Alpha v1.0 archive itself will not be modified.

## 12. High-Risk Use and Reporting

G.E.N.E Alpha v1.0 is not certified for:

- Medical diagnosis or treatment decisions
- Definitive legal decisions or legal representation
- Financial transactions or investment decisions
- Emergency response
- Control of vehicles, machinery, or critical infrastructure
- Access control, identity verification, or authentication decisions
- Decisions where an incorrect answer could directly cause serious harm

Use associated with such activities requires human review, independent verification, and safety measures appropriate to the use case.

Report publicly shareable limitations, documentation issues, or reproducible ordinary defects through the GitHub routes described in [Contact and Support](./CONTACT_AND_SUPPORT_EN.md).

Do not post personal information, credentials, private conversations, Founder verification information, or details of unresolved vulnerabilities in a public Issue.

---

Copyright © 2026 GeneSIS: Concept Engineer's HQ. All rights reserved.
