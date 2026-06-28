# ⚔ Dungeon Master Mate (DMM)

A lightweight, mobile-friendly **Progressive Web App** for tabletop RPG Dungeon Masters. Track encounters, manage NPCs, roll weapon damage, apply status ailments, and keep tabs on HP and XP — all from your phone, no app store required.

---

## Features

- **Player Party** — Save your player roster and pull them into any encounter
- **NPC Library** — Store reusable NPCs with resistance types and boss flags; set level on the fly when adding to an encounter
- **Weapon Library** — Define weapons with custom dice counts, dice types, and bonus damage; roll damage with one tap
- **Ailment Library** — Create status effects with round durations and damage dice (or no damage); ailments auto-expire after their rounds run out
- **Encounter Tracker** — Run multiple encounters with initiative sorting, HP tracking (-1 / -5 buttons), weapon assignment, ailment assignment, and automatic XP tallying
- **Backup & Restore** — Export your full library to a JSON file and import it back anytime
- **Offline Support** — Works with no internet connection after the first load (PWA service worker)
- **Install to Home Screen** — Add to your iPhone or Android home screen for a native app feel

---

## Getting Started

### Use it online

Visit the live app at:
**https://hunteraholicgamingdev.github.io/DungeonMasterMate/**

### Install on your phone

**iPhone / iPad (Safari):**
1. Open the link above in Safari
2. Tap the **Share** button (box with arrow)
3. Tap **Add to Home Screen**
4. Tap **Add**

**Android (Chrome):**
1. Open the link above in Chrome
2. Tap the **⋮ menu**
3. Tap **Add to Home screen**
4. Tap **Add**

---

## How to Use

### 1. Set up your library
- Go to **Players** and add your party members
- Go to **Weapons** and define your weapon dice (e.g. Longsword: 1D8+3)
- Go to **NPCs** and save your monster roster with resistance types
- Go to **Ailments** and create status effects like Poison (3 rounds, 1d4) or Blind (2 rounds, no damage)

### 2. Run an encounter
- Go to **Encounters** and tap **+ New Encounter**
- Add NPCs (you'll be prompted for their level, which sets HP/AC/XP automatically) and Players from your dropdowns
- Enter **initiative** for each combatant — they auto-sort highest to lowest
- Tap ⚔ weapon buttons to roll damage (shown in a toast)
- Use **-1** / **-5** buttons to reduce NPC HP
- Assign ailments with the **Assign Ailment** dropdown — tapping the 🩸 button rolls damage, subtracts HP, and counts down rounds until the ailment expires

### 3. Back up your data
- Go to **Settings** and tap **Export Backup** to save a `.json` file
- Use **Import Backup** to restore it on a new device

---

## Tech Stack

- Pure HTML, CSS, JavaScript — no build tools or frameworks required
- [Tailwind CSS](https://tailwindcss.com/) via CDN for styling
- localStorage for persistent data storage
- PWA service worker for offline caching
- Hosted via GitHub Pages

---

## Local Development

No build step needed. Just open the file:

```bash
git clone https://github.com/hunteraholicgamingdev/DungeonMasterMate.git
cd DungeonMasterMate
open index.html   # or just drag into your browser
```

---

## Roadmap / Ideas

- [ ] Healing buttons (+1 / +5 HP)
- [ ] Custom HP input for NPCs
- [ ] Initiative roll randomizer
- [ ] More ailment damage options (1d8, 1d10, 2d6...)
- [ ] Multiple resistance types per NPC
- [ ] Dark/light theme toggle

---

## License

MIT — free to use, modify, and share.
