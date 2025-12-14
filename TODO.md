# GW2 Teams — TODO

This document organizes proposed improvements by estimated implementation difficulty. Each item includes a short description and key tasks.

## Easy
- Sorting & Filters: Add table sorting by role/spec/gear and quick filters (e.g., Legendary, Support).
- Inline Editing: Click-to-edit rows for role/gear/notes without re-entering the form.
- Duplicate Detection: Detect duplicates on import (`playerName` + `characterName`) with simple merge/skip options.
- Export Options: CSV export and filtered JSON exports (e.g., only Healers). Per-squad metadata in export filename.
- Validation & Schema: Basic schema check for imports, with clear error messages.
- Print-Friendly View: Layout optimized for printing or PDF export of team sheet.
- Notes & Tags: Per-character tags (e.g., commander, backup) and searchable notes.
- Accessibility: Keyboard navigation, ARIA roles, and high-contrast toggle.

## Medium
- Squad Analytics: Per-squad dashboard (full boon coverage, role distribution, gear histogram).
- Merge Strategy: Smart merge with conflict resolution (keep newest, keep local, prompt per entry).
- Role Targets: Configurable role quotas with live completeness indicators and warnings.
- Boon Weights: Priority scoring per WvW meta; compute team score and highlight missing high-weight boons.
- Presets & Templates: Saved roster presets (e.g., Zerg 30, Strike 10) to scaffold compositions.
- URL Sharing: Encode roster/squad selection in URL for shareable state (guard length, optional short link).
- i18n: Language toggle (ES/EN) for roles, boons, and UI labels.
- Backup/Restore: Export/import full app state (roster + squads) and periodic auto-backup.

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