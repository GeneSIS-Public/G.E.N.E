# G.E.N.E Alpha v1.0 — Release Information

- **Document Version:** v0.5
- **Status:** Active — Public Release
- **Published By:** GeneSIS
- **Operating Entity:** GeneSIS-Operator
- **Project:** Project: Code-NOAH
- **Phase:** Phase 1
- **Product Line:** G.E.N.E v1.x
- **Current Release:** G.E.N.E Alpha v1.0
- **Public Release Date:** `2026-07-31`
- **Target Platform:** Windows x64
- **Build:** `G.E.N.E_Alpha_v1.0_R10-4D-4_Build-005`
- **Official Distribution URL:** https://genesis-protocol.booth.pm/items/8663637
- **Established:** 2026-07-31
- **Effective From:** 2026-07-31
- **Last Updated:** 2026-09-11

> 本書の日本語版を原文および正本として管理します。英語版その他の翻訳版との間に解釈上の差異がある場合は、適用法令上許される範囲で日本語版を優先します。

## 1. Release概要

| 項目 | 内容 |
|---|---|
| 製品 | `G.E.N.E Alpha v1.0` |
| Project | `Project: Code-NOAH` |
| Phase | `Phase 1` |
| Product Line | `G.E.N.E v1.x` |
| Platform | `Windows x64` |
| Build | `G.E.N.E_Alpha_v1.0_R10-4D-4_Build-005` |
| 配布形式 | ZIP Archive |
| 配布元 | GeneSIS公式BOOTH |
| 価格 | 無料 |
| 支援状況による機能差 | なし |
| Source Code | 非公開 |

公式Archive名：

```text
G.E.N.E_Alpha_v1.0_Windows_x64.zip
```

ArchiveのFile Size、SHA-256、Release Identityおよび検証方法は、[Release Verification](./RELEASE_VERIFICATION.md)を正本として確認してください。

## 2. G.E.N.Eとは何か

G.E.N.Eは、AIとの対話を一時的なChatで終わらせず、話者、由来、原文および文脈を保持したローカル資産として記録・運用するための、Windows x64向けローカルAI対話環境です。

中心となるConceptは次のとおりです。

> AIが変わっても、あなたの対話と思考まで失う必要はない。  
> 人間側に、AIとの継続性を作る。

G.E.N.Eは、Persona、History、Summary、KnowledgeおよびReferenceを、利用者自身の環境で管理するための対話環境を提供します。

G.E.N.EはLLM本体ではありません。文章生成には、Ollama等の外部ローカルLLM環境と、利用可能なModelが別途必要です。

## 3. 外部環境と利用者の管理範囲

G.E.N.E Application Archiveには、明示されていない限り、外部ローカルLLM環境、Modelおよびそれらの実行に必要なComputer Resourceは含まれません。

利用者は、次を自身で管理します。

- 外部ローカルLLM環境の導入と設定
- Modelの取得と選択
- Hardwareおよび用途との適合性
- 外部Software・ModelのLicenseと利用条件
- Local Computerと接続環境の安全管理
- 重要DataのBackup

性能、出力品質、言語能力および挙動は、OS、Hardware、Runtime、Modelおよび設定によって異なります。

すべての組合せで同一の動作または回答を保証するものではありません。

現在の制約、未検証範囲および利用上の注意は、[Known Limitations](./KNOWN_LIMITATIONS.md)をご確認ください。

## 4. Local動作とData

G.E.N.EはLocal動作を前提としています。

通常利用において、GeneSISは、G.E.N.E内の対話履歴、Persona、Summary、Knowledge、Reference、Promptまたは接続Modelの入出力を自動的に収集しません。

利用者が不具合報告または問い合わせのために自ら送信した情報は、その送信範囲で取り扱います。

接続する外部Software、ModelまたはServiceには、それぞれ独自のNetwork動作、利用条件またはData取扱いが存在する場合があります。

詳細は、[Privacy Notice](./PRIVACY_NOTICE.md)をご確認ください。

## 5. Alpha v1.0の位置づけ

G.E.N.E Alpha v1.0は、Project: Code-NOAH Phase 1における最初の公式公開Releaseです。

`Alpha`は、非公式Prototype、作業途中のPackageまたは未完成の実装を意味しません。

このReleaseで定義した最小G.E.N.E仕様は実装・試験済みであり、公式Archiveとして固定されています。

一方、次の領域は初期段階にあります。

- 一般公開後の運用履歴
- 対応環境と互換性の蓄積
- 外部Runtime・Modelとの組合せ検証
- 利用者環境に固有の動作確認
- 公開文書と仕様説明の成熟度

したがって、次を区別します。

```text
実装完了
≠
Project全体のRoadmap完了

公式Release
≠
無欠陥または全環境対応

Alpha
≠
非公式Prototype
```

未確認の不具合、環境固有の挙動または将来調整される仕様が存在する可能性があります。

## 6. 無料配布とFounder Support

G.E.N.E Alpha v1.0本体は無料で配布します。

支払い、Founder Supportへの参加、BOOSTその他の追加支援の有無によって、対応するG.E.N.E本体の機能、利用可能範囲または基本的なSupport範囲を変更しません。

無料配布版とFounder初期Packageに含まれるG.E.N.E本体Archiveは、同一Build・同一SHA-256です。

Founder SupportはG.E.N.Eの上位版購入ではなく、Project: Code-NOAH Phase 1への明示的な参加・支援です。

Founder資格、価格、Founder成果物、Supplemental / Additional Deliverable、期限非保証その他の正式条件は、Current Founder初期Packageに同梱された日本語Founder Terms TXTを正本として確認してください。GitHub上の[Founder Terms](./FOUNDER_TERMS.md)は購入前確認用Public Reference Copyです。

現在提供中のFounder成果物、Supplemental / Additional Deliverable、後日提供対象および関連文書は、[Founder Support Information](./FOUNDER_SUPPORT_INFORMATION.md)に集約しています。

Founder Support商品ページ：

https://genesis-protocol.booth.pm/items/8664431

## 7. 配布方針

G.E.N.E Phase 1 / v1.xの公式配布は、GeneSIS公式BOOTH上のG.E.N.E無料商品ページで行います。

```text
https://genesis-protocol.booth.pm/items/8663637
```

この商品ページは、G.E.N.E Phase 1 / v1.xの継続的な公式配布ページとして運用します。

後続のv1.x Releaseは、Versionを識別できる別Fileとして追加します。

既存の公式Archiveを、同名Fileのまま無言で差し替えません。

G.E.N.E無料商品ページでは、G.E.N.E v1.xの公式Releaseを配布します。Founder Supportに関するFounder成果物およびSupplemental / Additional Deliverableは、Founder Supportの条件と提供経路に従って別に取り扱います。Currentな提供対象はFounder Support Informationを確認してください。

## 8. 公式情報源

### BOOTH

BOOTHは、G.E.N.Eの公式配布、Founder Supportの受付および購入記録を取り扱う媒体です。

- G.E.N.E無料配布：https://genesis-protocol.booth.pm/items/8663637
- Founder Support：https://genesis-protocol.booth.pm/items/8664431

### GitHub

このRepositoryは、G.E.N.Eに関する確定した技術情報、Release情報、検証情報、Known Limitationsおよび公開文書を固定する公式技術媒体です。

GitHubは、決済、購入記録またはFounder資格の正本ではありません。

### 問い合わせ

公開可能な通常不具合はGitHub Issues、購入・Founder照合・権利・Privacyその他の非公開連絡は、[Contact and Support](./CONTACT_AND_SUPPORT.md)に記載する経路を使用してください。

未修正のSecurity問題は、[Security Policy](../SECURITY.md)の非公開経路を使用してください。

## 9. Source Repository、配布形式および利用条件

G.E.N.EのSource Repositoryは公開していません。

G.E.N.Eは、Executable Application Archiveとして配布します。独立したPython Source File、開発環境、Build Scriptおよび内部開発履歴は、利用者向け成果物として別途提供しません。

Application Archive、Documentation、Release情報または検証値の公開は、Source RepositoryへのAccess権、Source Codeの取得権または利用Licenseを付与するものではありません。

G.E.N.E Alpha v1.0のEULAは、Download前確認用Copyとして[こちら](./EULA.md)から確認できます。

G.E.N.E本体の利用条件は、正式配布Archiveに同梱された`EULA.txt`を正本として管理します。GitHub掲載版と正式配布Archive内のEULAとの間に差異がある場合は、正式配布Archive内の`EULA.txt`を優先します。

本書はEULAを置き換えません。

---

Copyright © 2026 GeneSIS: Concept Engineer's HQ. All rights reserved.
