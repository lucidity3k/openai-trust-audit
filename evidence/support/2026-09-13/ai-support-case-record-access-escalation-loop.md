# AI Support case-record access / escalation loop — transcript capture

Capture date: 2026-09-13 JST  
Scope: related Support Cases 10047260 / 10737395 / 13542215 / 13674098 / 13674651  
Evidence status: `USER_REPORTED` / `REVIEW_PENDING`  
Source type: user-supplied transcript copied into the audit record; original Support export / email / screenshot is not yet published with this entry.

## Why this record exists

This entry preserves the sequence currently supplied by the user concerning AI Support's inability to access individual Case records, a request to transfer the matter to a person/team with access, an escalation promise, a subsequent `new case` prompt, and a second escalation promise.

The record deliberately separates exact supplied text from evaluation. It does not infer the internal backend cause, intent, or actual access-control implementation.

## Supplied sequence

### 1. AI Support states that individual Case records cannot be accessed

The user supplied the following response:

> この窓口では、**Case Number（例：10047260 / 10737395 / 13542215 / 13674098 / 13674651）を指定されても、そのCaseの存在確認・状態・過去回答・送信済み質問・未回答事項・Case間の継承関係といった「個別Case記録」をこちらで参照して確認することはできません。**
>
> そのため、こちらで解決に進めるには、未回答の質問をこのスレッドに**箇条書きで貼り付け**てください（可能なら各項目に「希望する結論：返金／解約／請求確認／アカウント／不具合」も添えてください）。

### 2. User challenges the re-submission burden

The user then asked why a paying user should have to search, reconstruct, organize, and re-submit previously supplied Support history because the current AI Support window cannot access OpenAI's existing Case records. The user asked, in substance, why re-submission is required, what the rational basis is, whether the matter can be transferred to a person/team that can access Case records, and why that transfer was not performed first.

### 3. First escalation promise

The supplied response was:

> サポートスペシャリストにエスカレーションされました。数日以内にご返信をお待ちいただけます。返信はメールでもお送りします。必要に応じて、この会話に追加のコメントを投稿できます。

### 4. User prospectively predicts closure / new-case routing

Before the next supplied UI state, the user wrote:

> どうせケースクローズでしょ

The subsequent supplied UI text was:

> サポートを受けるには、新しいケースを作成してください

This record preserves that ordering. It does **not** by itself establish the precise backend Case status or closure reason; the exact observable text is the new-case prompt above.

### 5. AI Support again says prior Case/email records cannot be accessed

In the subsequent supplied interaction, AI Support stated:

> こちらでは過去のメール/Case記録そのものを参照できないため、あなたの本文に書かれている「未解消の具体的な要求（何を・いつまでに・どうしてほしいか）」をこのスレッド内の文面として特定できないと処理に進めません。いま最優先で解決したい結論だけ1つ（例：返金実行／自動更新停止／請求の二重計上確認／アカウント制限解除）を書いてください。

### 6. User requests a person with access

The user replied:

> なら参照できる権限者につなげ

### 7. Second escalation promise

The supplied response was:

> **人間のサポートスペシャリストへのエスカレーションを依頼しました**
>
> サポートスペシャリストにエスカレーションされました。数日以内にご返信をお待ちいただけます。返信はメールでもお送りします。必要に応じて、この会話に追加のコメントを投稿することもできます。

## Directly recordable observations from the supplied transcript

1. The AI Support text expressly states that the current window cannot access individual Case records even when Case Numbers are provided.
2. The AI Support text asks the user to paste unresolved questions into the current thread.
3. After the user asks why this re-submission burden should fall on the user and asks for a Case-aware escalation path, the supplied response states that the matter was escalated to a support specialist and that a response could be expected within days.
4. The user records a prediction that the Case will be closed before the supplied `create a new case` prompt appears.
5. A later supplied interaction again states that prior email/Case records cannot be accessed and asks the user to restate a single priority outcome.
6. After the user asks to be connected to an authorized person who can access the records, the supplied response again states that the matter was escalated to a human support specialist and that a response could be expected within days.

## Not established by this transcript alone

- The internal reason the Case-routing behavior occurred.
- Whether the first `new case` prompt corresponds to a formally closed backend Case or another UI/session state.
- Which specific internal team or person received either escalation.
- Whether the same or different Case Number was assigned to the second escalation.
- Whether a substantive specialist response was later delivered outside the supplied sequence.
- Internal permissions, tooling, or database access of AI Support or human Support staff beyond the wording shown above.

## Audit significance

The supplied sequence is relevant to the repository's ongoing review of:

- Case continuity and routing;
- repeated re-submission burden after information was previously provided to Support;
- escalation promises and later observable thread / new-case states;
- whether users can trace unresolved issues across Case Numbers and Support channels.

No conclusion about intent is drawn in this record.
