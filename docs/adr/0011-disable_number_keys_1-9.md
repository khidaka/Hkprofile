# ADR 0011: 数字キー1〜9を無効化し、ホームポジションでの数字入力に一本化

## ステータス
採用済み

## コンテキスト
- ホームポジションを崩さずに数字を入力できるよう、右シフト＋ホームポジションキーで1〜9を入力できる設定を既に導入している。
- 習慣化のため、元の数字キー（1〜9）は押しても何も起きないようにしたい。

## 決定
- `complex_modifications`で数字キー1〜9を`vk_none`にマッピングし、無効化する設定を追加した。
- ホームポジションでの数字入力は引き続き可能。

## 結果
- 数字キー1〜9を押しても何も入力されなくなった。
- ホームポジションでの数字入力に完全に慣れることができる。
- ホームポジションを崩さずに数字入力が可能となり、効率が向上した。 