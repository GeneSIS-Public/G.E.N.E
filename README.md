# G.E.N.E

[English](./README_EN.md)

> **AIが変わっても、あなたの対話と思考まで失う必要はない。**

**人間側に、AIとの継続性を作る。**

G.E.N.Eは、AIとの対話を一時的なChatで終わらせず、話者、由来、原文および文脈を保持したLocal Dataとして記録・運用するための、Windows x64向けローカルAI対話環境です。

G.E.N.EはLLM本体ではありません。文章生成には、Ollama等の外部ローカルLLM環境と、利用可能なModelが別途必要です。

## Current Release

| 項目 | 内容 |
|---|---|
| Release | `G.E.N.E Alpha v1.0` |
| Project / Phase | `Project: Code-NOAH / Phase 1` |
| Product Line | `G.E.N.E v1.x` |
| Platform | `Windows x64` |
| Build | `G.E.N.E_Alpha_v1.0_R10-4D-4_Build-005` |
| Public Release Date | `2026-07-31` |
| Status | `Released — 2026-07-31` |

G.E.N.E Alpha v1.0は、Project: Code-NOAH Phase 1における最初の公式Releaseとして、2026-07-31に一般公開しました。

`Alpha`は非公式Prototypeや作業途中のPackageを意味しません。このReleaseで定義した最小G.E.N.E仕様は実装・試験済みです。一方、一般公開後の運用履歴、互換性情報および外部Runtime・Modelとの組合せ検証は初期段階にあります。

詳しい位置づけは、[Release Information](./docs/RELEASE_INFORMATION.md)をご確認ください。

## Main Functions

- 外部ローカルLLM環境への接続
- Personaの作成・選択・管理
- Dialogue Historyの保存と参照
- Summaryの作成・保存・再利用
- Knowledgeの登録と利用
- 外部資料としてのReferenceファイルの登録と利用
- 話者、由来、原文および文脈を保持するLocal Data構造

機能の詳細と現在の制約は、[Known Limitations](./docs/KNOWN_LIMITATIONS.md)をご確認ください。

## Download

G.E.N.E本体は無料です。

公式配布はGeneSIS公式BOOTH上のG.E.N.E無料商品ページで行います。

- [GeneSIS公式BOOTH Shop](https://genesis-protocol.booth.pm/)

無料商品ページ直接URL：

- [G.E.N.E Alpha v1.0 — Windows x64 無料配布版](https://genesis-protocol.booth.pm/items/8663637)

Founder Support商品ページ：

- [Project: Code-NOAH Phase 1 Founder Support](https://genesis-protocol.booth.pm/items/8664431)

支払い、Founder Supportへの参加、BOOSTその他の追加支援の有無によって、対応するG.E.N.E本体の機能は変わりません。

## Before Use

- 重要なDataは、G.E.N.Eだけを唯一の保存先にせずBackupしてください。
- 外部Runtime、Model、OSおよびHardwareの全組合せに対する互換性を保証しません。
- Modelを変更しても、同一の回答、挙動または人格的同一性を保証しません。
- AI出力の正確性、完全性または安全性を保証しません。
- 取得したArchiveは、展開・実行前にFile SizeとSHA-256を確認してください。

## Documentation

### Release

- [Release Information](./docs/RELEASE_INFORMATION.md)
- [Release Verification](./docs/RELEASE_VERIFICATION.md)
- [Known Limitations](./docs/KNOWN_LIMITATIONS.md)
- [Changelog](./CHANGELOG.md)

### Operation

- [Contact and Support](./docs/CONTACT_AND_SUPPORT.md)
- [Security Policy](./SECURITY.md)
- [Privacy Notice](./docs/PRIVACY_NOTICE.md)

### Terms and Founder

- [EULA — Download前確認用Copy](./docs/EULA.md)
- [Founder Terms](./docs/FOUNDER_TERMS.md)

文書一覧と英語公式翻訳は、[Documentation Index](./docs/README.md)をご確認ください。

## Contact

| 内容 | 経路 |
|---|---|
| 公開可能な通常不具合・文書Feedback・開発Feedback | GitHub Issues |
| 購入・Founder照合・利用条件・権利・Privacy・非公開連絡 | [Contact and Support](./docs/CONTACT_AND_SUPPORT.md) |
| 未修正のSecurity問題 | [Security Policy](./SECURITY.md) |

公開Issueへ個人情報、認証情報、購入情報、私的な対話履歴または未修正脆弱性の詳細を投稿しないでください。

## Source Repository、配布形式および利用条件

G.E.N.EのSource Repositoryは公開していません。

G.E.N.EはExecutable Application Archiveとして配布し、独立したPython Source File、開発環境、Build Scriptおよび内部開発履歴は、利用者向け成果物として別途提供しません。

Download前確認用の[EULA Copy](./docs/EULA.md)をGitHub上で確認できます。G.E.N.E本体の利用条件は、正式配布Archiveに同梱された`EULA.txt`を正本として管理します。

## Official Media

| 目的 | 公式媒体 |
|---|---|
| 公式配布・Founder Support | [BOOTH](https://genesis-protocol.booth.pm/) |
| 思想・開発背景・連載・公式声明 | [note](https://note.com/genesis_protocol) |
| 告知・宣伝・開発進捗 | [X](https://x.com/GeneSIS_PRCL) |
| GeneSIS公式技術領域 | [GitHub Organization](https://github.com/GeneSIS-Public) |

**GeneSIS by Concept Engineer's HQ.**

---

Copyright © 2026 GeneSIS: Concept Engineer's HQ. All rights reserved.
