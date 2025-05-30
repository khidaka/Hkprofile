# Karabiner-Elements Configuration

## Overview
This repository contains a custom `karabiner.json` configuration file for [Karabiner-Elements](https://karabiner-elements.pqrs.org/), a powerful keyboard customization tool for macOS. The configuration includes key remappings and complex modifications to enhance efficiency and workflow.

## Features
### General Key Remappings
- `Caps Lock` → `Right Command`
- `Right Command` → `Japanese Kana` (Disabled by default)
- `Right Shift + Right Command` → `Japanese Eisuu` (Disabled by default)
- `Japanese Eisuu (英数)` → `Enter`
- `right_shift + Japanese Kana (かな)` → `Japanese Eisuu (英数)`
- `Close Bracket ( ] )` → `Shift + 8` ( * )
- `Backslash ( \ )` → `Shift + 9` ( ( )
- `Spacebar` → `Right Shift` (acts as space when pressed alone)

### Application Switching
- When an application is activated, the input mode automatically switches to EISUU (英数).
- After switching applications, releasing the left_command key also sends EISUU (英数), ensuring the input mode is always reset to alphanumeric.

### Numeric Key Remappings (with Right Shift)
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
- `0` → `-`

### Additional Remappings
- `Shift + Delete/Backspace` → `*`
- `Shift + Enter` → `+` (Disabled by default)
- `Shift + 8` → `[` (Open Bracket)
- `Shift + 9` → `]` (Close Bracket)
- `Left Command + H/J/K/L` → Arrow keys (Left, Down, Up, Right)

## Installation
1. Install [Karabiner-Elements](https://karabiner-elements.pqrs.org/).
2. Clone this repository:
   ```sh
   git clone https://github.com/khidaka/Hkprofile.git
   ```
3. Copy the `karabiner.json` file to your Karabiner configuration folder:
   ```sh
   cp karabiner.json ~/.config/karabiner/
   ```
4. Open Karabiner-Elements and select the profile "Hk profile."

## Customization
You can modify `karabiner.json` to adjust key mappings according to your needs. Use the Karabiner-Elements "Complex Modifications" tab to enable or disable specific mappings.

## License
This configuration is open-source and available for customization. Feel free to modify and adapt it to your workflow.

