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

> 本書の日本語版を原文および正本として管理します。英語版その他の翻訳版との間に解釈上の差異がある場合は、適用法令上許される範囲で日本語版を優先します。

本書は、G.E.N.E Alpha v1.0の公式Application Archiveを識別し、取得したFileが固定済みの公式Archiveと一致するか確認するための値と方法を示します。

## 1. 公式Archive

| 項目 | 固定値 |
|---|---|
| Product | `G.E.N.E Alpha v1.0` |
| File Name | `G.E.N.E_Alpha_v1.0_Windows_x64.zip` |
| File Size | `79,504,332 bytes` |
| Build | `G.E.N.E_Alpha_v1.0_R10-4D-4_Build-005` |
| SHA-256 | `420db62dbb6763aebe01a5e0ab0225ebdafdb9bc6ec471e45098d2e812d3ffea` |
| Release Identity SHA-256 | `1ac70e76edc2225e69f80d33b4bb60c2d01bb8fd135b14e4cdb8bae7367cbcc9` |
| Release Record Signed Date | `2026-07-21` |
| Internal Archive Verification | `PASS` |

これらの値は、G.E.N.E Alpha v1.0の固定済み公式Archiveを識別します。

公式Archive自体は変更、再圧縮または同名差替えを行いません。

## 2. 各値の意味

### File Name

公式ArchiveのFile名です。

File名だけでは内容の同一性を証明できないため、File SizeとSHA-256も確認してください。

### File Size

Archive全体のByte数です。

File Sizeが一致していても内容が同一とは限らないため、SHA-256による確認が必要です。

### SHA-256

公式Application ArchiveそのもののSHA-256です。

取得したFileのSHA-256が次と完全一致することを確認してください。

```text
420db62dbb6763aebe01a5e0ab0225ebdafdb9bc6ec471e45098d2e812d3ffea
```

大文字・小文字はHash値の意味を変えませんが、文字の欠落、追加または置換が一つでもある場合は一致していません。

### Build

Application内で識別されるBuild IDです。

```text
G.E.N.E_Alpha_v1.0_R10-4D-4_Build-005
```

Archive検証ではSHA-256を優先し、Build表示は内部識別の補助として使用します。

### Release Identity SHA-256

Release Recordを識別するための値です。

```text
1ac70e76edc2225e69f80d33b4bb60c2d01bb8fd135b14e4cdb8bae7367cbcc9
```

これはApplication ArchiveのSHA-256ではありません。Archive検証には前項のArchive SHA-256を使用してください。

## 3. Windows PowerShellでの確認

### SHA-256

PowerShellで、ArchiveがあるDirectoryへ移動し、次を実行します。

```powershell
Get-FileHash ".\G.E.N.E_Alpha_v1.0_Windows_x64.zip" -Algorithm SHA256
```

表示された`Hash`が次と一致することを確認します。

```text
420DB62DBB6763AEBE01A5E0AB0225EBDAFDB9BC6EC471E45098D2E812D3FFEA
```

### File Size

```powershell
(Get-Item ".\G.E.N.E_Alpha_v1.0_Windows_x64.zip").Length
```

表示結果が次であることを確認します。

```text
79504332
```

### 一括確認例

```powershell
$file = ".\G.E.N.E_Alpha_v1.0_Windows_x64.zip"

Get-Item $file | Select-Object Name, Length
Get-FileHash $file -Algorithm SHA256
```

## 4. Windows certutilでの確認

PowerShellを使用しない場合は、Command Promptで次を実行できます。

```cmd
certutil -hashfile "G.E.N.E_Alpha_v1.0_Windows_x64.zip" SHA256
```

表示されたSHA-256が本書の固定値と一致することを確認してください。

## 5. Linux・macOSでの確認

配布対象PlatformはWindows x64ですが、別環境でArchiveを確認する場合は次を利用できます。

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

## 6. 一致しない場合

次のいずれかが一致しない場合は、そのFileを公式Archiveとして扱わないでください。

- File名
- File Size
- SHA-256

まず、GeneSIS公式BOOTHから再取得してください。

再取得しても一致しない場合は、Fileを実行または展開せず、[Contact and Support](./CONTACT_AND_SUPPORT.md)に記載するGeneSIS公式窓口へ連絡してください。

未修正のSecurity問題が疑われる場合は、公開IssueやSNSへ詳細を投稿せず、[Security Policy](../SECURITY.md)の非公開経路を使用してください。

## 7. Release Archiveの検証証跡

固定済み公式Archiveは、Release時に次の内部検証を完了しています。

| 項目 | 結果 |
|---|---|
| Release Archive Verification Status | `PASS` |
| ZIP整合性 | `PASS` |
| Release Manifest署名 | `Ed25519 / PASS` |
| Release Manifest記載Artifact | `75 / 75 一致` |
| `09_SHA256SUMS.txt` | `75 / 75 一致` |

```text
Release Archive Verification Status:
PASS
```

この結果は、公式Archiveの固定、Manifest署名および内部Artifact照合に関するRelease証跡です。

BOOTHその他の配布経路上で行う取得確認は、本書のArchive識別値とは分離したGeneSIS-Operatorの内部活動証跡として管理します。配布経路上の確認結果によって、本書のFile Size、SHA-256、BuildまたはRelease Identityを変更しません。

## 8. Founder Packageとの関係

Founder初期Packageには、無料配布版と同じ公式G.E.N.E Application Archiveを格納します。

Founder Package内の次のFileは、本書の固定値と一致しなければなりません。

```text
G.E.N.E_Alpha_v1.0_Windows_x64.zip
```

Founder Packageの外側ZIPには、別のFile名、File SizeおよびSHA-256が設定されます。

```text
G.E.N.E Application Archive SHA-256
≠
Founder Package外側ZIP SHA-256
```

Founder Package外側ZIPの検証値は、Package完成後に外部Verification Recordへ記録します。本書のArchive SHA-256へ置き換えたり、混在させたりしません。

## 9. 更新と差替え

G.E.N.E Alpha v1.0の公式Archiveは変更しません。

文書、Support経路またはKnown Limitationsが更新されても、固定済みApplication Archiveへ変更を加えません。

後続のG.E.N.E v1.x Releaseは、Versionを識別できる別Fileとして配布します。

同じFile名のまま内容だけを変更する無言差替えは行いません。

---

Copyright © 2026 GeneSIS: Concept Engineer's HQ. All rights reserved.
