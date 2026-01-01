# Russian Translit Plugin for Obsidian

Real-time English to Russian transliteration plugin for Obsidian.

## Features

- **F2 Toggle**: Press F2 to activate/deactivate translit mode
- **Real-time Conversion**: As you type English letters, they convert to Cyrillic instantly
- **Visual Indicator**: Status bar shows "🇷🇺 TRANSLIT" when active
- **Smart Matching**: Handles multi-character combinations (shch→щ, zh→ж, etc.)
- **Case Sensitive**: Supports both lowercase and uppercase letters

## Transliteration Map

### Multi-character combinations
- `shch` → `щ`
- `yo` → `ё`
- `zh` → `ж`
- `ts` → `ц`
- `ch` → `ч`
- `sh` → `ш`
- `yu` → `ю`
- `ya` → `я`
- `yi` → `ы`
- `je` → `э`
- `''` → `ъ`

### Single characters
- `a`→`а`, `b`→`б`, `v`→`в`, `g`→`г`, `d`→`д`, `e`→`е`
- `z`→`з`, `i`→`и`, `y`→`й`, `k`→`к`, `l`→`л`, `m`→`м`
- `n`→`н`, `o`→`о`, `p`→`п`, `r`→`р`, `s`→`с`, `t`→`т`
- `u`→`у`, `f`→`ф`, `h`→`х`, `c`→`ц`, `'`→`ь`

All combinations also work with capital letters.

## Installation

### From Release (Manual)

1. Download `main.js` and `manifest.json` from the latest release
2. Create a folder `translit-plugin` in your vault's `.obsidian/plugins/` directory
3. Copy the downloaded files into this folder
4. Reload Obsidian
5. Enable the plugin in Settings → Community Plugins

### From Source

1. Clone this repository into your vault's plugins folder:
   ```bash
   cd /path/to/vault/.obsidian/plugins
   git clone https://github.com/yourusername/obsidian-translit-plugin.git translit-plugin
   cd translit-plugin
   ```

2. Install dependencies and build:
   ```bash
   npm install
   npm run build
   ```

3. Reload Obsidian and enable the plugin

## Usage

1. Open any note in Obsidian
2. Press **F2** to activate translit mode (you'll see "🇷🇺 TRANSLIT" in the status bar)
3. Start typing in English - it will convert to Russian automatically
4. Press **F2** again to deactivate and return to normal typing

### Examples

When translit mode is active:
- Type `privet` → `привет`
- Type `Moskva` → `Москва`
- Type `shchuka` → `щука`
- Type `borshch` → `борщ`

## Hotkeys

- **F2**: Toggle translit mode on/off

You can change this hotkey in Obsidian's Settings → Hotkeys → "Toggle Translit Mode"

## Development

```bash
# Install dependencies
npm install

# Build for production
npm run build

# Development mode (auto-rebuild on changes)
npm run dev
```

## License

MIT

## Support

If you encounter any issues or have suggestions, please open an issue on GitHub.