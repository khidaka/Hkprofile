# Karabiner-Elements Custom Rules

## 概要 / Overview

このリポジトリは、**MacBookのJIS配列（日本語配列）キーボード**を前提とした [Karabiner-Elements](https://karabiner-elements.pqrs.org/) 用カスタムキーマップ設定ファイル (`karabiner.json`) を共有するものです。  
主に macOS 上で、JIS配列特有の記号や親指位置の英数キーを活用し、分割・ミニマルキーボードでもホームポジションから手を離さず快適な操作ができるよう設計しています。

This repository provides a highly customized Karabiner-Elements profile based on the **JIS (Japanese) layout MacBook keyboard**.  
It enables home-row centered, thumb-Enter operation, and various ergonomic remaps for minimalist/split keyboards on macOS.

---

## 主な特徴 / Features

- **MacBookのJIS配列キーボード前提**  
  JIS独自の記号配置・英数キー（親指位置）を活かした設計

- **Caps Lock → 右Command**  
  Caps Lock キーを右Commandキーとして再割り当て

- **Enterキーを英数キー（親指位置）にリマップ**  
  標準のEnterキーは無効化し、  
  「英数（Eisu）」キーをEnterとして利用。  
  分割・小型キーボードでも「親指Enter」運用が可能

- **右Shift+nm,jkliop → 123456789**  
  右Shift＋ホームポジションで数字入力  
  （例：右Shift+nで「1」, 右Shift+mで「2」...）

- **Spacebarを押しっぱなしで右Shift化**  
  Spaceを単独で押すとSpace、他キーと同時なら右Shiftに

- **左Command+hjkl → 矢印キー**  
  Vimライクにコマンド＋hjklでカーソル移動

- **記号・演算子のホームポジション入力**  
  右Shift+asdf で括弧類,  
  右Shift+uhb:' で+-*/ などを直感的に配置

- **その他、使わないキーの無効化や特殊用途リマップ多数**  
  （例：物理の数字キーや矢印キーを完全に無効化し、ホームポジション起点入力に最適化）

---

## 使い方 / Usage

1. [Karabiner-Elements](https://karabiner-elements.pqrs.org/) をインストール
2. 本リポジトリの `karabiner.json` を  
   `~/.config/karabiner/karabiner.json` に上書き or  
   Karabinerの設定画面からインポート
3. キーボード配列は **JIS（日本語配列）** でご利用ください
4. 自作キーボード等で動作確認し、違和感があればjsonを直接編集

---

## 詳細なルール例 / Main Rules Overview

- **Caps Lock → 右Command**
- **英数キー（親指位置） → Enterキー**
- **（標準の）Enterキー → 無効化**
- **右Shift + [n m , j k l i o p] → [1 2 3 4 5 6 7 8 9]**
- **右Shift + a/s/d/f → 括弧/バックスラッシュ**
- **右Shift + u/h/b/':' → + - * =**
- **左Command + hjkl → 矢印キー**
- **Spaceバー：単押しはSpace、同時押しは右Shift**

詳しい全リストは `karabiner.json` 内の `"complex_modifications"` をご参照ください。

---

## 注意・Tips

- **MacBookのJIS配列（日本語配列）キーボードを前提**としています。  
  US配列や他メーカーのキーボードで使う場合、物理キー・記号配置が異なり、追加調整が必要です。
- 物理の数字キーや矢印キー等、一部キーが完全に無効化されています。  
  普通のキーボード利用には向きません。  
  自作やミニマリスト配列、分割型での利用が前提です。
- **親指位置の英数キーが「Enter」になる仕様**のため、物理キーボード側に英数キーが必要です。
- 必要に応じて個人環境に合わせて設定を微調整してください。

---

## ライセンス / License

MIT License (or specify your own if different)

---

## 参考・謝辞 / References & Acknowledgements

- [Karabiner-Elements公式ドキュメント](https://karabiner-elements.pqrs.org/docs/json/)
- この設定をベースに自分仕様へどんどんアレンジしてご利用ください

---

## 問い合わせ / Contact

質問やフィードバックは [Issues](https://github.com/khidaka/Hkprofile/issues) へどうぞ。

