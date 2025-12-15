# GW2 Teams — TODO

This document organizes proposed improvements by estimated implementation difficulty. Each item includes a short description and key tasks.

## Completed
- **Subgroup Management**: Organize roster into 15 subgroups with visual grid layout.
- **Subgroup Analysis**: Real-time boon coverage visualization per subgroup (Quickness, Alacrity, etc.).
- **Find Classes by Boon**: Reverse lookup tool to find providers for specific boons.
- **Role Presets**: One-click application of standard compositions (Zerg 30, Minstrel Blob, etc.).
- **Role Targets**: Configurable quotas per role with progress tracking.
- **Generic Characters**: Quick creation of placeholder characters for theory-crafting.
- **Sorting & Filters**: Table sorting by role/spec/gear plus quick filters (search, role, gear, tag).
- **Inline Editing**: Per-row edit/save/cancel with validation.
- **Duplicate Detection**: Detect duplicates on add/import/merge.
- **Export Options**: Filter-aware JSON and CSV exports.
- **Validation & Schema**: Schema checks on add/import/merge.
- **Print-Friendly View**: Print CSS hides controls and lightens backgrounds.
- **Notes & Tags**: Tags field, pill display, and tag filter.
- **Reset Roster**: Button to clear all roster data with confirmation.

## Medium
- **Squad Analytics**: Per-squad dashboard (full boon coverage, role distribution, gear histogram).
- **Merge Strategy**: Smart merge with conflict resolution (keep newest, keep local, prompt per entry).
- **Boon Weights**: Priority scoring per WvW meta; compute team score and highlight missing high-weight boons.
- **URL Sharing**: Encode roster/squad selection in URL for shareable state.
- **i18n**: Language toggle (ES/EN) for roles, boons, and UI labels.
- **Backup/Restore**: Export/import full app state (roster + squads) and periodic auto-backup.

## Hard
- Squad Comparison: Side-by-side comparison between two squads and the roster with diffs, heatmaps.
- Performance Optimizations: Lazy rendering for large datasets, debounced updates, memoized aggregation.
- Gear Details Guidance: Extended fields (runes/sigils/infusions) with meta-based hints per archetype.
- Advanced Analytics: Role synergy scoring, boon uptime estimation, and recommended adjustments.
- About/Help System: Rich help modal with contextual tips, links to GW2 Wiki, and onboarding flow.

## Notes
- Start with Easy items to improve usability quickly (Sorting, Duplicates, Inline Editing).
- Medium items add depth for planning and collaboration.
- Hard items require careful UX design and performance considerations.