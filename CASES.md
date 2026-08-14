# Cases / Support Case索引

最終更新: 2026-08-13 JST  
状態: Bootstrap index + first public Support evidence

## 読み方

この索引は調査対象を固定するためのものです。Case番号、主題、候補イベントを掲載しても、原資料の公開確認前はCase上の事実認定を完了したことになりません。

- `PUBLIC_VERIFIED`: この公開リポジトリ内の原資料から直接確認済み
- `REVIEW_PENDING`: private索引、利用者提供情報、候補資料等があるが、公開用原資料との照合前
- `USER_REPORTED`: 利用者の報告として記録。公開証拠による観測へ置換しない
- `UNCONFIRMED`: 現時点の資料で確認できない

## Case一覧

### Case 09185540

- **Current subject:** Agent Mode・有料アクセスに関する連続Caseの一部
- **Evidence status:** `REVIEW_PENDING`
- **Public evidence:** なし
- **Current public claim:** Case番号と連続Case候補であることだけを索引化。個別イベントは未公開
- **Open questions:** 開始日時、担当表示、質問、回答、終了状態、他Caseとの正確な継承関係

### Case 09330474

- **Current subject:** Agent Mode・Support Specialistへのエスカレーション表示
- **Evidence status:** `REVIEW_PENDING`
- **Candidate event:** private索引は2026-05-29のエスカレーション・数日以内の返信表示を記録。原資料の公開照合前
- **Public evidence:** なし
- **Open questions:** 原文、表示主体、後続返信、回答内容、Case終了状態

### Case 09899636

- **Current subject:** Agent Mode・Support Specialistへのエスカレーション表示
- **Evidence status:** `REVIEW_PENDING`
- **Candidate event:** private索引は2026-06-10のエスカレーション・数日以内の返信見込み表示を記録。原資料の公開照合前
- **Public evidence:** なし
- **Open questions:** 原文、表示主体、後続返信、回答内容、Case終了状態

### Case 10047260

- **Current subject:** refund request。公開済みCase 10737395のAira返信内で、Case 10047260のrefund requestのreviewを続けると明示されている
- **Evidence status:** 上記のCase間参照は`PUBLIC_VERIFIED`。返金申立ての全経過・主要争点・過去提出資料は`REVIEW_PENDING` / `USER_REPORTED`
- **Public evidence:** [Case 10737395 evidence record](evidence/support/2026-08-13/case-10737395-closure-warning-refund-followup.md)
- **Direct observation:** 2026-08-13 06:22、Aira / OpenAI SupportはCase 10737395と表示された返信で、Case 10047260のrefund requestのreview継続を明記
- **Open questions:** Case 10047260の原スレッド、返金申立て全文、保存済み記録確認の有無、事実確認、最終返金判断、10737395とのrouting関係

### Case 10546615

- **Current subject:** Agent Modeの利用枠、返金または救済経路に関する連続Caseの一部
- **Evidence status:** `REVIEW_PENDING`
- **Public evidence:** なし
- **Current public claim:** Case番号と連続Case候補であることだけを索引化
- **Open questions:** 個別イベント、他Caseとの関係、最終回答、終了状態

### Case 10730658

- **Current subject:** `UNCONFIRMED`
- **Evidence status:** `UNCONFIRMED`
- **Public evidence:** なし
- **Current public claim:** 調査対象Case番号として登録
- **Open questions:** 主題、日時、actor、他Caseとの関係、回答・終了状態のすべて

### Case 10737395

- **Current subject:** closure warningと、Case 10047260のrefund reviewを継続すると明記したAira / OpenAI Support返信
- **Evidence status:** `PUBLIC_VERIFIED` for the published events
- **Public evidence:** [Case file](cases/10737395/README.md) / [Evidence record](evidence/support/2026-08-13/case-10737395-closure-warning-refund-followup.md) / [public-redacted PDF](evidence/support/2026-08-13/case-10737395-closure-warning-refund-followup.public-redacted.pdf)
- **Directly documented sequence:** 2026-08-12 07:04 closure warning → 08:59 user reply `は?` → 2026-08-13 06:22 Aira / OpenAI Support reply labeled Case 10737395
- **Direct observation:** Aira返信はCase 10047260のrefund requestのreviewを続けるためGoogle Play Order IDを要求し、既に提供されたconcerns / supporting informationは再送不要と明記
- **User report / review pending:** Google Play Order ID一覧自体も以前に提出済みだったとの利用者報告。今回の公開PDF単独では未確認
- **Open questions:** 10737395と10047260のrouting理由、Order IDの過去提出原資料、refund outcome、Caseの最終終了状態

### Case 10737880

- **Current subject:** Agent Modeの利用回数制限、計上基準、内部記録確認可否、エスカレーション後の経過
- **Evidence status:** `REVIEW_PENDING` / 終了状態は現段階で`USER_REPORTED`
- **Candidate event:** private索引は2026-06-30のSupport Specialistへのエスカレーションと、今後数日以内の返信見込み表示を記録。原資料の公開照合前
- **User report:** Specialistによる中核質問への回答、解決、理由説明、事前の終了通知が確認できないままCaseが終了状態になったとの報告
- **Public evidence:** なし
- **Open questions:** 原文、後続全返信、正式な終了日時、終了通知、終了理由、終了主体

### Case 10849106

- **Current subject:** 画像編集でinpainting / mask指定を利用できない問題
- **Evidence status:** `REVIEW_PENDING`
- **Candidate event:** private分析・ドラフトにCase番号と主題の記載がある。原資料の公開照合前
- **Public evidence:** なし
- **Open questions:** 問い合わせ原文、回答、機能仕様または不具合判定、終了状態、終了理由

### Case 12115787

- **Current subject:** outage説明、根拠確認要求、説明変更、正式訂正要求、最終Yes/No質問、無回答・Case終了との利用者報告
- **Evidence status:** `USER_REPORTED` / `REVIEW_PENDING`
- **User-reported sequence:**
  1. Support担当者が、問い合わせ時にplatform outageがありerror rateが高かった可能性と、問題をaddressedした旨を事実形式で説明
  2. 利用者がStatus Incident、URL、開始・終了時刻、発生時間との重複、内部記録確認の有無を質問
  3. 後続説明が、特定Incidentやspecific internal operational recordを確認した説明ではなくgeneral referenceだったという趣旨へ変更
  4. 利用者が正式訂正を要求
  5. case-specific internal record、request-ID correlation、specific public incidentを確認していなかったとの理解が正しいか、Yes/Noで質問
  6. 最終質問への回答がないままCase要約・Feedback表示へ移行したとの報告
- **Public evidence:** なし
- **Open questions:** 全イベントの正確な日時、原文、担当者表示、訂正の有無、最後のOpenAI回答、終了日時、終了通知・終了理由

## 番号不明・消失・メールのみのCase

Case Numberが表示されていない関連問い合わせには番号を推測で付与しません。次の形式で一時IDを付けます。

```text
UNNUMBERED-YYYYMMDD-NN
```

このIDはGitHub上の整理用であり、OpenAIのCase Numberではありません。履歴から消失したCase、Support UIでは表示されないがメールに残るCaseも、各アクセス経路と確認日時を分けて記録します。

## Case公開時の必須項目

- Case Number
- 対象期間とタイムゾーン
- 表示上のactor
- 利用者の質問
- 実際の回答
- 回答予告・エスカレーション
- 訂正要求と応答
- 最終質問と後続回答の有無
- Case終了日時、通知、理由、返信欄、履歴表示
- 公開証拠、SHA-256、redaction状態
- 未確認事項

## English summary

The case list is a controlled research index, not a finding ledger. Case 10737395 is the first entry backed by a public-redacted Support PDF in this repository. That evidence directly shows a closure warning, a user reply, and an Aira / OpenAI Support response labeled Case 10737395 that explicitly says it is continuing review of a refund request for Case 10047260. Whether the requested Google Play Order ID had already been submitted is not established by this PDF alone.
