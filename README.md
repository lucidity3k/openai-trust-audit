# OpenAI Trust — Public Evidence & Support Audit

> Independent public evidence and accountability archive concerning OpenAI products, support practices, representations, and documented user experiences. Not affiliated with or endorsed by OpenAI.

OpenAI、OpenAIの契約主体・関連組織、OpenAI Support、AI-assisted Support、ChatGPTについて、有料サービスの表示、実際の利用状態、Support Caseの経過、公式説明、訂正要求、回答・無回答・Case終了、および後日の表示変更を、原資料と時系列に基づいて保存・照合する独立した利用者側監査リポジトリです。

これはOpenAIの公式リポジトリではありません。OpenAIから承認・後援を受けたものでもありません。

## 現在の公開状態

**Bootstrap + first public Support evidence（2026-08-13 JST）**

監査方法、出典方針、Case索引、時系列、人物・組織の記録方法に加え、Case 10737395に関する最初のpublic-redacted Support PDFとCase別索引を公開しています。生証拠は無差別に公開せず、個人情報・完全性・引用位置をレビューした資料だけを追加します。Case単位のFTC文書との要件照合はまだ公開していません。

| 状態 | 意味 |
|---|---|
| 公開済み | 公開前レビューを通過し、このリポジトリから参照できる資料 |
| レビュー中 | private原資料または利用者提供情報はあるが、完全性・個人情報・引用位置を確認中 |
| 未処理 | 対象として識別済みだが、原資料との対応付けを開始していない |

## 監査の基本単位

記述は次の6区分を混同しません。

1. **Observation / 観測事実** — 公開されたファイル、画面、ログ、返信、公式ページから直接確認できる内容
2. **User Report / 利用者報告** — 利用者が報告した内容。原資料の公開確認前は観測事実へ昇格させない
3. **Inference / 推論** — 複数の観測から導く説明候補
4. **Evaluation / 評価** — 観測、公式基準、推論に対する監査上の判断
5. **Unconfirmed / 未確認** — 内部ログ、担当権限、承認経路、意図など、証拠上確定していない内容
6. **Official Source / 公式資料** — OpenAI、FTC、米国政府等が公開した資料。公式であることと、個別Caseの実挙動が整合することは別に検証する

直接確認できた事実は「可能性」へ弱めません。一方、確認していない意図、心理、内部承認、役割、法的確定判断は事実として書きません。

詳細は [METHODOLOGY.md](METHODOLOGY.md) と [SOURCE_POLICY.md](SOURCE_POLICY.md) を参照してください。

## Case索引

以下は調査対象の索引です。Case番号の掲載だけで、当該Caseに関する主張が立証済みまたは公開済みであることを意味しません。

| Case Number | 現在の主題 | 公開状態 |
|---|---|---|
| 09185540 | Agent Mode・有料アクセスに関する連続Caseの一部 | レビュー中 |
| 09330474 | Agent Mode・Support Specialistへのエスカレーション表示 | レビュー中 |
| 09899636 | Agent Mode・Support Specialistへのエスカレーション表示 | レビュー中 |
| 10047260 | refund request。10737395の公開返信内で明示的に参照 | 一部公開確認済み / 全経過レビュー中 |
| 10546615 | Agent Mode・利用枠、返金または救済経路に関する連続Caseの一部 | レビュー中 |
| 10730658 | 主題と他Caseとの関係を原資料で確認中 | 未処理 |
| 10737395 | closure warning、Aira返信、Case 10047260のrefund reviewへの明示的参照 | [公開証拠あり](cases/10737395/README.md) |
| 10737880 | Agent Mode・利用枠・エスカレーション後の経過 | レビュー中 |
| 10849106 | 画像編集のinpainting / mask指定に関する問い合わせ | レビュー中 |
| 12115787 | outage説明、根拠確認要求、説明変更、訂正要求、最終質問への無回答・Case終了との利用者報告 | レビュー中 |

派生Case、Case Number不明の問い合わせ、履歴から消失したCase、メール側にのみ残るCaseは、番号を推測せず別区分で管理します。詳細は [CASES.md](CASES.md) を参照してください。

## 最初の公開Support証拠

Case 10737395について、利用者本人の表示氏名と個人メールアドレスをredactした公開用PDFを追加しています。Support側の業務上の表示、Case Number、日時、本文、Aira / OpenAI Support署名は証拠上重要なため保持しています。

- [Case 10737395](cases/10737395/README.md)
- [Evidence record](evidence/support/2026-08-13/case-10737395-closure-warning-refund-followup.md)
- [Public-redacted PDF](evidence/support/2026-08-13/case-10737395-closure-warning-refund-followup.public-redacted.pdf)

このPDFから直接確認できる範囲では、2026-08-12にclosure warningが送られ、利用者が返信し、2026-08-13にAira / OpenAI SupportがCase 10737395と表示された返信でCase 10047260のrefund requestのreviewを続けると明示しています。同返信はGoogle Play Order IDを要求すると同時に、既に提供されたconcerns / supporting informationは再送不要と記載しています。

利用者はOrder ID一覧自体もそれ以前に提出済みと報告していますが、この点は今回のPDF単独では確認できないため、対応する原資料が公開・検証されるまで`USER_REPORT` / `REVIEW_PENDING`として分離します。

## 主要な問題類型

現時点では次を**調査テーマ**として登録しています。結論ではありません。

- 有料プランの表示と実際の利用可能状態の差分
- 利用上限、解除時刻、残量、同時実行条件の表示
- Support Specialistへのエスカレーション表示と後続回答
- 回答予定後の実質回答、無回答、Case終了
- Support UIの履歴、返信欄、Caseアクセス経路の消失
- 説明変更と正式訂正要求への対応
- 証拠保全通知を含む問い合わせに対する削除関連Help Center案内
- Case番号間の継承・参照と、その説明の有無
- 既提出情報の再提出要求
- OpenAI公式表示とFTC公式文書の要素別照合

## 現行の公式情報アンカー

2026-08-08 JSTに公式ページの実表示を確認しました。これはURL確認であり、取得時点のPDFスナップショット保存は次回以降に行います。

- [OpenAI Terms of Use](https://openai.com/policies/terms-of-use/) — 2026-01-01発効版は、個人向けServicesの契約を利用者と **OpenAI OpCo, LLC** の間の契約として記載
- [OpenAI — Our structure](https://openai.com/our-structure/) — OpenAI Foundation、OpenAI Group PBC、Foundation Boardおよび使命に関する現行公式表示
- [FTC Act](https://www.ftc.gov/legal-library/browse/statutes/federal-trade-commission-act)
- [15 U.S.C. § 45](https://uscode.house.gov/view.xhtml?req=%28title%3A15+section%3A45+edition%3Aprelim%29)
- [FTC Policy Statement on Deception](https://www.ftc.gov/legal-library/browse/ftc-policy-statement-deception)
- [FTC Policy Statement on Unfairness](https://www.ftc.gov/legal-library/browse/ftc-policy-statement-unfairness)
- [FTC Policy Statement Regarding Advertising Substantiation](https://www.ftc.gov/legal-library/browse/ftc-policy-statement-regarding-advertising-substantiation)

公式資料は存在だけで実挙動を証明しません。Case証拠との照合は、記録、公式文言、一致要素、不一致・未確認要素、文書照合上の評価を分離して行います。

## 初期ディレクトリ

```text
cases/                 Case別の索引・分析
evidence/support/      Support原資料の公開用コピーとメタデータ
evidence/openai-official/
evidence/ftc-official/
findings/              複数資料を用いた監査所見
people/                人物別の証拠索引
timeline/              詳細時系列
official-snapshots/    公式ページの取得時点スナップショット
```

生証拠を無差別に投入しません。各ディレクトリは公開前レビューを通過した資料だけを受け入れます。

## 訂正受付方針

OpenAI、OpenAI OpCo, LLC、記録に登場する担当者その他の関係者が、具体的な事実誤認を指摘する場合は、対象Case、日時、対象記述、訂正内容、根拠資料を示してください。根拠を確認できた訂正は、変更履歴と理由を残して反映します。

事実訂正と削除要請は別に扱います。訂正によって過去の公開内容を痕跡なく消しません。専用の `CORRECTIONS_AND_NONRESPONSES.md` は次段階で作成します。

## 更新履歴

| 日付 (JST) | 更新 |
|---|---|
| 2026-08-08 | 公開監査の方法論、出典方針、Case索引、時系列骨格、人物・組織索引を初期作成。生証拠は未公開 |
| 2026-08-13 | Case 10737395の最初のpublic-redacted Support PDF、Aira索引、Case 10047260への明示的参照、時系列を追加 |

## English summary

This repository is an independent, user-side public audit archive. The bootstrap methodology and indexes are now accompanied by the first published Support evidence for Case 10737395. The redacted PDF directly documents a closure warning, a user reply, and an Aira / OpenAI Support response labeled Case 10737395 that explicitly says it is continuing review of the refund request for Case 10047260. The user's report that the Google Play Order ID list had already been submitted remains separate pending publication of the supporting source.
