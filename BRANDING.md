# BRANDING.md: Atelier Sound (based on SoundCraft)

This branch (`academy`) is SoundCraft by the ArtCraft team with **rebranding** and one small
change made by The Agent Factory for Claude Academy: in the browser build, the interface language follows
`?lang=xx` in the page address (set by the Claude Academy tools page), then the browser's preferred
languages (upstream always shows English on the web). Where the app has no French catalog we add
one (`rebrand/apps/<app>/fr.tsv` in the deploy repo). No format or engine code is changed.

| | |
|---|---|
| Upstream | https://github.com/storytold/soundcraft (tag in `UPSTREAM_TAG` of the deploy repo's versions.env) |
| Licence | MIT OR Apache-2.0, unchanged (`LICENSE-MIT`, `LICENSE-APACHE`, `NOTICE`) |
| Name shown in the app | Atelier Sound (French: Atelier Son) |
| Credit line | "Based on SoundCraft by the ArtCraft team (github.com/storytold/soundcraft)." |
| Not affiliated | with the ArtCraft team, Adobe or Microsoft |

Why: `docs/brand/LICENSE-brand.txt` of the original says a modified version must remove the
ArtCraft name and marks and must not present itself as an ArtCraft product, while plain-text
credit is allowed. The product name SoundCraft is not covered by that license; we still
show our own name in the title, About box and start screen so nobody thinks the ArtCraft team
runs this copy. Crate names, binaries and file extensions are unchanged.

Every change is made by `rebrand/rebrand.py soundcraft` in the deploy repo (rules in
`rebrand/apps/soundcraft.toml`); each changed file starts with a one-line change notice.
In-app links: community -> https://www.skool.com/claudeacademy, website -> https://claudeacademy.ca.

## Files changed by `rebrand.py`

- `apps/soundcraft-web/index.html`
- `apps/soundcraft-web/src/web.rs`
- `crates/ui-egui/src/menus.rs`
- `crates/ui-egui/src/panels.rs`

## Removed (ArtCraft marks, not licensed to forks)

- `docs/brand`
