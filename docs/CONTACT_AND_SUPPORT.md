# Contact and Support

この文書では、G.E.N.EおよびGeneSISに関する問い合わせ窓口と、内容ごとの受付経路を案内します。

問い合わせ内容に応じて、GitHub Issues、GitHubの非公開脆弱性報告機能、またはGeneSIS公式窓口を使用してください。

Supportの対象範囲、対応方針および対象外事項の詳細は、[G.E.N.E / GeneSIS 共通Support Policy](./SUPPORT_POLICY.md)を確認してください。

## Public Technical Issues

公開可能で再現性のある通常の技術的不具合は、G.E.N.E公式RepositoryのGitHub Issuesで受け付けます。

Issueを作成する際は、可能な範囲で次の情報を記載してください。

* 使用しているG.E.N.EのVersionまたはBuild
* 使用しているOSおよび実行環境
* 接続しているローカルLLM環境
* 使用しているLLMモデル
* 問題の概要
* 問題が発生するまでの操作
* 再現手順
* 期待していた動作
* 実際に発生した動作
* 再現頻度
* 関連するLogまたは画面情報
* 確認済みの回避方法

すべての項目を記載する必要はありません。

ただし、再現に必要な情報が不足している場合、GeneSISが問題を確認または調査できないことがあります。

個人情報、Password、Access Token、API Key、秘密鍵その他の機密情報は、GitHub Issuesへ掲載しないでください。

次の内容は、公開Issueへ投稿しないでください。

* Security上の懸念
* 個人情報を含む問題
* 購入またはFounder資格に関する情報
* 非公開の利用条件または権利に関する相談
* 第三者が悪用できる未修正の問題
* 公開に適さないLog、File、Pathまたは画面情報
* 未加工の対話履歴、Persona情報または私的なデータ

## Security Reports

Security上の懸念は、公開のGitHub Issue、SNSまたはその他の公開場所へ投稿しないでください。

このRepositoryで非公開脆弱性報告機能が有効になっている場合は、GitHub Security画面の非公開報告経路を使用してください。

非公開脆弱性報告機能が利用できない場合は、GeneSIS公式窓口へ非公開でご連絡ください。

詳細は、Repository直下の[`SECURITY.md`](../SECURITY.md)を確認してください。

問題がSecurity上の懸念に該当するか判断できない場合も、公開Issueへ詳細を投稿せず、非公開経路を使用してください。

## Official Contact

次の内容は、GeneSIS公式窓口で受け付けます。

* 購入に関する問い合わせ
* Founder資格および購入記録の照合
* 利用条件、配布条件および権利に関する問い合わせ
* 個人情報に関する連絡
* 公開に適さない技術的不具合
* Security上の懸念
* GitHub Issuesを利用できない特別な事情があり、公開可能な代替手段がない場合の連絡
* その他、公開の場で扱うことが適切でない問い合わせ

**GeneSIS 公式窓口 - Official Contact**

`［genesis.official.poc@mail.com］`

問い合わせ内容が分かる件名を付けてください。

件名例：

```text
[Founder] Founder資格・購入記録の照合
[Rights] 利用条件・権利に関する問い合わせ
[Private Bug] 非公開の不具合報告
[Security Report] Security上の懸念
[Other] その他の非公開連絡
```

Security上の懸念を報告する場合は、件名の先頭に次の表記を付けてください。

```text
[Security Report]
```

## Founder Verification

Founder資格または購入記録の照合を依頼する場合は、可能な範囲で次の情報を記載してください。

* BOOTHの注文番号
* 対象商品名
* おおよその購入時期
* BOOTH上で確認可能なユーザー識別情報
* 問い合わせの目的

照合には、必要最小限の情報のみを送信してください。

次の情報は送信しないでください。

* BOOTH、Googleその他のPassword
* 2段階認証Code
* Backup Code
* Access Token
* API Key
* 秘密鍵
* クレジットカード番号
* 金融口座の認証情報

GeneSISから、これらの認証情報の提出を求めることはありません。

## GitHub Issues Are Not for Private Support

GitHub Issuesは、原則として第三者が閲覧できる公開領域です。

個人情報、購入情報、認証情報、非公開資料、私的な対話履歴または第三者へ公開すべきでない情報を含む問い合わせには使用しないでください。

公開Issueへ機密情報を誤って投稿した場合は、可能な範囲で速やかに内容を削除または編集し、GeneSIS公式窓口へご連絡ください。

Token、Password、秘密鍵その他の認証情報を公開してしまった場合は、投稿を削除するだけでなく、該当する認証情報を速やかに無効化または変更してください。

## Social Media

SNSは、Release告知、更新情報、簡単な案内および公式導線の周知に使用します。

SNS上の投稿、Reply、MentionまたはDirect Messageは、正式なSupport受付経路ではありません。

Supportが必要な場合は、GitHub Issues、GitHubの非公開脆弱性報告機能、またはGeneSIS公式窓口を使用してください。

SNS上で個人情報、購入情報、認証情報または未修正のSecurity問題を送信しないでください。

## Support Scope

Founder参加、BOOSTまたはその他の任意支援には、原則として次の個別対応は含まれません。

* 個別PCへの導入代行
* Remote操作による設定
* OllamaやLLMモデルの導入代行
* 個別Personaの作成
* 対話履歴の変換または整理代行
* 個別環境へのカスタマイズ
* 継続的な個別Consulting
* 外部製品自体のSupport

詳細は、[G.E.N.E / GeneSIS 共通Support Policy](./SUPPORT_POLICY.md)に従います。

## Response and Resolution

GeneSISは、受け付けた内容を確認し、必要に応じて調査および対応方針を検討します。

ただし、次の事項を保証するものではありません。

* すべての問い合わせへの返信
* 一定期間内の返信
* 個別対応
* 問題の修正
* 要望の採用または実装
* 対応期限
* 特定の結果
* 利用者データの復旧

受付順と対応順は一致しない場合があります。

技術的不具合の評価、対応順位および修正方針は、主として次の要素を考慮して判断します。

* 再現性
* 影響範囲
* 重大性
* 安全性
* データ消失または破損の可能性
* 利用者への影響
* 技術的実現性
* 製品思想との整合
* 開発状況

支援額、Founder参加の有無または購入回数によって、技術的評価、問い合わせ対応順位、修正順位または基本的な応対方針を変更しません。

## Current Status

G.E.N.E Alpha v1.0は現在、一般公開準備中です。

GitHub Issues、非公開脆弱性報告機能、関連URLおよびSupport Policyの正式な運用状態は、一般公開時までに更新します。

---
Copyright © 2026 GeneSIS: Concept Engineer's HQ. All rights reserved.
