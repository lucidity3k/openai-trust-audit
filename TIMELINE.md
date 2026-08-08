# Timeline / 時系列索引

最終更新: 2026-08-08 JST  
状態: Bootstrap timeline

## 記録規則

- 日時は原資料の表示とタイムゾーンを保存する。
- 日付のみ確認できる場合、時刻を補完しない。
- private索引由来の候補イベントは`REVIEW_PENDING`とする。
- 利用者報告は`USER_REPORT`とする。
- 公式ページ上の出来事とSupport Case上の出来事を区別する。

## 日付を確認できるイベント

| Date | Timezone | Case / Scope | Actor | Event | Classification | Public source status |
|---|---|---|---|---|---|---|
| 2025-10-28 | 公式ページ記載 | OpenAI structure | OpenAI | 更新されたstructureを発表。OpenAI FoundationとOpenAI Group PBCを公式ページに記載 | `OFFICIAL_SOURCE` | [Our structure](https://openai.com/our-structure/)。snapshot未保存 |
| 2026-01-01 | 公式ページ記載 | Terms of Use | OpenAI | 現行Terms of UseのPublished / Effective date。個人向けServicesの契約相手としてOpenAI OpCo, LLCを記載 | `OFFICIAL_SOURCE` | [Terms of Use](https://openai.com/policies/terms-of-use/)。snapshot未保存 |
| 2026-05-24 | 未確認 | Agent Mode連続Case | 利用者 / OpenAI Support | private取込み索引はSupport Case系列の開始日として記録 | `REVIEW_PENDING` | 公開原資料なし |
| 2026-05-29 | 未確認 | 09330474 | OpenAI Support表示 | private索引はSupport Specialistへのエスカレーションと数日以内の返信表示を記録 | `REVIEW_PENDING` | 公開原資料なし |
| 2026-06-10 | 未確認 | 09899636 | OpenAI Support表示 | private索引はSupport Specialistへのエスカレーションと数日以内の返信見込み表示を記録 | `REVIEW_PENDING` | 公開原資料なし |
| 2026-06-30 | 未確認 | 10737880 | OpenAI Support表示 | private索引はSupport Specialistへのエスカレーションと今後数日以内の返信見込み表示を記録 | `REVIEW_PENDING` | 公開原資料なし |
| 2026-07-15 | private取込み記録 | Agent Mode連続Case | 利用者側資料 | 158ページと記録されたSupport correspondence PDFの取込みノートをprivate資料側で作成。PDF binary、SHA-256、公開用redactionは未完了と同ノートに明記 | `PRIVATE_VERIFIED` / 公開証拠未収録 | public原資料なし |
| 2026-08-08 | Asia/Tokyo | public repository | lucidity3k/openai-trust-audit | 方法論、出典方針、Case索引、人物・組織索引、時系列骨格をDraft PR化 | `OBSERVATION` | 本PR |

## 日時未確定のレビュー対象

| Scope | Candidate sequence | Classification | Missing fields |
|---|---|---|---|
| 10737880 | エスカレーション表示後、利用者が中核質問を返信。その後、実質回答・解決・理由説明・事前通知なしでCase終了状態になったとの報告 | `USER_REPORT` | 後続全返信、終了日時、通知、理由、保存画面 |
| 10849106 | inpainting / mask問題への実質回答がないまま返信不能の終了状態になったとの記録候補 | `REVIEW_PENDING` | 原文、日時、回答、終了画面 |
| 12115787 | outage説明、根拠確認、general referenceへの説明変更、訂正要求、最終Yes/No、無回答・Case終了との報告 | `USER_REPORT` | 全日時、原文、actor、訂正、終了表示 |
| 複数関連Case | 証拠保全通知等を含む通知に対して、AI assistantがデータexportおよび削除関連Help Center記事を案内したとの報告 | `USER_REPORT` / `REVIEW_PENDING` | Case番号、各日時、原文、スクリーンショット、記事URL |
| 複数関連Case | 回答予告後に実質回答がないままCaseが終了したとの反復報告 | `USER_REPORT` / `REVIEW_PENDING` | Caseごとの予告者、予告日時、回答、終了日時、通知、理由 |

## 次の時系列作業

1. Support PDFの原本・公開用コピーを分離する。
2. 各Caseの全メッセージを日時順に抽出する。
3. エスカレーション、回答予告、利用者返信、正式訂正要求、最終質問、最後のOpenAI回答、終了確認を別イベントにする。
4. Support UI、メール、Case summary、Feedback表示を別ソースとして記録する。
5. 日時・actor・Case番号が確認できない欄は「記録上確認できず」とする。
6. OpenAI公式ページとFTC公式文書は取得日時点のsnapshotを保存する。

## English summary

The bootstrap timeline separates dated official-source events, private-index candidates, and undated user reports. Missing timestamps and actor identities are not inferred. Case-level chronology will be promoted only after raw-source and redaction review.

