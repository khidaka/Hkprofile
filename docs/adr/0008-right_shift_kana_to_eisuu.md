# ADR 0008: right_shift + japanese_kanaでjapanese_eisuu、japanese_kana単独はそのまま

## ステータス
採用済み

## コンテキスト
- 日本語キーボードの「かな」キー（japanese_kana）は、通常そのまま使いたいが、右シフトと組み合わせて「英数」入力（japanese_eisuu）にも素早く切り替えたいニーズがあった。
- 以前はsimple_modificationsで「かな」キーを別のキーにリマップしていたが、柔軟性に欠けていた。

## 決定
- simple_modificationsから「japanese_kana → keyboard_fn」のリマップを削除。
- complex_modificationsで「right_shift + japanese_kana → japanese_eisuu」を追加。
- 「japanese_kana」単独はデフォルト動作（かな入力切替）とする。

## 結果
- かなキー単独はそのまま「かな」入力切替。
- 右シフト＋かなで「英数」入力切替が可能になり、入力効率が向上した。 