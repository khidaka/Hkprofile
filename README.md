# Hkprofile

## 概要
このリポジトリは、macOS用の強力なキーボードカスタマイズツールである[Karabiner-Elements](https://karabiner-elements.pqrs.org/)の設定ファイル`karabiner.json`を含んでいます。この設定は、タイピング効率を向上させ、ホームポジションのエルゴノミクスを維持するように設計されています。

## 機能

### 基本キーリマップ
- `Caps Lock` → `Right Command`
- `Spacebar` → `Right Shift`（単独押しでスペース）
- `英数` → `Enter`
- `Enter` → 無効化
- `Right Command` → `Delete/Backspace`
- `Right Shift` → 無効化

### 日本語入力モード管理
- `Right Command` → `かな`（デフォルトで無効）
- `Right Shift + Right Command` → `英数`（デフォルトで無効）
- `Right Shift + かな` → `英数`

### 数字キー（右シフトと組み合わせ）
- `Right Shift + n` → `1`
- `Right Shift + m` → `2`
- `Right Shift + ,` → `3`
- `Right Shift + j` → `4`
- `Right Shift + k` → `5`
- `Right Shift + l` → `6`
- `Right Shift + i` → `7`
- `Right Shift + o` → `8`
- `Right Shift + p` → `9`
- `Right Shift + 0` → `0`
- `Right Shift + [` → `0`（7890を4本の指で連続して打つため）
- `0` → `-`（元のハイフンキーの代わり）
  - *注: ホームポジションのエルゴノミクスを維持するため、元の数字キー1-9とハイフンキーは無効化されています*

### 記号入力（右シフトと組み合わせ）
- `Right Shift + Q` → `!`
- `Right Shift + ;` → `:`
- `Right Shift + .` → `/`
  - *注: 以前は`Right Shift + ;`で`=`を入力していたが、現在はコロン(:)に変更し、競合を解消しました*

### 括弧と特殊文字のリマップ
- `]` → `Shift + 8`（*）
- `\` → `Shift + 9`（(）
- `Shift + Delete/Backspace` → `*`
- `Shift + Enter` → `+`（デフォルトで無効）
- `Shift + 8` → `[`
- `Shift + 9` → `]`

### ナビゲーション
- `Left Command + H/J/K/L` → 矢印キー（左/下/上/右）
  - *注: ホームポジションのエルゴノミクスを考慮してLeft Commandを使用*

## インストール方法
1. [Karabiner-Elements](https://karabiner-elements.pqrs.org/)をインストール
2. このリポジトリをクローン：
   ```sh
   git clone https://github.com/khidaka/Hkprofile.git
   ```
3. `karabiner.json`ファイルをKarabinerの設定フォルダにコピー：
   ```sh
   cp karabiner.json ~/.config/karabiner/
   ```
4. Karabiner-Elementsを開き、"Hk profile"を選択

## カスタマイズ
必要に応じて`karabiner.json`を編集して、キーマッピングを調整できます。Karabiner-Elementsの"Complex Modifications"タブを使用して、特定のマッピングを有効または無効にすることができます。

## 開発環境
- macOS
- Karabiner-Elements

## ライセンス
MIT

