# G.E.N.E Alpha v1.0 — Release Verification

- **Document Version:** v0.4
- **Status:** Active — Public Release
- **Published By:** GeneSIS
- **Operating Entity:** GeneSIS-Operator
- **Applicable Release:** G.E.N.E Alpha v1.0
- **Public Release Date:** `2026-07-31`
- **Target Platform:** Windows x64
- **Established:** 2026-07-31
- **Effective From:** 2026-07-31

> The Japanese version of this document is the original and authoritative version. If any inconsistency or difference in interpretation arises between this translation and the Japanese version, the Japanese version governs to the extent permitted by applicable law.

This document provides the values and procedures used to identify the official G.E.N.E Alpha v1.0 application archive and verify that an obtained file matches the fixed official archive.

## 1. Official Archive

| Item | Fixed Value |
|---|---|
| Product | `G.E.N.E Alpha v1.0` |
| File Name | `G.E.N.E_Alpha_v1.0_Windows_x64.zip` |
| File Size | `79,504,332 bytes` |
| Build | `G.E.N.E_Alpha_v1.0_R10-4D-4_Build-005` |
| SHA-256 | `420db62dbb6763aebe01a5e0ab0225ebdafdb9bc6ec471e45098d2e812d3ffea` |
| Release Identity SHA-256 | `1ac70e76edc2225e69f80d33b4bb60c2d01bb8fd135b14e4cdb8bae7367cbcc9` |
| Release Record Signed Date | `2026-07-21` |
| Internal Archive Verification | `PASS` |

These values identify the fixed official G.E.N.E Alpha v1.0 archive.

The official archive itself will not be modified, recompressed, or silently replaced under the same filename.

## 2. Meaning of Each Value

### File Name

This is the filename of the official archive.

A filename alone does not prove identical content. Verify the file size and SHA-256 as well.

### File Size

This is the total number of bytes in the archive.

An identical file size does not necessarily mean identical content, so SHA-256 verification is required.

### SHA-256

This is the SHA-256 of the official application archive itself.

Confirm that the SHA-256 of the obtained file exactly matches:

```text
420db62dbb6763aebe01a5e0ab0225ebdafdb9bc6ec471e45098d2e812d3ffea
```

Letter case does not change the meaning of a hexadecimal hash, but any missing, added, or replaced character means that the value does not match.

### Build

This is the build identifier displayed or recorded within the application.

```text
G.E.N.E_Alpha_v1.0_R10-4D-4_Build-005
```

Use SHA-256 as the primary archive verification value. The build identifier is supplementary internal identification.

### Release Identity SHA-256

This value identifies the Release Record.

```text
1ac70e76edc2225e69f80d33b4bb60c2d01bb8fd135b14e4cdb8bae7367cbcc9
```

It is not the SHA-256 of the application archive. Use the archive SHA-256 above when verifying the downloaded archive.

## 3. Verification with Windows PowerShell

### SHA-256

Open PowerShell in the directory containing the archive and run:

```powershell
Get-FileHash ".\G.E.N.E_Alpha_v1.0_Windows_x64.zip" -Algorithm SHA256
```

Confirm that the displayed `Hash` matches:

```text
420DB62DBB6763AEBE01A5E0AB0225EBDAFDB9BC6EC471E45098D2E812D3FFEA
```

### File Size

```powershell
(Get-Item ".\G.E.N.E_Alpha_v1.0_Windows_x64.zip").Length
```

Confirm that the result is:

```text
79504332
```

### Combined Example

```powershell
$file = ".\G.E.N.E_Alpha_v1.0_Windows_x64.zip"

Get-Item $file | Select-Object Name, Length
Get-FileHash $file -Algorithm SHA256
```

## 4. Verification with Windows certutil

From Command Prompt:

```cmd
certutil -hashfile "G.E.N.E_Alpha_v1.0_Windows_x64.zip" SHA256
```

Confirm that the displayed SHA-256 matches the fixed value in this document.

## 5. Verification on Linux or macOS

The target platform is Windows x64, but the archive may also be checked from another environment.

### Linux

```bash
sha256sum G.E.N.E_Alpha_v1.0_Windows_x64.zip
stat -c %s G.E.N.E_Alpha_v1.0_Windows_x64.zip
```

### macOS

```bash
shasum -a 256 G.E.N.E_Alpha_v1.0_Windows_x64.zip
stat -f %z G.E.N.E_Alpha_v1.0_Windows_x64.zip
```

## 6. When Values Do Not Match

Do not treat a file as the official archive when any of the following does not match:

- Filename
- File size
- SHA-256

First, obtain the file again from the official GeneSIS BOOTH page.

If the values still do not match, do not run or extract the file. Contact the official GeneSIS route described in [Contact and Support](./CONTACT_AND_SUPPORT_EN.md).

When an unresolved security issue is suspected, do not post details in a public Issue or on social media. Use the private route in the [Security Policy](../SECURITY_EN.md).

## 7. Release Archive Verification Evidence

The fixed official archive completed the following internal release verification:

| Item | Result |
|---|---|
| Release Archive Verification Status | `PASS` |
| ZIP integrity | `PASS` |
| Release Manifest signature | `Ed25519 / PASS` |
| Artifacts listed in the Release Manifest | `75 / 75 matched` |
| `09_SHA256SUMS.txt` | `75 / 75 matched` |

```text
Release Archive Verification Status:
PASS
```

This result is release evidence for fixation of the official archive, verification of the Manifest signature, and internal artifact matching.

Checks performed through BOOTH or another delivery route are maintained separately as internal activity evidence of the GeneSIS-Operator. A delivery-route check does not change the file size, SHA-256, build, or Release Identity stated in this document.

## 8. Relationship to the Founder Package

The initial Founder package contains the same official G.E.N.E application archive as the free distribution.

The following file inside the Founder package must match the fixed values in this document:

```text
G.E.N.E_Alpha_v1.0_Windows_x64.zip
```

The outer Founder package ZIP has its own filename, file size, and SHA-256.

```text
G.E.N.E application archive SHA-256
is not the same as
Founder package outer ZIP SHA-256.
```

The verification values for the outer Founder package ZIP will be recorded in an external verification record after the package is complete. They will not replace or be mixed with the archive SHA-256 in this document.

## 9. Updates and Replacement

The official G.E.N.E Alpha v1.0 archive will not be modified.

Updates to documentation, support routes, or Known Limitations do not modify the fixed application archive.

Later G.E.N.E v1.x releases will be distributed as separately versioned files.

GeneSIS will not silently replace the content of an existing official archive while retaining the same filename.

---

Copyright © 2026 GeneSIS: Concept Engineer's HQ. All rights reserved.
