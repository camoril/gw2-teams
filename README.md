# GW2 Teams — WvW Roster & Squads

GW2 Teams is a single-page web app to manage Guild Wars 2 World vs World (WvW) rosters and compare/import squads from other users. It runs locally in your browser (no backend) and uses Tailwind CSS via CDN.

## Features
- **Roster Management**: 
  - Add players/characters with role, class/spec, gear quality, notes, and tags.
  - **Subgroup Management**: Organize players into 15 subgroups.
  - **Generic Characters**: Quickly add placeholder characters for theory-crafting based on class/spec.
- **Advanced Analysis**:
  - **Team Boons**: Auto-aggregates boons provided by the entire roster.
  - **Subgroup Analysis**: Visual cards for each subgroup showing specific boon coverage (Quickness, Alacrity, etc.) to ensure balanced parties.
  - **Role Presets**: Apply templates like "Zerg 30", "Minstrel Blob", or "Boon Ball" to set role targets and track composition progress.
- **Data Management**:
  - **Local Storage**: All data persists in your browser.
  - **Import/Export**: Support for JSON (full/filtered) and CSV formats.
  - **Squads**: Import external rosters as separate squads to compare or merge.

## Usage
Online demo: https://hypercube.com.mx/gw2_roster/

1. Open `index.html` in your browser (or use VS Code Live Server).
2. Fill the form to add characters to your roster.
3. Use the top buttons to export/import roster JSON.
4. Use "Import as Squad" to bring in another group's JSON as a separate squad.
5. Click "Manage Squads" to view, export, merge, or delete squads.

## Data Format
Roster and Squad JSON files are arrays of character objects:

```json
[
  {
    "playerName": "Player",
    "characterName": "Character",
    "role": "Ranged Healer",
    "subgroup": "1",
    "classSpec": "elementalist-tempest",
    "gear": "Legendary",
    "tags": ["tag1", "tag2"],
    "notes": "Optional notes"
  }
]
```

## Development
- Stack: HTML5 + Tailwind CSS (CDN) + Vanilla JavaScript.
- Preview locally: 
  ```bash
  python3 -m http.server
  ```
- No build step or external dependencies.

## Security & Privacy
- Data is stored only in your browser via `localStorage`.
- Exported JSON contains the roster/squad members you added or imported; review before sharing.

## License
This project is licensed under the GNU General Public License v3.0 (GPL-3.0).

- Full text: see `LICENSE` in the repository or https://www.gnu.org/licenses/gpl-3.0.txt
- You may copy, modify, and distribute under the terms of GPLv3.
- This app includes links to external icons hosted on the GW2 Wiki; those assets are subject to their respective licenses and are not bundled in this repository.

## Author
Ernesto Pineda Batalla (camoril)
