# Security Policy

## Supported Versions

現在のSecurity Support対象は、次のとおりです。

| Version                | Security Support |
| ---------------------- | ---------------- |
| G.E.N.E Alpha v1.0     | 正式一般公開後に対象       |
| 開発途中Build・内部運用版・未公開試験版 | 対象外              |

G.E.N.E Alpha v1.0は現在、一般公開準備中です。

正式な製品Packageの一般公開開始後、本表を更新します。

原則として、Security SupportはGeneSISが公式配布対象として明示しているVersionに限ります。

## Reporting a Security Concern

Security上の懸念を発見した場合は、公開のGitHub Issue、SNSまたはその他の公開場所へ詳細を投稿しないでください。

可能な場合は、このRepositoryのGitHub Security画面にある非公開脆弱性報告機能を使用してください。

非公開脆弱性報告機能が利用できない場合は、次のGeneSIS公式窓口へご連絡ください。

**GeneSIS 公式窓口 - Official Contact**

`［genesis.official.poc@mail.com］`

メールで報告する場合は、件名の先頭に次の表記を付けてください。

```text
[Security Report]
```

次の情報を、公開Issue、SNSその他の公開場所へ掲載しないでください。

* 未修正の脆弱性を再現または悪用できる具体的な手順
* Access Token、Password、認証Codeまたは秘密鍵
* API Keyその他の認証情報
* 個人情報または第三者の非公開情報
* 不正アクセス、権限回避または情報取得につながる詳細
* 個人情報や秘密情報を含むFile、Log、Pathまたは画面情報
* 利用者への危険が生じる可能性のある未公開情報

## Information to Include

可能な範囲で、次の情報を含めてください。

* 対象となるG.E.N.EのVersionまたはBuild
* Packageの取得元
* 使用しているOSおよび実行環境
* 問題の概要
* 問題を確認した日時
* 再現条件または再現手順
* 想定される影響
* 問題が発生するために必要な権限や前提条件
* 関連するLogまたは画面情報
* 暫定的な回避方法
* 報告時点で第三者へ公開しているか
* 希望する連絡方法

Password、認証Code、秘密鍵、API Key、個人情報その他、調査に不要な機微情報は送信しないでください。

File Path、Logまたは画面情報に個人名、メールアドレス、Tokenその他の秘密情報が含まれる場合は、必要部分を伏せてください。

GeneSISから、Password、2段階認証Code、Backup Codeまたは秘密鍵の提出を求めることはありません。

事前の依頼なく、実行形式のExploit、Malwareまたは第三者のデータを送信しないでください。

## Responsible Disclosure

報告されたSecurity上の懸念について、GeneSISは内容を確認し、必要に応じて調査および対応方針を検討します。

利用者への危険を抑えるため、修正版または公式案内が公開されるまで、第三者が悪用できる詳細の公開を控えるようご協力ください。

GeneSISは可能な範囲で、報告の受領確認、追加情報の依頼および状況共有を行います。

ただし、報告の受領は、返信、修正、対応時期、Security Advisoryの公開または特定の結果を保証するものではありません。

公開の要否および時期は、影響範囲、再現性、利用者への危険性、対応状況および適用法令を考慮して判断します。

本Policyは、秘密保持契約、報奨金制度または脆弱性報奨金Programを構成するものではありません。

## Non-Security Issues

次の内容は、原則としてSecurity報告ではありません。

* 一般的な操作方法の質問
* 機能追加の要望
* 表示上の軽微な問題
* 公開しても利用者への危険を生じさせない通常の不具合
* AIまたはLLMの回答内容や品質
* 購入、利用条件、権利またはFounder資格に関する問い合わせ

公開可能で再現性のある通常の技術的不具合は、G.E.N.E公式RepositoryのGitHub Issuesを使用してください。

購入、利用条件、権利、Founder資格、個人情報およびその他の非公開連絡については、GeneSIS公式窓口へご連絡ください。

問題がSecurity上の懸念に該当するか判断できない場合は、公開Issueへ詳細を投稿せず、非公開経路を使用してください。

## Scope

本Security Policyは、次を対象とします。

* GeneSISの公式配布元から取得したG.E.N.E Alpha v1.0の正式Package
* `GeneSIS-Public/G.E.N.E` Repositoryに掲載された公式文書
* 同Repositoryに掲載されたRelease情報および検証情報
* GeneSISが本Policyの対象として別途明示したG.E.N.E関連成果物

原則として、次は対象外です。

* 開発途中Build
* 内部運用版
* 未公開試験版
* 第三者が改変または再配布したPackage
* 非公式Patchまたは非公式Build
* G.E.N.Eとは無関係なOS、LLM、Ollamaその他の外部製品単体の問題
* EULAまたは適用法令に反する利用を前提とする問題
* Social Engineering、Spamまたはサービス妨害を目的とする行為

外部製品に由来する問題でも、G.E.N.Eとの連携によってSecurity上の影響が生じる場合は、参考情報として受け付けることがあります。

G.E.N.EのSource Code、内部運用版、開発途中Build、未公開試験版および内部設計資料は、このRepositoryでは公開していません。

## Contact

**GeneSIS 公式窓口 - Official Contact**

`［genesis.official.poc@mail.com］`

件名：

```text
[Security Report]
```

すべての報告への返信および対応期限を保証するものではありません。

---

Copyright © 2026 GeneSIS: Concept Engineer's HQ. All rights reserved.
