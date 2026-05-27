# Design sources

Editable design files for the site's binary assets. Tracked in git so the
source survives, but NEVER deployed.

This directory sits outside `docs/`. MkDocs only publishes from `docs/`,
so nothing here ships to `site/` or to the production publication.

## Contents

PSD and other editable sources for the rendered assets that live under
`docs/media/` and `docs/`. Examples (added as we make them):

- `favicon.psd`: source for the site favicon set rendered to
  `docs/favicon.ico` (and any sized PNG variants).
- `boop-and-wobble-cover.psd`: source for the cover illustration rendered
  to `docs/media/boop-and-wobble-cover.png` (and any WebP variants).
- `og-image.psd`: source for `docs/media/og-image.png` (1200x630 social
  card) if/when a static OG image is shipped.

## Adding new design sources

1. Put the editable file here (`assets/<name>.psd`).
2. Export the rendered asset to its final location under `docs/` (e.g.
   `docs/media/<name>.png`, or `docs/favicon.ico` for site-root icons).
3. Reference the rendered asset, not the source, from markdown, theme
   config, or HTML overrides.

## Why this layout

Design sources are tracked (so the editable file survives team handoff,
software upgrades, and laptop turnover) but excluded from publish (so
the PSD never ends up downloadable next to the rendered PNG). Rendered
assets live next to the content that references them.
