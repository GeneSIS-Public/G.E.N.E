# G.E.N.E Alpha v1.0 — Release Verification

- **Document Version:** v0.2 Final Draft
- **Status:** Draft — Pending Public Release
- **Established:** ［正式公開時に記入］
- **Effective From:** ［公開開始時に記入］
- **Published By:** GeneSIS
- **Project:** Project: Code-NOAH
- **Product:** G.E.N.E Alpha v1.0
- **Target Platform:** Windows x64

> This document records the official verification values for the G.E.N.E Alpha v1.0 Windows x64 release archive.  
> The existence of this document does not, by itself, indicate that public distribution has started.

## 日本語案内

この文書は、G.E.N.E Alpha v1.0の正式配布ZIPが、GeneSISの公開した正式Release記録と一致するか確認するための資料です。

Windowsでは、PowerShellで次のCommandを実行し、表示されたSHA-256を本書の正式値と比較してください。

```powershell
Get-FileHash ".\G.E.N.E_Alpha_v1.0_Windows_x64.zip" -Algorithm SHA256
```

SHA-256が一致しない場合は、ZIPを展開または実行せず、公式GeneSIS BOOTHから再取得してください。

正式な検証値および詳細な手順は、以下の本文に記載しています。

## Verification Scope

This document describes archive-level verification using the file size and SHA-256 hash of the complete ZIP archive.

It does not provide a complete procedure for independently verifying the signed Release Manifest or the full internal release-evidence chain.

A separate signature-verification procedure may be published when GeneSIS provides that process for public use.

## 1. Official Release Archive

The official release archive is identified by all of the following values.

| Item | Official Value |
|---|---|
| File Name | `G.E.N.E_Alpha_v1.0_Windows_x64.zip` |
| File Size | `79,504,332 bytes` |
| SHA-256 | `420db62dbb6763aebe01a5e0ab0225ebdafdb9bc6ec471e45098d2e812d3ffea` |
| Build | `G.E.N.E_Alpha_v1.0_R10-4D-4_Build-005` |
| Release Identity SHA-256 | `1ac70e76edc2225e69f80d33b4bb60c2d01bb8fd135b14e4cdb8bae7367cbcc9` |
| Release Record Signed Date | `2026-07-21` |
| Release Verification Status | `PASS` |

The official ZIP archive must not be modified after these values have been established.

Changing, recompressing, renaming the internal files, adding files, removing files or editing any content inside the archive will normally change the archive SHA-256 value.

## 2. What the Values Mean

### 2.1 File Name

The expected archive name is:

```text
G.E.N.E_Alpha_v1.0_Windows_x64.zip
```

A different file name does not by itself prove that the contents are different, because users can rename a downloaded file.

For verification, the SHA-256 value is more important than the local file name.

### 2.2 File Size

The expected archive size is:

```text
79,504,332 bytes
```

A different size indicates that the file is not byte-for-byte identical to the official archive.

Matching size alone is not sufficient. Always verify the SHA-256 value.

### 2.3 Archive SHA-256

The archive SHA-256 is calculated directly from the complete ZIP file.

Expected value:

```text
420db62dbb6763aebe01a5e0ab0225ebdafdb9bc6ec471e45098d2e812d3ffea
```

If the calculated value matches exactly, the local ZIP file matches the SHA-256 value published for the official archive represented by this record.

### 2.4 Build Identifier

The official Build identifier is:

```text
G.E.N.E_Alpha_v1.0_R10-4D-4_Build-005
```

The Build identifier identifies the intended G.E.N.E build represented by this release.

The Build identifier is not a substitute for file-hash verification.

### 2.5 Release Identity SHA-256

The official Release Identity value is:

```text
1ac70e76edc2225e69f80d33b4bb60c2d01bb8fd135b14e4cdb8bae7367cbcc9
```

This value identifies the official GeneSIS release record associated with this build.

It is distinct from the SHA-256 value calculated directly from the ZIP archive.

Unless GeneSIS publishes a separate Release Identity generation and verification procedure, users should treat this value as an official release-record identifier and should use the archive SHA-256 value for direct local-file verification.

## 3. Verify on Windows PowerShell

Open PowerShell in the folder containing the downloaded ZIP file and run:

```powershell
Get-FileHash ".\G.E.N.E_Alpha_v1.0_Windows_x64.zip" -Algorithm SHA256
```

Expected hash:

```text
420db62dbb6763aebe01a5e0ab0225ebdafdb9bc6ec471e45098d2e812d3ffea
```

PowerShell may display hexadecimal letters in uppercase. Uppercase and lowercase letters represent the same hexadecimal value.

Example comparison:

```text
Expected:
420db62dbb6763aebe01a5e0ab0225ebdafdb9bc6ec471e45098d2e812d3ffea

Calculated:
420DB62DBB6763AEBE01A5E0AB0225EBDAFDB9BC6EC471E45098D2E812D3FFEA
```

These two values match.

## 4. Verify with Windows `certutil`

Windows users may also run:

```cmd
certutil -hashfile "G.E.N.E_Alpha_v1.0_Windows_x64.zip" SHA256
```

Compare the result with:

```text
420db62dbb6763aebe01a5e0ab0225ebdafdb9bc6ec471e45098d2e812d3ffea
```

Ignore spaces inserted by the command when comparing the hexadecimal value.

## 5. Verify on Linux

Run:

```bash
sha256sum "G.E.N.E_Alpha_v1.0_Windows_x64.zip"
```

Expected output begins with:

```text
420db62dbb6763aebe01a5e0ab0225ebdafdb9bc6ec471e45098d2e812d3ffea
```

## 6. Verify on macOS

Run:

```bash
shasum -a 256 "G.E.N.E_Alpha_v1.0_Windows_x64.zip"
```

Expected output begins with:

```text
420db62dbb6763aebe01a5e0ab0225ebdafdb9bc6ec471e45098d2e812d3ffea
```

## 7. Result Interpretation

### Match

The file is consistent with the official release archive when:

```text
File size:
79,504,332 bytes

SHA-256:
420db62dbb6763aebe01a5e0ab0225ebdafdb9bc6ec471e45098d2e812d3ffea
```

The SHA-256 comparison is the primary verification step.

A matching SHA-256 confirms consistency with the hash published in this record.

Users should also confirm that both the distribution page and this verification document were reached through official GeneSIS channels.

### Mismatch

Do not run or extract the archive if the calculated SHA-256 does not match.

A mismatch may indicate:

- an incomplete or corrupted download;
- a modified or recompressed archive;
- a different G.E.N.E build;
- a file obtained from an unofficial source;
- accidental local modification;
- malicious tampering.

Delete the mismatched file and obtain a new copy from the official distribution channel.

Do not attempt to repair the archive manually and then treat it as an official file.

## 8. Official Distribution and Information Sources

The official G.E.N.E archive is distributed through the official GeneSIS BOOTH channel.

This GitHub Repository is the official source for:

- Release information;
- verification values;
- Build identification;
- Known Limitations;
- Support and Security policies;
- official technical documentation.

GitHub is not the purchase record or Founder qualification authority.

BOOTH purchase records are the authoritative source for Founder qualification where applicable.

## 9. Reporting a Verification Problem

For a simple documentation error that contains no private information, use the public GitHub Issue route described in [Contact and Support](./CONTACT_AND_SUPPORT.md).

For a suspected malicious archive, compromised distribution route or other non-public Security concern, follow the private reporting route in [Security Policy](../SECURITY.md).

For purchase, Founder qualification or other private matters, contact the GeneSIS official Gmail address described in [Contact and Support](./CONTACT_AND_SUPPORT.md).

Do not post the following information in a public GitHub Issue:

- purchase or Founder identification information;
- private email correspondence;
- Passwords, authentication codes, API Keys or private keys;
- private dialogue history or Persona information;
- unredacted local paths or Logs containing personal information;
- details of an unpatched Security issue.

## 10. Verification Checklist

Before using the archive, confirm all applicable items.

```text
[ ] The file was obtained from the official GeneSIS distribution channel.
[ ] The expected archive name is G.E.N.E_Alpha_v1.0_Windows_x64.zip.
[ ] The file size is 79,504,332 bytes.
[ ] The calculated SHA-256 exactly matches the official SHA-256.
[ ] The release is identified as G.E.N.E_Alpha_v1.0_R10-4D-4_Build-005.
[ ] Any mismatch or Security concern has been reported through the correct route.
```

## 11. Related Documents

- [G.E.N.E Repository README](../README.md)
- [Contact and Support](./CONTACT_AND_SUPPORT.md)
- [G.E.N.E / GeneSIS Common Support Policy](./SUPPORT_POLICY.md)
- [Security Policy](../SECURITY.md)
- [Privacy Notice](./PRIVACY_NOTICE.md)

---

Copyright © 2026 GeneSIS: Concept Engineer's HQ. All rights reserved.
