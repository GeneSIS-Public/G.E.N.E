# Contact and Support

- **Document Version:** v0.5
- **Status:** Active
- **Published By:** GeneSIS
- **Operating Entity:** GeneSIS-Operator
- **Applicable To:** GeneSIS / Project: Code-NOAH / G.E.N.E Phase 1 / v1.x
- **Established:** 2026-07-31
- **Effective From:** 2026-07-31
- **Updated:** 2026-09-01

> 本書の日本語版を原文および正本として管理します。英語版その他の翻訳版との間に解釈上の差異がある場合は、適用法令上許される範囲で日本語版を優先します。

本書は、GeneSISおよびG.E.N.Eに関する問い合わせ経路、Support範囲および基本的な対応方針を定めます。

## 1. 受付経路

| 内容 | 受付経路 |
|---|---|
| 記事の内容、読む順番、簡単な使い方に関する短い質問 | note — 簡易質問窓口 |
| 公開可能で再現性のある通常不具合 | GitHub Issues — Bug Report |
| 文書の誤り・不足 | GitHub Issues — Documentation Feedback |
| 開発上の提案・Feedback | GitHub Issues — Development Feedback |
| 購入、Founder照合、利用条件、権利、Privacy | GeneSIS公式窓口 |
| 公開に適さない不具合・その他の非公開連絡 | GeneSIS公式窓口 |
| 未修正のSecurity問題 | [Security Policy](../SECURITY.md)に記載する非公開経路 |

**GeneSIS公式窓口**

`genesis.official.poc@mail.com`

**簡易質問窓口（note）**

[GeneSIS_簡易窓口](https://note.com/genesis_protocol/n/n6a2a06ad2698)

簡易質問窓口は、記事の内容、読む順番、簡単な使い方に関する短い質問を、公開コメントで受け付けるための経路です。正式な不具合報告、非公開の問い合わせまたはSecurity報告には使用しないでください。

コメントは公開されます。個人情報、購入情報、認証情報、私的な対話履歴、未修正脆弱性の詳細その他の非公開情報を投稿しないでください。

簡易質問窓口を含め、すべての質問への返信または問題の解決を保証するものではありません。

Xを含むSNS上のReply、MentionまたはDirect Messageは、正式なSupport受付経路ではありません。

## 2. GitHub Issues

GitHub Issuesは公開領域です。通常不具合を報告する場合は、可能な範囲で次を記載してください。

- G.E.N.EのVersionまたはBuild
- OS、Runtime、Model等の実行環境
- 問題の概要
- 再現手順
- 期待した動作と実際の動作
- 再現頻度
- 公開可能なLogまたは画面情報
- 確認済みの回避方法

情報が不足している場合は、確認または再現ができないことがあります。

公開Issueへ次を投稿しないでください。

- 個人情報、購入情報、Founder照合情報
- Password、Token、API Key、秘密鍵、認証Code
- 私的な対話履歴、Persona情報、非公開資料
- 未修正脆弱性の再現・悪用に利用できる詳細
- 第三者へ公開すべきでないFile、Log、Pathまたは画面情報

認証情報を誤って公開した場合は、投稿の削除だけでなく、該当情報を速やかに無効化または変更してください。

## 3. 非公開の問い合わせ

GeneSIS公式窓口では、購入、Founder照合、利用条件、権利、Privacy、公開に適さない不具合その他の非公開連絡を受け付けます。

件名例：

```text
[Founder] Founder資格・購入記録の照合
[Rights] 利用条件・権利に関する問い合わせ
[Privacy] 個人情報に関する問い合わせ
[Private Bug] 非公開の不具合報告
[Other] その他の非公開連絡
```

Founder照合では、必要に応じてBOOTH注文番号、商品名、おおよその購入時期等を確認します。

GeneSISが、Password、2段階認証Code、Backup Code、クレジットカード番号その他の認証・決済情報を求めることはありません。

個人情報の取扱いと権利請求については、[Privacy Notice](./PRIVACY_NOTICE.md)をご確認ください。

## 4. Security報告

未修正のSecurity問題は、公開IssueまたはSNSへ投稿しないでください。

GitHubの非公開脆弱性報告機能が有効な場合はその経路を使用し、利用できない場合はGeneSIS公式窓口へ、件名`[Security Report]`で連絡してください。

対象範囲、報告内容および開示方針は、[Security Policy](../SECURITY.md)を優先します。

## 5. Support範囲

GeneSISは、状況に応じて次の対応を行うことがあります。

- 通常不具合と再現条件の確認
- Known Limitationsまたは回避方法の案内
- 文書の訂正・補足
- 修正版または更新版の検討
- 公式配布物と検証情報の確認
- 利用条件、権利またはFounder資格に関する案内

次の個別作業は、別途明示しない限りSupportに含みません。

- 個別PCへの導入またはRemote設定
- Ollama、Model、OS、Hardware等の外部製品自体のSupport
- Persona、Prompt、KnowledgeまたはReferenceの個別作成
- 対話履歴やDataの変換、整理または復旧代行
- 個別環境向けCustomization
- 継続的な個別Consulting
- Source Code、内部資料または未公開Buildの提供

G.E.N.Eは外部Runtime、Model、OSおよびHardwareと組み合わせて使用されます。外部製品単体の仕様、障害、提供終了または回答品質をGeneSISが管理・保証するものではありません。

## 6. 対応方針

対応の判断では、主として再現性、影響範囲、重大性、安全性、Data消失の可能性、技術的実現性および現在の開発状況を考慮します。

支援額、Founder参加、BOOSTまたは購入回数によって、技術評価、修正順位または基本的なSupport範囲を変更しません。

受付順と対応順は一致しない場合があります。

GeneSISは個人運営であるため、健康、生活、資金、技術的事情または外部Platformの変更等により、開発、公開、返信またはSupportを一時停止、縮小または終了する場合があります。

次を保証するものではありません。

- すべての問い合わせへの返信
- 一定期間内の返信
- 個別対応
- 問題の修正
- 要望の採用または実装
- 対応期限
- 利用者Dataの復旧
- 特定の結果

暴言、脅迫、嫌がらせ、Spam、虚偽情報、違法行為への協力要求または運営を著しく妨害する行為がある場合は、対応を制限または終了することがあります。正当な批判、不具合報告または異なる意見のみを理由に制限するものではありません。

## 7. 関連文書

- G.E.N.E本体の利用条件：正式配布Packageに付属するEULA
- Security報告：[Security Policy](../SECURITY.md)
- 個人情報：[Privacy Notice](./PRIVACY_NOTICE.md)
- Founder参加：[Founder Terms](./FOUNDER_TERMS.md)
- 対応環境・制約：[Known Limitations](./KNOWN_LIMITATIONS.md)

本書は、個別対応、返信、修正または一定期間内の対応を保証するService Level Agreementではありません。

---

Copyright © 2026 GeneSIS: Concept Engineer's HQ. All rights reserved.
