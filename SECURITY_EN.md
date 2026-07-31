# Security Policy

- **Document Version:** v0.4
- **Status:** Active
- **Published By:** GeneSIS
- **Operating Entity:** GeneSIS-Operator
- **Applicable To:** G.E.N.E Phase 1 / v1.x and this official Repository
- **Established:** 2026-07-31
- **Effective From:** 2026-07-31

> The Japanese version of this document is the original and authoritative version. If any inconsistency or difference in interpretation arises between this translation and the Japanese version, the Japanese version governs to the extent permitted by applicable law.

This document defines the scope, private reporting routes, and basic policy for unresolved security issues.

## 1. Scope

Coverage begins at different times depending on the subject:

| Subject | Coverage Begins |
|---|---|
| The `GeneSIS-Public/G.E.N.E` Repository, published documents, release information, and verification information | From the Effective From date of this Policy |
| The G.E.N.E Alpha v1.0 application and official distribution package | Covered from 2026-07-31 |
| Other GeneSIS deliverables expressly identified as covered by this Policy | From the time individually stated |

The following are generally outside scope:

- Development builds, internal operational versions, or unreleased test versions
- Packages modified or redistributed by third parties
- Unofficial patches or builds
- Issues solely affecting external products such as an operating system, Ollama, an LLM, or a model and unrelated to G.E.N.E
- Social engineering, spam, or denial-of-service activity
- Issues that require unlawful conduct, unauthorized access, or use contrary to the EULA

Issues originating in an external product may still be accepted as reference information when integration with G.E.N.E creates a security impact.

### Supported Versions

| Version | Security Support |
|---|---|
| G.E.N.E Alpha v1.0 | Covered |
| Development builds, internal versions, and unreleased test versions | Not covered |

The G.E.N.E Alpha v1.0 application, official distribution package, Repository, and published documents are covered by this Policy from 2026-07-31.

## 2. Private Reporting

Do not post details of an unresolved security issue in a public GitHub Issue, on X or other social media, or in any other public location.

When GitHub Private Vulnerability Reporting is enabled for this Repository, use that private route.

If it is unavailable, contact the official GeneSIS address:

`genesis.official.poc@mail.com`

Email subject:

```text
[Security Report]
```

When uncertain whether an issue qualifies as a security concern, use a private route rather than posting details publicly.

## 3. Information to Include

Where reasonably possible, include:

- Affected version or build
- Source of the package
- Operating environment, including OS, runtime, and model
- Summary of the issue
- Date and time of confirmation
- Reproduction conditions or steps
- Expected impact
- Required privileges or prerequisites
- Logs or screen information reduced to a safely shareable form
- Any confirmed workaround
- Whether the issue has already been disclosed to a third party
- Preferred contact method

GeneSIS may be unable to investigate or reproduce a report when necessary information is unavailable.

## 4. Information Not to Send

Do not send sensitive information that is unnecessary for investigation, including:

- Passwords, tokens, API keys, private keys, or authentication codes
- Two-factor authentication codes or backup codes
- Credit card numbers or other payment information
- Personal information or third-party non-public information
- Private conversation history, Persona information, or non-public materials
- Third-party data
- Executable exploits or malware not specifically requested in advance

Redact secrets contained in file paths, logs, or screen information.

GeneSIS will not request passwords, authentication codes, backup codes, private keys, or payment information.

## 5. Testing and Disclosure Boundaries

When reviewing a potential security issue, do not:

- Access accounts, devices, files, or data without authorization
- Modify, delete, or destroy data
- Conduct denial-of-service or excessive-load testing
- Use social engineering
- Attack, track, or collect information about third parties
- Violate applicable law, the EULA, or third-party rights

To reduce risk to users, GeneSIS asks reporters to withhold details that could enable exploitation until a correction or official notice is published.

This Policy does not authorize unlawful access, destructive testing, testing against third-party systems, or other unauthorized conduct.

## 6. Response Policy

GeneSIS will review reports and may consider investigation, requests for additional information, workaround guidance, correction, or an official notice.

The following are primary considerations:

- Reproducibility
- Scope of impact
- Severity
- Risk to user data
- Exploitability
- Feasibility of correction
- Current development and operational conditions

Receipt of a report does not guarantee a reply, correction, response deadline, publication of a Security Advisory, or any specific result.

The GeneSIS-Operator determines whether and when disclosure is appropriate, considering impact, exploitability, response status, and applicable law.

This Policy does not create a confidentiality agreement, reward program, or bug bounty program.

## 7. Non-Security Matters

The following are generally not security reports:

- General usage questions
- Feature requests
- Minor display issues
- Ordinary defects that can be disclosed without creating risk to users
- AI or LLM answer content or quality
- Questions about purchases, terms, rights, privacy, or Founder status

For ordinary defects and general inquiries, see [Contact and Support](./docs/CONTACT_AND_SUPPORT.md).

---

Copyright © 2026 GeneSIS: Concept Engineer's HQ. All rights reserved.
