# Security Policy

- **Document Version:** v0.4
- **Status:** Active
- **Published By:** GeneSIS
- **Operating Entity:** GeneSIS-Operator
- **Applicable To:** G.E.N.E Phase 1 / v1.x and this official Repository
- **Established:** 2026-07-31
- **Effective From:** 2026-07-31

> 本書の日本語版を原文および正本として管理します。英語版その他の翻訳版との間に解釈上の差異がある場合は、適用法令上許される範囲で日本語版を優先します。

本書は、未修正のSecurity問題を非公開で報告するための対象範囲、報告経路および基本方針を定めます。

## 1. 対象範囲

対象ごとの適用開始時点は次のとおりです。

| 対象 | 適用開始 |
|---|---|
| `GeneSIS-Public/G.E.N.E` Repository、掲載文書、Release情報および検証情報 | 本PolicyのEffective Fromから対象 |
| G.E.N.E Alpha v1.0 Applicationおよび公式配布Package | 2026-07-31から対象 |
| GeneSISが本Policyの対象として別途明示する成果物 | 個別に明示する時点から対象 |

次は原則として対象外です。

- 開発途中Build、内部運用版または未公開試験版
- 第三者が改変・再配布したPackage
- 非公式Patchまたは非公式Build
- G.E.N.Eと無関係なOS、Ollama、LLM、Modelその他の外部製品単体の問題
- Social Engineering、SpamまたはService妨害
- 違法行為、無断AccessまたはEULAに反する利用を前提とする問題

外部製品に由来する問題でも、G.E.N.Eとの連携によってSecurity上の影響が生じる場合は、参考情報として受け付けることがあります。

### Supported Versions

| Version | Security Support |
|---|---|
| G.E.N.E Alpha v1.0 | 対象 |
| 開発途中Build・内部運用版・未公開試験版 | 対象外 |

G.E.N.E Alpha v1.0 Application、公式配布Package、Repositoryおよび公開文書は、2026-07-31から本Policyの対象です。

## 2. 非公開報告

未修正のSecurity問題は、公開のGitHub Issue、Xを含むSNS、その他の公開場所へ詳細を投稿しないでください。

このRepositoryでGitHub Private Vulnerability Reportingが有効な場合は、その非公開報告経路を使用してください。

利用できない場合は、次のGeneSIS公式窓口へ連絡してください。

`genesis.official.poc@mail.com`

メール件名：

```text
[Security Report]
```

問題がSecurity上の懸念に該当するか明確な判断ができない場合も、公開せず非公開経路を使用してください。

## 3. 報告に含める情報

可能な範囲で、次を含めてください。

- 対象VersionまたはBuild
- Packageの取得元
- OS、Runtime、Model等の実行環境
- 問題の概要
- 確認日時
- 再現条件または再現手順
- 想定される影響
- 必要な権限または前提条件
- 公開可能な範囲へ整理したLogまたは画面情報
- 確認済みの回避方法
- 第三者へ既に公開しているか
- 希望する連絡方法

情報が不足している場合は、確認または再現ができないことがあります。

## 4. 送信しない情報

調査に不要な機微情報は送信しないでください。

- Password、Token、API Key、秘密鍵、認証Code
- 2段階認証CodeまたはBackup Code
- クレジットカード番号その他の決済情報
- 個人情報または第三者の非公開情報
- 私的な対話履歴、Persona情報または非公開資料
- 第三者Data
- 事前に依頼されていない実行形式のExploitまたはMalware

File Path、Logまたは画面情報に秘密情報が含まれる場合は、必要部分を伏せてください。

GeneSISがPassword、認証Code、Backup Code、秘密鍵または決済情報の提出を求めることはありません。

## 5. 検証・開示上の注意

Security確認を行う場合も、次を行わないでください。

- 自分に権限のないAccount、端末、FileまたはDataへのAccess
- Dataの改変、削除または破壊
- Service妨害または過度な負荷を与える試験
- Social Engineering
- 第三者への攻撃、追跡または情報収集
- 適用法令、EULAまたは第三者の権利に反する行為

利用者への危険を抑えるため、修正版または公式案内が公開されるまで、第三者が悪用できる詳細の公開を控えるよう協力を求めます。

本Policyは、違法なAccess、破壊的な試験、第三者Systemへの試験その他の行為を許可するものではありません。

## 6. 対応方針

GeneSISは、報告内容を確認し、必要に応じて調査、追加情報の依頼、回避案内、修正または公式告知を検討します。

判断では、主として次を考慮します。

- 再現性
- 影響範囲
- 重大性
- 利用者Dataへの危険
- 悪用可能性
- 修正可能性
- 現在の開発・運営状況

報告の受領は、返信、修正、対応期限、Security Advisoryの公開または特定の結果を保証するものではありません。

公開の要否および時期は、影響、悪用可能性、対応状況および適用法令を考慮してGeneSIS-Operatorが判断します。

本Policyは、秘密保持契約、報奨金制度または脆弱性報奨金Programを構成しません。

## 7. Security報告ではないもの

次は通常、Security報告ではありません。

- 一般的な操作方法の質問
- 機能追加の要望
- 表示上の軽微な問題
- 公開しても利用者への危険を生じさせない通常不具合
- AIまたはLLMの回答内容・品質
- 購入、利用条件、権利、PrivacyまたはFounder資格の問い合わせ

通常不具合と一般問い合わせは、[Contact and Support](./docs/CONTACT_AND_SUPPORT.md)をご確認ください。

---

Copyright © 2026 GeneSIS: Concept Engineer's HQ. All rights reserved.
