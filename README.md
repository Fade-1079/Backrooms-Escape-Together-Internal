
Internal cheat DLL for **Backrooms: Escape Together**. 
Injectable DLL, Console commands, No GUI
I'll upload the source if this gets 20 stars 

---

## Features

### ESP
Every entity in your level gets drawn with a screen-space box, a name label, a distance readout, and a head dot so you can track them through walls and around corners. Box height and width scale with distance so far-away targets stay readable and up-close ones don't blow up your screen.

### Player ESP
Draws every other player in the server. Labels use their **real in-game name** prefixed with `@`, plus their character class so you know who's who and what they're running. Color-coded red. Your own character is filtered out — you won't see a box over yourself.

### Entity / Monster ESP
Draws AI entities and hostile NPCs in **purple**. Same box + name + distance treatment as players. Toggleable independently from player ESP so you can run one without the other.

### Object ESP
Draws world objects and actors you'd normally have to hunt for — item pickups, interactables, anything in the level that isn't a player or a monster. Color-coded orange, small dot marker instead of a full box so it doesn't clutter the screen.

### Proximity Alerts
When any player or monster gets within a set distance of you, a **huge flashing red banner** fires across the top of your screen with their name and how close they are. Pulsing fade in and out, thick border, positioned so you can't miss it. Distance threshold is adjustable.

### Console
Everything is driven from an in-game console. No menus, no clicking, no overlays stealing your mouse. Type a command, get an effect. Commands use plain English with `0`/`1` for on/off so there's nothing to memorize.

### Entity Lists
The top-right of your screen shows live, scrollable lists of everything currently in your level — players, monsters, and objects separated into their own panels with index numbers, real names, class names, and world coordinates for each entry. Use it to see exactly what's loaded and where it is.

### Configurable Distances
Set your max ESP draw distance and your proximity alert range on the fly. Default max draw distance is effectively unlimited so nothing gets culled, but you can clamp it down if you want a lighter overlay.

---

## Commands

Toggle any ESP layer with `0` (off) or `1` (on). Plain English also works.

| Command | Effect |
|---|---|
| `playeresp 0\|1` | Toggle player ESP |
| `monsteresp 0\|1` | Toggle monster / entity ESP |
| `objectesp 0\|1` | Toggle object ESP |
| `proximityesp 0\|1` | Toggle proximity alerts |
| `proximityrange <n>` | Set proximity alert distance |
| `maxdrawdistance <n>` | Set max ESP draw distance |
| `getplayerposition` | Print your current world position |
| `listplayers` | List every player with name and coords |
| `listmonsters` | List every monster with class and coords |
| `listobjects [n]` | List objects (default 100) |
| `clearconsole` | Clear the console |
| `quit` | Close the console |

---

## Install

1. Download the DLL .
2. Launch **Backrooms: Escape Together**.
3. Inject the DLL with a DLL Injector
4. A console window opens, Cheat is loaded

---

## Questions / Help

DM **@fade1079** on Discord.