# Scroll of Beasts

An [Obsidian](https://obsidian.md) plugin for browsing D&D5e monster statblocks. Designed for use with the [Fantasy Statblocks](https://github.com/javalent/fantasy-statblocks) plugin.

## Features

- Searches your Fantasy Statblocks bestiary
- Filter monsters by name, type, subtype, size, CR, and first letter
- Animated rune display as the scroll updates
- Tally bar shows filtered vs. total monster count, with a sense of humor
- Optional Forgotten Realms wiki integration — shows intro text, lore, and images for selected monsters
- Local monster folder support — notes with `name`, `cr`, `size`, `type` frontmatter appear in search with full metadata; multi-monster notes use a `monsters:` array
- Works on desktop and mobile (tested on iOS)

## Requirements

- [Fantasy Statblocks](https://github.com/javalent/fantasy-statblocks) plugin installed and populated with monster data

## Installation via BRAT

1. Install the [BRAT](https://github.com/TfTHacker/obsidian42-brat) plugin
2. Open BRAT settings → **Add a beta plugin for testing**
3. Enter: `Edjil/scroll-of-beasts`
4. Enable the plugin in Settings → Community Plugins

## Manual installation

1. Download `main.js` and `manifest.json` from this repository
2. Create a folder `.obsidian/plugins/scroll-of-beasts/` in your vault
3. Copy both files into that folder
4. Reload Obsidian and enable the plugin in Settings → Community Plugins

## Monster folders configuration

1. In Scroll of Beasts plugin settings, click **Add Folder**.
2. Set the path to your custom monster notes folder. Example: `DnD/Common/Monsters`
3. Add frontmatter to notes so they appear in search with correct CR, size, and type.

**Single monster note:**
```yaml
---
name: Gulthias Tree
cr: "4"
size: Huge
type: Plant
---
```

**Multi-monster note** (e.g. a note covering several variants):
```yaml
---
monsters:
  - name: Goblin Warrior
    cr: "1/4"
    size: Small
    type: Fey
    subtype: Goblinoid
  - name: Goblin Boss
    cr: "1"
    size: Small
    type: Fey
    subtype: Goblinoid
---
```

Notes without frontmatter still appear in the folder link list but show N/A for CR/size/type. Notes whose names match a Fantasy Statblocks bestiary entry will have their local note linked automatically (no frontmatter required for that).

## Forgotten Realms wiki configuration

1. In Scroll of Beasts plugin settings, check the box to Fetch lore & image from Forgotten Realms wiki
2. The free FR wiki will provide information for discovered beasts



