# G.E.N.E Changelog

- **Document Version:** v0.3
- **Status:** Active — Public Release
- **Published By:** GeneSIS
- **Operating Entity:** GeneSIS-Operator
- **Applicable Product Line:** G.E.N.E v1.x
- **Established:** 2026-07-31
- **Effective From:** 2026-07-31

> 本書を日本語原文・正本として管理します。英語版その他の翻訳版との間に解釈上の差異がある場合は、日本語版を優先します。

本書は、G.E.N.Eの公式公開Versionごとに、利用者へ影響する追加、変更、修正、削除およびSecurity上の変更を記録します。

内部開発履歴、媒体設定、公開前Draft、監査過程および利用者へ影響しない軽微な文言修正は、原則として記録しません。

## [Unreleased]

現時点で、G.E.N.E Alpha v1.0の固定済み公式Archiveに対する未公開の製品変更はありません。

将来の変更は、公開Versionが確定した時点で、該当する項目へ記録します。

## [Alpha v1.0] — 2026-07-31

### Release

| 項目 | 内容 |
|---|---|
| Project | `Project: Code-NOAH` |
| Phase | `Phase 1` |
| Product Line | `G.E.N.E v1.x` |
| Platform | `Windows x64` |
| Build | `G.E.N.E_Alpha_v1.0_R10-4D-4_Build-005` |
| Public Release Date | 2026-07-31 |
| Release Record Signed Date | `2026-07-21` |

G.E.N.E Alpha v1.0は、Project: Code-NOAH Phase 1における最初の公式公開Releaseです。

### Added

- Windows x64向けG.E.N.E Application
- AIとの対話をLocal Dataとして記録・運用する基本環境
- Ollama等の外部ローカルLLM環境への接続機能
- Personaの作成・選択・管理
- Dialogue Historyの保存と参照
- Summaryの作成・保存・再利用
- Knowledgeの登録・利用
- 外部資料としてのReferenceファイルの登録・利用
- 話者、由来、原文および文脈を保持するための基本構造
- 利用者自身の環境で対話Dataを管理するLocal運用
- G.E.N.E Alpha v1.0の正式配布Package
- EULA、READMEその他の同梱文書
- 公式Release情報、Archive検証情報およびKnown Limitations

### Release Characteristics

- G.E.N.EはLLM本体ではなく、外部ローカルLLM環境とModelを別途必要とします。
- G.E.N.E本体は無料で配布します。
- Founder Support、BOOSTその他の支援状況によるG.E.N.E本体の機能差はありません。
- Source Codeは公開していません。
- 公式Archiveは固定済みであり、同名のまま内容を変更しません。
- 後続のG.E.N.E v1.xは、Versionを識別できる別Fileとして配布します。

### Verification

公式ArchiveのFile名、File Size、SHA-256、Release Identityおよび確認方法は、[Release Verification](./docs/RELEASE_VERIFICATION.md)を正本として確認してください。

### Known Limitations

現在の対応環境、未検証範囲、外部Runtime・Model依存、Backupおよび将来互換性に関する注意は、[Known Limitations](./docs/KNOWN_LIMITATIONS.md)をご確認ください。

### Notes

`Alpha`は、非公式Prototype、作業途中のPackageまたは未完成実装を意味しません。

このReleaseで定義した最小G.E.N.E仕様は実装・試験済みです。一方、一般公開後の運用履歴、互換性情報および外部Runtime・Modelとの組合せ検証は初期段階にあります。

詳しい位置づけは、[Release Information](./docs/RELEASE_INFORMATION.md)をご確認ください。

---

Copyright © 2026 GeneSIS: Concept Engineer's HQ. All rights reserved.
