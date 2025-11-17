# Auto-Promote

Automatically promote raid members to assistant based on customizable rules. Perfect for raid leaders who want to streamline raid management.

## Features

- **Flexible Promotion Rules**: Promote players by name, class, or both
- **Smart Auto-Management**: Automatically promotes when raid composition changes
- **Easy Configuration**: Simple slash commands and right-click menu integration
- **Class-Based Promotion**: Option to automatically promote all Mages and/or Paladins
- **Manual Control**: Full control over individual promotions via raid context menu

## Installation

1. Download the latest release
2. Extract to your `Interface/AddOns` folder
3. Restart WoW or reload UI (`/reload`)

## Usage

### Slash Commands

Type `/autopromote` or `/ap` followed by:

| Command | Description |
|---------|-------------|
| `toggle` | Enable/disable the addon |
| `add <name>` | Add player to promotion watchlist |
| `rem <name>` | Remove player from watchlist |
| `list` | Show current watchlist |
| `mages` | Toggle auto-promotion for all Mages |
| `paladins` | Toggle auto-promotion for all Paladins |
| `promote` | Run promotion check manually |

### Right-Click Menu

1. Open raid frame (`O` key)
2. Right-click any player
3. Select **"AutoPromote"** to add/remove them from watchlist
   - ✅ Checked = Player will be auto-promoted
   - ❌ Unchecked = Player won't be auto-promoted

### Examples

```lua
/autopromote mages          -- Auto-promote all Mages
/autopromote add Playername -- Add specific player
/autopromote list           -- View promotion list
