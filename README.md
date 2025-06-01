# Hkprofile

## Overview
This repository contains a custom `karabiner.json` configuration file for [Karabiner-Elements](https://karabiner-elements.pqrs.org/), a powerful keyboard customization tool for macOS. The configuration is designed to enhance typing efficiency and maintain home position ergonomics.

## Features

### Basic Key Remappings
- `Caps Lock` → `Right Command`
- `Spacebar` → `Right Shift` (acts as space when pressed alone)
- `Japanese Eisuu (英数)` → `Enter`
- `Enter` → Disabled
- `Right Command` → `Delete/Backspace`
- `Right Shift` → Disabled

### Japanese Input Mode Management
- `Right Command` → `Japanese Kana` (Disabled by default)
- `Right Shift + Right Command` → `Japanese Eisuu` (Disabled by default)
- `right_shift + Japanese Kana (かな)` → `Japanese Eisuu (英数)`
- Automatic EISUU (英数) mode when:
  - Application is activated
  - Left Command is released after app switching

### Numeric Input (with Right Shift)
- `Right Shift + B` → `1`
- `Right Shift + N` → `2`
- `Right Shift + M` → `3`
- `Right Shift + H` → `4`
- `Right Shift + J` → `5`
- `Right Shift + K` → `6`
- `Right Shift + U` → `7`
- `Right Shift + I` → `8`
- `Right Shift + O` → `9`
- `Right Shift + 0` → `0`
- `0` → `-` (replaces original hyphen key)
  - *Note: Original number keys 1-9 and hyphen key are disabled to maintain home position ergonomics*

### Symbol Input (with Right Shift)
- `Right Shift + Q` → `!`
- `Right Shift + P` → `=`
  - *Note: Original Shift + 1 for ! and Shift + - for = are disabled to prevent accidental inputs*

### Bracket and Special Character Remappings
- `Close Bracket ( ] )` → `Shift + 8` ( * )
- `Backslash ( \ )` → `Shift + 9` ( ( )
- `Shift + Delete/Backspace` → `*`
- `Shift + Enter` → `+` (Disabled by default)
- `Shift + 8` → `[` (Open Bracket)
- `Shift + 9` → `]` (Close Bracket)

### Navigation
- `Left Command + H/J/K/L` → Arrow keys (Left, Down, Up, Right)
  - *Note: Uses Left Command for better home position ergonomics*

## Installation
1. Install [Karabiner-Elements](https://karabiner-elements.pqrs.org/)
2. Clone this repository:
   ```sh
   git clone https://github.com/khidaka/Hkprofile.git
   ```
3. Copy the `karabiner.json` file to your Karabiner configuration folder:
   ```sh
   cp karabiner.json ~/.config/karabiner/
   ```
4. Open Karabiner-Elements and select the profile "Hk profile"

## Customization
You can modify `karabiner.json` to adjust key mappings according to your needs. Use the Karabiner-Elements "Complex Modifications" tab to enable or disable specific mappings.

## Development Environment
- macOS
- Karabiner-Elements

## License
MIT

