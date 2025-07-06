# 0016. 不要なjapanese_eisuuイベントの削除

## Status

Accepted

## Context

エンターキーを無効化しているにも関わらず、イベントビューアーで`japanese_eisuu`イベントが発行されている問題が発生していた。

## Decision

以下の2つのルールを削除する：

1. **Switch to EISUU (英数) when application is activated**
   - アプリ切り替え時に自動で`japanese_eisuu`を送信するルール
   - 過去にアプリ切り替え時の最初のモードを`japanese_eisuu`にしたかった名残だが、現在は使用していない

2. **Send EISUU when left_command is released after app switching**
   - left_commandキーを離した時に`japanese_eisuu`を送信するルール
   - アプリ切り替え後の自動EISUU切り替え機能だが、現在は不要

## Consequences

### Positive
- 意図しない`japanese_eisuu`イベントが発生しなくなる
- エンターキーの無効化が正しく機能する
- 設定がよりシンプルになる

### Negative
- アプリ切り替え時の自動EISUU切り替え機能が失われる
- ただし、この機能は現在使用していないため実質的な影響なし

## Notes

残したルール：
- **right_shift + japanese_kana to japanese_eisuu**: 意図的に使用しているため保持 