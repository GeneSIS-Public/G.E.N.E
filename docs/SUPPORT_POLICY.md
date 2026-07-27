# G.E.N.E / GeneSIS Common Support Policy

* **Document Version:** v0.1
* **Established:** ［制定日］
* **Effective From:** ［適用開始日］
* **Published By:** GeneSIS
* **Applicable Project:** Project: Code-NOAH
* **Applicable Product:** G.E.N.E Alpha v1.0

## 1. Purpose

このSupport Policyは、G.E.N.EおよびGeneSISが公開する関連成果物について、問い合わせの受付範囲、対応方針、対象外事項および連絡経路を定めるものです。

G.E.N.Eを無料で利用する場合、Phase 1 Founderとして参加する場合、またはその他の経路で任意支援を行う場合を含め、原則としてすべての利用者へ共通して適用します。

本Policyは、個別対応、返信、問題解決、修正または一定期間内の対応を保証する契約、Service Level Agreementまたは優先Support契約ではありません。

## 2. Support Principles

GeneSISは、次の原則に基づいてSupportを運用します。

> 品質は妥協しない。
> 利用障壁は高くしない。
> 価値を安売りもしない。

技術的不具合、問い合わせおよびFeedbackの評価は、主として次の要素を考慮して行います。

* 再現性
* 影響範囲
* 重大性
* 安全性
* データ消失または破損の可能性
* 利用者への影響
* 技術的実現性
* 製品思想および開発方針との整合
* 現在の開発状況

支援額、Founder参加の有無、購入回数または任意支援の経路によって、技術的評価、問い合わせ対応順位、修正順位または基本的な応対方針を変更しません。

受付順と対応順は一致しない場合があります。

## 3. Supported Products

本Policyの初版で対象とする製品は、次のとおりです。

| Product             | Support Status |
| ------------------- | -------------- |
| G.E.N.E Alpha v1.0  | 正式一般公開後に対象     |
| 開発途中Build           | 対象外            |
| 内部運用版               | 対象外            |
| 未公開試験版              | 対象外            |
| 第三者が改変したPackage     | 対象外            |
| 非公式Buildまたは非公式Patch | 対象外            |

G.E.N.E Alpha v1.0は現在、一般公開準備中です。

正式なSupport運用の開始時に、本表および関連する受付状態を更新します。

O-type Generator Founder Edition、Gene-ScrIbe ConSole Founder Editionその他の関連成果物については、GeneSISが各成果物または公式文書で本Policyの適用を明示した時点から対象とします。

## 4. Public Technical Issues

公開可能で再現性のある通常の技術的不具合は、G.E.N.E公式RepositoryのGitHub Issuesで受け付けます。

Issueへ投稿する際は、可能な範囲で次の情報を記載してください。

* G.E.N.EのVersionまたはBuild
* 使用しているOSおよび実行環境
* 接続しているローカルLLM環境
* 使用しているLLMモデル
* 問題の概要
* 問題が発生するまでの操作
* 再現条件または再現手順
* 期待していた動作
* 実際に発生した動作
* 再現頻度
* 関連するLogまたは画面情報
* 確認済みの回避方法

すべての項目を記載する必要はありません。

ただし、再現に必要な情報が不足している場合、GeneSISが問題を確認または調査できないことがあります。

GitHub Issuesは、原則として第三者が閲覧できる公開領域です。

個人情報、認証情報、購入情報、私的な対話履歴、Persona情報、非公開資料または第三者へ公開すべきでない情報は投稿しないでください。

## 5. Private Contact

次の内容は、GitHub IssuesではなくGeneSIS公式窓口へご連絡ください。

* 購入に関する問い合わせ
* Founder資格または購入記録の照合
* 利用条件、配布条件または権利に関する問い合わせ
* 個人情報に関する連絡
* 公開に適さない技術的不具合
* Security上の懸念
* GitHub Issuesを利用できない特別な事情があり、公開可能な代替手段がない場合の連絡
* その他、公開の場で扱うことが適切でない問い合わせ

**GeneSIS 公式窓口 - Official Contact**

`genesis.official.poc@mail.com`

問い合わせ経路、件名例、Founder照合に必要な情報および送信してはならない情報の詳細は、[Contact and Support](./CONTACT_AND_SUPPORT.md)を確認してください。

## 6. Security Reports

Security上の懸念は、公開のGitHub Issue、SNSまたはその他の公開場所へ投稿しないでください。

このRepositoryで非公開脆弱性報告機能が有効になっている場合は、GitHub Security画面の非公開報告経路を使用してください。

利用できない場合は、GeneSIS公式窓口へ非公開でご連絡ください。

Security報告の対象範囲、必要情報および開示方針の詳細は、Repository直下の[Security Policy](../SECURITY.md)を確認してください。

問題がSecurity上の懸念に該当するか判断できない場合も、公開場所へ詳細を投稿せず、非公開経路を使用してください。

## 7. Included Support

GeneSISは、必要性、技術的実現性および開発状況を考慮し、次の対応を行うことがあります。

* 公開可能な技術的不具合の確認
* 再現条件の調査
* Known Limitationsの案内
* 公式文書の訂正または補足
* 回避方法が存在する場合の案内
* 修正版または更新版の検討
* Security上の懸念の確認
* 利用条件、権利またはFounder資格に関する案内
* 公式配布物および検証情報の確認

これらは、個別案件について必ず実施することを保証するものではありません。

## 8. Support Not Included

無料利用、Founder参加、BOOSTまたはその他の任意支援には、原則として次の個別対応は含まれません。

* 個別PCへの導入代行
* Remote操作による設定または調査
* 個別環境への訪問対応
* Ollamaその他のローカルLLM環境の導入代行
* LLMモデルの選定または導入代行
* 個別Personaの作成
* Promptの個別設計
* 対話履歴の変換、分類または整理代行
* 個別KnowledgeまたはReferenceの構築
* 個別環境向けのカスタマイズ
* Source Codeの提供
* 内部設計資料の提供
* 開発途中Buildまたは未公開試験版の提供
* 継続的な個別Consulting
* 利用者データの復旧
* 第三者製品自体のSupport
* EULAまたは適用法令に反する利用への支援

GeneSISが別途、特定の対応またはServiceを明示的に提供した場合は、その個別条件が適用されます。

## 9. External Products and Environments

G.E.N.Eは、Ollama、ローカルLLM、OSおよびその他の外部環境と組み合わせて使用されます。

外部製品の仕様、障害、更新、互換性、利用条件、提供終了またはモデル固有の挙動について、GeneSISは管理または保証できません。

次の問題は、原則として外部製品の提供元へ確認してください。

* Ollama自体の導入または起動に関する問題
* LLMモデル自体の品質、性能または回答傾向
* OS、DriverまたはHardware固有の問題
* 外部製品の利用条件またはAccountに関する問題
* G.E.N.Eを使用しなくても発生する外部製品単体の問題

ただし、外部製品との連携によってG.E.N.E固有の問題が発生する場合は、参考情報として受け付けることがあります。

## 10. AI and LLM Output

G.E.N.EはLLMモデル本体ではありません。

LLMが生成する回答について、GeneSISは次の事項を保証しません。

* 正確性
* 完全性
* 最新性
* 特定目的への適合性
* 一貫性
* 不適切または意図しない出力が発生しないこと
* 法的、医療的、金融的その他の専門的判断への適合性

重要な判断では、生成内容を利用者自身が確認し、必要に応じて適切な専門家または一次情報を参照してください。

LLMの回答内容や品質のみを理由とする問題は、原則としてG.E.N.E本体の技術的不具合には該当しません。

## 11. User Data and Backups

G.E.N.Eは、対話、Persona、History、Summary、KnowledgeおよびReferenceを利用者の管理下で運用することを前提としています。

利用者は、必要なデータについて自己の責任でBackupを作成し、保存状態および復元可能性を確認してください。

Update、設定変更、データ移行または問題調査を行う前には、可能な範囲で重要データをBackupしてください。

GeneSISは、次の事項を保証しません。

* 利用者データの完全な保存
* 誤操作、機器故障または外部環境に起因するデータの復旧
* すべてのVersion間での完全な互換性
* 第三者Softwareによって変更または破損したデータの復旧
* 個別環境におけるBackup代行

データ消失または破損につながる可能性がある不具合を確認した場合は、利用を中断し、可能な範囲で既存データを保全した上で報告してください。

## 12. Founder and Voluntary Support

Phase 1 Founderは、G.E.N.Eの上位版または優先Support契約ではありません。

Founder参加、BOOTH BOOST、OFUSEその他の任意支援によって、次の事項は変化しません。

* G.E.N.E本体の機能
* 技術的不具合の評価基準
* 問い合わせ対応順位
* 修正順位
* 開発判断への影響力
* 個別Supportの範囲
* 基本的な応対方針

Founderの参加条件およびFounder向け成果物については、別途公開するFounder参加条件書およびFounder提供方針に従います。

## 13. Response and Resolution

GeneSISは、受け付けた内容を確認し、必要に応じて調査および対応方針を検討します。

ただし、次の事項を保証するものではありません。

* すべての問い合わせへの返信
* 一定期間内の返信
* 個別対応
* 問題の修正
* 要望の採用または実装
* 特定Versionでの修正
* 対応期限
* 利用者データの復旧
* 特定の結果

報告の受領は、問題がG.E.N.Eに由来すること、修正が必要であること、または報告者の見解にGeneSISが同意することを意味しません。

## 14. Feature Requests and Feedback

機能追加の要望、改善提案およびFeedbackは、今後の改善検討に使用することがあります。

ただし、受付は次の事項を保証しません。

* 採用
* 実装
* 実装時期
* 個別回答
* 提案者への権利付与
* 開発判断への参加権
* 利益分配その他の対価

Feedbackの技術的評価は、支援額、Founder参加の有無または購入回数によって変更しません。

秘密情報、未公開事業案、第三者の権利物または権利処理が必要な資料を、事前の合意なく送信しないでください。

## 15. Personal and Confidential Information

GeneSISは、問い合わせ対応に必要な範囲で、送信された個人情報、購入情報および非公開情報を確認・保管する場合があります。

これらの情報は、主として次の目的で使用します。

* 問い合わせ内容の確認
* Founderまたは購入記録の照合
* 不具合の調査
* 権利関係の確認
* 成果物の提供
* Security上の対応
* 法令上必要な対応

法令上必要な場合を除き、本人の同意なく、目的外で個人情報または非公開情報を公開しません。

Gmail、BOOTH、GitHubその他の外部サービスを通じて送信された情報には、各サービスの利用規約およびPrivacy Policyも適用されます。

調査に不要な個人情報、認証情報、対話履歴または機密情報を送信しないでください。

## 16. Communication Conduct

GeneSISは、次に該当する場合、問い合わせへの返信、調査または以後の対応を制限・終了することがあります。

* 暴言、脅迫、差別または嫌がらせ
* 過度に反復される連絡
* 同一要求への継続的な回答強要
* 個別対応を当然の義務として要求する行為
* 違法行為またはEULA違反への協力要求
* なりすまし
* 虚偽の購入情報
* Spamまたは不正な宣伝
* GeneSISまたは第三者の安全を脅かす行為
* 開発、運営または生活を著しく妨害する行為

技術的な批判、否定的な評価、正当な不具合報告または異なる意見のみを理由として対応を制限することはありません。

## 17. Social Media

SNSは、Release告知、更新情報、簡単な案内および公式導線の周知に使用します。

SNS上の投稿、Reply、MentionまたはDirect Messageは、正式なSupport受付経路ではありません。

SNS上で個人情報、購入情報、認証情報、私的な対話履歴または未修正のSecurity問題を送信しないでください。

## 18. Availability and Emergencies

GeneSISは、24時間監視、緊急電話窓口、即時対応、稼働率保証またはService Level Agreementを提供しません。

個人の生命、安全、医療、犯罪、災害その他の緊急事態について、本Support窓口を使用しないでください。

緊急性がある場合は、地域の公的機関、緊急窓口または適切な専門機関へ連絡してください。

## 19. Relationship with Other Documents

G.E.N.E本体の利用条件については、正式製品Packageに付属するEULAを優先します。

Founder参加に関する条件は、Founder参加条件書およびFounder提供方針に従います。

Security報告については、[Security Policy](../SECURITY.md)に定める内容を優先します。

問い合わせ経路と必要情報については、[Contact and Support](./CONTACT_AND_SUPPORT.md)を確認してください。

本Policyと他の公式文書でVersionまたは内容が異なる場合は、それぞれに記載された適用対象、制定日および適用開始日を確認してください。

## 20. Policy Updates

GeneSISは、製品の更新、運用状況、受付経路、法令または安全上の必要性に応じて、本Policyを改定することがあります。

改定時には、Document Version、制定日、適用開始日および必要に応じて変更内容を更新します。

重要な変更を行う場合は、BOOTH、GitHub、note、SNSその他の公式媒体を通じて、可能な範囲で告知します。

過去のVersionに適用される条件については、各文書に記載された適用対象および適用開始日を確認してください。

---

Copyright © 2026 GeneSIS: Concept Engineer's HQ. All rights reserved.
