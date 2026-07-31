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

> 本書の日本語版を原文および正本として管理します。英語版その他の翻訳版との間に解釈上の差異がある場合は、適用法令上許される範囲で日本語版を優先します。

本書は、G.E.N.E Alpha v1.0について、現在確認されている制約、公式対応を表明しない環境、十分な試験が完了していない条件および重要な利用上の注意を示します。

記載されていない問題が存在しないこと、または記載した制約が将来すべて解消されることを保証するものではありません。

## 1. 制約の区分

本書では、各事項を次の観点で扱います。

- **確認済み制約**：現在の公式Buildの仕様または構造から確認できる制約
- **非対応環境**：現Releaseで公式対応を表明しない環境
- **未試験条件**：十分な試験または互換性確認が完了していない条件
- **外部依存**：OS、Hardware、Runtime、Modelその他の外部要素へ主として依存する事項
- **運用上の注意**：Data保護や安全な利用のために必要となる注意

非対応または未試験であることは、必ずしも動作不能が確認されていることを意味しません。

また、「発生する場合がある」と記載する事項が、すべての環境で発生することを意味するものでもありません。

## 2. 概要

| 項目 | 現在の位置づけ |
|---|---|
| Platform | Windows x64のみを公式対象とする |
| AI Runtime | 外部ローカルLLM環境が必要 |
| Model互換性 | すべてのModel・Runtime Versionを保証しない |
| 性能 | Hardware、Model、Runtimeおよび設定に依存する |
| AI出力 | 正確性、一貫性または安全性を保証しない |
| 対話継続性 | 保存ContextはModel間のIdentity同一性を保証しない |
| Local Data | 利用者自身によるBackupが必要 |
| Cloud Backup | GeneSISによるCloud Backup・同期はない |
| 将来互換性 | Data・設定・外部環境の完全な後方互換性を保証しない |
| 公開運用履歴 | 一般公開後の互換性・不具合情報は蓄積初期段階 |

## 3. Alpha段階

G.E.N.E Alpha v1.0は、今回定義した最小G.E.N.E仕様を実装・試験済みの公式Releaseです。

`Alpha`は、非公式Prototype、作業途中のPackageまたは未完成実装を意味しません。

一方、一般公開後の運用履歴、利用者環境での互換性情報、外部Runtime・Modelとの組合せ試験および公開文書の成熟度は初期段階です。

そのため、次が存在する可能性があります。

- 未確認の不具合
- 特定環境だけで発生する起動・表示・保存・通信上の問題
- 十分に試験されていないWorkflow
- 将来Releaseで調整される設定、形式または挙動
- 修正または外部環境の更新によって生じる互換性差異

Alphaの詳しい位置づけは、[Release Information](./RELEASE_INFORMATION.md)をご確認ください。

## 4. 対象Platform

公式対象Platformは次のとおりです。

```text
Windows x64
```

次の環境は、現Releaseで公式対応を表明しません。

- 32-bit Windows
- Windows on ARM
- macOS
- Linux
- Mobile OS
- Browserのみの環境
- GeneSISが個別に確認していない仮想化環境
- GeneSISが個別に確認していない互換Layer
- GeneSISが個別に確認していないRemote Desktop環境

非対応または未試験環境では、起動不能、表示差異、保存・通信の失敗、性能低下その他の異なる挙動が発生する場合があります。

## 5. 外部RuntimeとModel

G.E.N.EはLLM本体ではなく、単独では文章を生成しません。

AI Responseには、Ollama等の外部ローカルLLM環境と、利用可能なModelが別途必要です。

公式Packageで明示されない限り、外部Runtime、Modelおよびそれらの実行に必要なComputer ResourceはG.E.N.E Archiveに含まれません。

利用者は、次を自身で管理します。

- 外部Runtimeの導入、設定および更新
- Modelの取得、選択および保存
- 各Software・ModelのLicenseと利用条件
- Hardwareおよび用途への適合性
- 外部環境のSecurityとNetwork設定

外部Runtimeで利用可能なModelであっても、すべてのG.E.N.E機能で正しく動作するとは限りません。

次の差異が発生する場合があります。

- 予期しないResponse形式
- 指示またはRoleへの追従失敗
- 日本語性能の低下
- Context長の制限
- 応答遅延またはTimeout
- 不完全または不正な形式の出力
- Runtime・Model更新後の挙動変化

GeneSISは、すべてのRuntime、Runtime Version、ModelまたはModel Versionとの互換性を保証しません。

## 6. Hardwareと性能

性能は、主として次に依存します。

- CPU・GPU性能
- 利用可能RAM・VRAM
- Storage速度と空き容量
- Model SizeとQuantization
- Context長
- Background Process
- 発熱・電力制限
- 外部Runtimeの設定

現時点では、すべての利用可能Modelで一定の性能を保証する単一のHardware要件を定めていません。

環境によって、起動遅延、Response遅延、高Memory使用、Model Load失敗、Timeout、System全体の低速化またはOS・外部Runtimeによる処理終了が発生する場合があります。

固定された応答時間、生成速度または性能水準を保証しません。

## 7. AI出力と対話継続性

AI出力は、利用者が選択した外部Modelによって生成されます。

出力には、次が含まれる場合があります。

- 不正確または古い情報
- 不完全、矛盾または捏造された内容
- 不適切または偏った表現
- 同じ入力に対する異なる結果
- 特定状況で危険となる提案

G.E.N.Eは、すべての生成内容を独立して検証しません。重要な情報は利用者が別途確認してください。

G.E.N.Eは、人間側に対話記録とContextの継続性を構築するための環境です。

ただし、接続Model、Model Version、System Instruction、Persona、Context容量、RuntimeまたはG.E.N.E Versionが変わると、回答、解釈および挙動も変わる場合があります。

保存Contextの継続性は、異なるModel間でのIdentity、記憶解釈、感情表現または推論挙動の同一性を保証しません。

## 8. Local Data、Backupおよび移行

G.E.N.EはLocal動作を前提とします。

ただし、代替不能な情報の唯一の保管場所として使用しないでください。

利用者は、重要な対話履歴、Persona、Summary、Knowledge、Reference、設定および関連Fileを、自身の責任でBackupしてください。

次の原因によって、Dataの消失、破損または利用不能が生じる可能性があります。

- 偶発的削除または上書き
- Storage故障
- OS・Application・Runtimeの異常終了
- 保存中断
- Security Softwareその他の外部Software
- 利用者によるFile・設定の直接変更
- 将来Versionとの非互換

GeneSISは、利用者のLocal G.E.N.E Dataを保存するCloud Backupまたは同期Serviceを運営しません。

公式Migration手順または互換性情報が公開されない限り、将来VersionとのData・設定互換性を保証しません。

更新または再導入を行う前に、重要DataのBackupを作成してください。

## 9. Networkと外部構成要素

G.E.N.EはLocal AI環境での使用を前提とします。

ただし、利用者が選択した外部Runtime、Model管理Tool、Model Download機能、OS Service、Security Softwareその他の第三者構成要素がNetwork通信を行わないことまでは保証しません。

利用者は、各外部構成要素の設定、Documentation、利用条件、Privacy PolicyおよびNetwork挙動を確認してください。

GeneSIS-Operatorは、外部提供者による独立したData処理またはService変更を管理しません。

G.E.N.E本体と個人情報の基本的な取扱いは、[Privacy Notice](./PRIVACY_NOTICE.md)をご確認ください。

## 10. Archive検証とSecurity警告

取得したArchiveは、展開・実行前に、公式配布経路、File SizeおよびSHA-256を確認してください。

固定値と検証方法は、[Release Verification](./RELEASE_VERIFICATION.md)を正本とします。

SHA-256の一致は、取得したArchiveが固定済み公式Archiveと同一であることを確認する手段です。ただし、それだけで次を保証するものではありません。

- Softwareが無欠陥であること
- すべての環境で安全・正常に動作すること
- すべての内部構成要素が独立監査済みであること
- 到達した配布ページ自体が公式であること

Windows、BrowserまたはSecurity Softwareが、Download Reputation、取得元、Application ReputationまたはCode Signing状態に応じて警告を表示する場合があります。

`Release Record Signed Date`はGeneSISのRelease記録に関する日付であり、それだけでMicrosoft Authenticode等のOS Code Signing状態を示すものではありません。

File名だけを理由に警告を無視せず、公式導線とArchive SHA-256を確認してください。

未修正のSecurity問題が疑われる場合は、公開IssueまたはSNSへ詳細を投稿せず、[Security Policy](../SECURITY.md)の非公開経路を使用してください。

## 11. Updateと将来互換性

将来のG.E.N.E v1.xでは、次が変更される場合があります。

- UIおよび操作手順
- 設定項目
- 対応Runtime・Model
- Dialogue処理
- 内部File・Data形式
- 導入・Directory構造
- 対応・非対応環境
- Documentation

すべてのAlpha段階File、設定、Data形式または外部Runtimeとの無期限の後方互換性を保証しません。

既存環境を更新または置換する前に、対象ReleaseのRelease Information、Known Limitations、Changelogおよび公開されている場合はMigration手順を確認してください。

後続ReleaseはVersionを識別できる別Fileとして配布され、G.E.N.E Alpha v1.0の固定済み公式Archive自体は変更されません。

## 12. 高Risk用途と報告

G.E.N.E Alpha v1.0は、次の用途について認証された製品ではありません。

- 医療診断または治療判断
- 確定的な法律判断または法的代理
- 金融取引または投資判断
- 緊急対応
- Vehicle、MachineryまたはCritical Infrastructureの制御
- Access Control、本人確認またはAuthentication判断
- 誤回答が直接重大な損害を生む判断

このような用途と関連して利用する場合は、人間による確認、独立検証および用途に応じた安全措置が必要です。

公開可能な制約、文書上の問題または再現可能な通常不具合は、[Contact and Support](./CONTACT_AND_SUPPORT.md)に記載するGitHub経路から報告してください。

個人情報、認証情報、私的対話、Founder照合情報または未修正脆弱性の詳細を、公開Issueへ投稿しないでください。

---

Copyright © 2026 GeneSIS: Concept Engineer's HQ. All rights reserved.
