# Source Policy / 出典・公開方針

最終更新: 2026-08-08 JST  
状態: Bootstrap draft

## 1. 優先順位

1. 改変されていない原資料
2. 原資料から作成し、検証済みの公開用redacted copy
3. OpenAI、FTC、米国政府等の公式ページ・公式文書
4. 原資料に対応付けられた時系列・索引
5. 利用者報告
6. 第三者資料
7. 推論・評価

順位は「公式資料が常に事実として優越する」という意味ではありません。公式表示と実際のCase記録が衝突する場合は、双方を保存し、衝突をそのまま記録します。

## 2. private資料の扱い

privateリポジトリ、メール、Library上のファイル、Support UI、決済画面、端末上の記録は、公開許可が包括的にあるとはみなしません。候補資料を1件ずつ確認します。

private資料のファイル名や索引が存在しても、それだけで内容を公開済みまたは立証済みとは扱いません。privateリポジトリ全体をpublicへ複製しません。private URL、内部ブランチ、秘密トークン、認証情報を公開文書へ記載しません。

## 3. 原本保全

`evidence/`の原本は不変です。

- 上書き、再圧縮、OCR置換、翻訳上書き、ページ抽出による代替をしない
- 改訂版、再取得版、翻訳、OCR、公開用コピーは別ファイルにする
- 元ファイル名、バイト数、ページ数、SHA-256、取得日時、取得方法を記録する
- 原本をfindingsや文字起こしで置き換えない

## 4. 公開前に確認する情報

利用者本人について、次を確認し、原則として公開用コピーから除去します。

- メールアドレス、電話番号、住所
- 注文番号、決済情報、カード・銀行情報
- IP、Cookie、セッション、認証情報、API key、秘密トークン
- アカウント固有URL、不要な端末識別情報
- 本件の検証に不要な第三者情報

redactionは、例えば`[REDACTED: USER EMAIL]`のように種類を示します。単なる黒塗り画像だけでなく、PDFのテキスト層、埋込みオブジェクト、注釈、メタデータから復元できないことを検証します。

## 5. Support担当者名

Supportメール、Support画面、Case履歴などの原資料に業務上の氏名が表示されている場合、次を対応付けたうえで原資料どおり記録できます。

- 氏名
- 表示上の所属
- Case Number
- 日時
- 実際の回答内容
- 公開証拠

原資料にない肩書、権限、雇用関係、社内役割、承認責任、意思決定責任は追加しません。私生活、住所、私用連絡先、家族、非公開SNS等は収集・公開しません。

Bootstrap段階では、公開前レビューを完了したSupport担当者名はありません。

## 6. 経営・ガバナンス関係者

経営陣・理事等は、取得日時点のOpenAI公式ページが示す氏名と役職だけを記録します。個別Support Caseを承認・認識・処理したとは、直接証拠がない限り記載しません。

## 7. 公式資料レジスター（初期）

以下は2026-08-08 JSTに実表示または公式検索結果を確認した取得候補です。PDF・スクリーンショットの保存とSHA-256登録は未実施です。

### OpenAI

- [Terms of Use](https://openai.com/policies/terms-of-use/) — Published / Effective: 2026-01-01
- [Our structure](https://openai.com/our-structure/) — updated structure announced 2025-10-28
- [About](https://openai.com/about/)
- [OpenAI Charter](https://openai.com/charter/)

### FTC・米国政府

- [Federal Trade Commission Act](https://www.ftc.gov/legal-library/browse/statutes/federal-trade-commission-act)
- [15 U.S.C. § 45](https://uscode.house.gov/view.xhtml?req=%28title%3A15+section%3A45+edition%3Aprelim%29)
- [FTC Policy Statement on Deception](https://www.ftc.gov/legal-library/browse/ftc-policy-statement-deception)
- [FTC Policy Statement on Unfairness](https://www.ftc.gov/legal-library/browse/ftc-policy-statement-unfairness)
- [FTC Policy Statement Regarding Advertising Substantiation](https://www.ftc.gov/legal-library/browse/ftc-policy-statement-regarding-advertising-substantiation)
- [Bringing Dark Patterns to Light](https://www.ftc.gov/reports/bringing-dark-patterns-light)
- [Negative Option Rule](https://www.ftc.gov/legal-library/browse/rules/negative-option-rule) — 変更履歴と現行状態を使用時に再確認する
- [FTC Action Against Vonage](https://www.ftc.gov/news-events/news/press-releases/2022/11/ftc-action-against-vonage-results-100-million-customers-trapped-illegal-dark-patterns-junk-fees-when-trying-cancel-service)
- [FTC v. Vonage Complaint (PDF)](https://www.ftc.gov/system/files/ftc_gov/pdf/Vonage-Complaint.pdf)
- [Vonage Stipulated Final Order (PDF)](https://www.ftc.gov/system/files/ftc_gov/pdf/Vonage-Stipulated-Final-Order.pdf)

## 8. 公式資料の区別

次を同一の法的重みとして扱いません。

- Statute / U.S. Code
- FTC Policy Statement
- Rule / Federal Register notice
- Complaint / 申立て
- Final Order / 判決・合意命令
- Press Release
- Business Guidance / Staff Report

タイトル、発行主体、日付、文書種別、該当ページを記録します。Press ReleaseだけでComplaintやOrderの内容を代替しません。

## 9. 引用・翻訳

引用は必要最小限にし、原文、引用位置、出典へリンクします。省略記号で意味を変えません。日本語訳は原文と分け、翻訳であることを明示します。翻訳を原資料へ上書きしません。

## 10. 公開可否の判断表

| 資料 | 初期判断 | 公開条件 |
|---|---|---|
| Supportメール／UI原本 | レビュー必須 | 権利、完全性、個人情報、Case対応付けを確認 |
| 利用者メール・決済資料 | 原則private | 必要性があり、強いredactionと再検証が完了した場合のみ |
| OpenAI公式ページ | 公開候補 | URL、取得日時、版、ハッシュを記録 |
| FTC・政府公式資料 | 公開候補 | 文書種別、日付、該当箇所を記録 |
| Support担当者の業務上の署名氏名 | 条件付き公開 | Case、日時、回答、原資料を対応付ける |
| 私生活・私用連絡先 | 公開禁止 | 本件との関係を問わず収集しない |
| private CloseAIの分析文書 | レビュー必須 | 原資料との対応、分類、公開リスクを再確認 |
| 利用者報告 | 条件付き公開 | `USER_REPORT`と明示し、観測事実に置換しない |

## 11. 公開前チェック

- [ ] 原本を改変していない
- [ ] SHA-256、サイズ、取得日時、タイムゾーンがある
- [ ] Case Numberと日時を推測していない
- [ ] 個人情報、決済、認証、端末情報を確認した
- [ ] redactionが復元不能である
- [ ] 担当者名を実際の回答と対応付けた
- [ ] 引用が原文と一致する
- [ ] 観測、報告、推論、評価、未確認、公式資料を分けた
- [ ] private資料を丸ごと公開していない

## English summary

Private materials are reviewed item by item. Original evidence is immutable; redacted public copies are separate and must be tested for irreversible redaction. Business names shown in support evidence may be published only with a case, timestamp, response, and source linkage. Private contact and account data are excluded.

