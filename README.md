# Scroll of Beasts

An [Obsidian](https://obsidian.md) plugin for browsing D&D5e monster statblocks. Designed for use with the [Fantasy Statblocks](https://github.com/javalent/fantasy-statblocks) plugin.

## Features

- Searches your Fantasy Statblocks bestiary
- Filter monsters by name, type, subtype, size, CR, and first letter
- Animated rune display as the scroll updates
- Tally bar shows filtered vs. total monster count, with a sense of humor
- Optional Forgotten Realms wiki integration — shows intro text, lore, and images for selected monsters
- Optional local monster folder support for your own non-statblock entries
- Works on desktop and mobile (tested on iOS)

## Requirements

- [Fantasy Statblocks](https://github.com/javalent/fantasy-statblocks) plugin installed and populated with monster data

## Installation via BRAT

1. Install the [BRAT](https://github.com/TfTHacker/obsidian42-brat) plugin
2. Open BRAT settings → **Add a beta plugin for testing**
3. Enter: `EricJLange/scroll-of-beasts`
4. Enable the plugin in Settings → Community Plugins

## Manual installation

1. Download `main.js` and `manifest.json` from this repository
2. Create a folder `.obsidian/plugins/scroll-of-beasts/` in your vault
3. Copy both files into that folder
4. Reload Obsidian and enable the plugin in Settings → Community Plugins

## Monster folders configuration

1. In Scroll of Beasts plugin settings, click Add Folder.
2. Modify the path to point to a custom folder containing monster notes. Example: DnD/Common/Monsters
3. Add notes in this folder with non-statblock monster stuff. Example: Goblinoids.md is a note with my dossier on all goblin and hobgoblin types, including lore and encounter suggestions

## Forgotten Realms wiki configuration

1. In Scroll of Beasts plugin settings, check the box to Fetch lore & image from Forgotten Realms wiki
2. The free FR wiki will provide information for discovered beasts



