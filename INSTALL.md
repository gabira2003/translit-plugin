# Quick Installation Guide

## Step 1: Locate Your Obsidian Vault Plugins Folder

Find your vault's plugins directory:
- **Windows**: `C:\Users\YourUsername\YourVault\.obsidian\plugins\`
- **Mac**: `/Users/YourUsername/YourVault/.obsidian/plugins/`
- **Linux**: `/home/yourusername/YourVault/.obsidian/plugins/`

If the `plugins` folder doesn't exist, create it.

## Step 2: Install the Plugin

1. Inside the `plugins` folder, create a new folder called `translit-plugin`
2. Copy these 3 files into the `translit-plugin` folder:
   - `main.js`
   - `manifest.json`
   - (optional) `README.md`

Your folder structure should look like:
```
YourVault/
└── .obsidian/
    └── plugins/
        └── translit-plugin/
            ├── main.js
            ├── manifest.json
            └── README.md (optional)
```

## Step 3: Enable the Plugin

1. Open Obsidian
2. Go to Settings (gear icon) → Community plugins
3. Click "Turn on community plugins" if not already enabled
4. Under "Installed plugins", find "Russian Translit"
5. Toggle it ON

## Step 4: Use the Plugin

1. Open any note
2. Press **F2** to activate translit mode
   - You'll see "🇷🇺 TRANSLIT" appear in the status bar at the bottom
3. Start typing in English - it converts to Russian automatically!
   - Example: type `privet` → get `привет`
4. Press **F2** again to turn off translit mode

## Customizing the Hotkey

If you want to use a different key instead of F2:

1. Go to Settings → Hotkeys
2. Search for "Toggle Translit Mode"
3. Click the hotkey and press your preferred key combination

## Troubleshooting

**Plugin doesn't appear in the list:**
- Make sure the folder is named exactly `translit-plugin`
- Check that `main.js` and `manifest.json` are in the folder
- Try restarting Obsidian

**Translit mode doesn't work:**
- Make sure you see "🇷🇺 TRANSLIT" in the status bar when F2 is pressed
- Try clicking in the editor after activating the mode
- Check that you're in edit mode (not preview mode)

**Need to modify the transliteration mapping:**
- You can edit the source code in `main.ts` and rebuild
- Or contact me for a custom version

## Examples of Usage

When translit mode is ON (F2 pressed):

| You type | You get |
|----------|---------|
| `privet` | `привет` |
| `Moskva` | `Москва` |
| `borshch` | `борщ` |
| `shchuka` | `щука` |
| `tsarь` | `царь` |
| `je`to   | `э`то   |

Enjoy typing in Russian! 🇷🇺