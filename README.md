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

### 四則演算（右シフトレイヤー）
- `Right Shift + u` → `+`（JIS配列: Shift+;）
- `Right Shift + h` → `-`
- `Right Shift + b` → `*`（JIS配列: Shift+2 など、実際はShift+quote）

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
- `Right Shift + [` → `0`

### 記号入力（右シフトと組み合わせ）
- `Right Shift + Q` → `!`
- `Right Shift + ;` → `:`
- `Right Shift + .` → `/`

### 括弧と特殊文字のリマップ
- `]` → `Shift + 8`（*）
- `\` → `Shift + 9`（(）
- `Right Shift + a/s/d/f` → 括弧・カッコ類
- `Shift + Delete/Backspace` → `*`
- `Shift + 8` → `[`（デフォルトで無効）
- `Shift + 9` → `]`（デフォルトで無効）

### ナビゲーション
- `Left Command + H/J/K/L` → 矢印キー（左/下/上/右）

### 無効化されているキー
- 数字キー `0-9`（単独押し）
- ハイフン（-）
- セミコロン（;）
- 矢印キー（上下左右）
- Enter/Return
- Delete/Backspace
- 右シフト
- 右コマンド

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

