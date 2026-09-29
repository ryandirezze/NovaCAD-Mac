# NovaCAD Marketing Hero Design

## Understanding Summary

- Create polished 5:2 hero images positioning NovaCAD as native CAD for macOS.
- Speak primarily to Mac-based CAD professionals in engineering, architecture,
  facilities, and plant-layout work.
- Show recreated product UI with original synthetic geometry, never real or
  proprietary CAD layouts.
- Use a dark, precision-focused visual system.
- Keep each composition effective in a GitHub README and social-media feed.
- Deliver editable SVG sources and ready-to-share PNG exports.

## Assumptions

- Each master asset is 2500 x 1000 pixels, an exact 5:2 aspect ratio.
- Copy is concise and factual; open source supports rather than replaces the
  primary native-macOS message.
- macOS character is conveyed through interface proportions and materials,
  without Apple, Autodesk, AutoCAD, or other third-party marks.
- All technical geometry is original artwork created for the campaign.
- Assets have no network dependencies or external image references.
- Typography and major messages remain legible near 1000 x 400 pixels.
- SVG sources remain understandable and editable without adding application
  runtime code or dependencies.
- The assets are campaign artwork, not feature-comparison charts or literal
  pixel-perfect screenshots.

## Final Design

### Precision Workspace

An asymmetric headline-and-product composition. The left side leads with
"Native CAD for Mac" and concise proof points. The right side contains a large,
polished NovaCAD window showing a fictional industrial plan, an active
measurement, and markup. Cyan geometry extends slightly beyond the app window
to suggest an expansive technical workspace.

### Infinite Canvas

An immersive charcoal drafting surface covered by an original micro-factory
layout. Floating NovaCAD controls align with the geometry instead of forming a
complete centered window. The headline "Your drawings. At Mac speed." creates
a stronger editorial and social-media treatment while a badge preserves the
"Native CAD for Mac" position.

### Technical Triptych

A compact product story organized around three overlapping scenes: Navigate,
Measure, and Mark up. A narrow title rail holds the NovaCAD identity and lead
message. Different drawing scales and densities turn the panels into a workflow
rather than a generic feature-card grid.

## Shared Visual System

- Near-black and charcoal backgrounds with restrained blue atmosphere.
- White and cyan drawing geometry, with red-orange reserved for markup.
- Fine drafting grids, coordinate ticks, and sparse dimensions for texture.
- Simplified UI labels and controls based on NovaCAD's real application
  structure: ribbon, layers, properties, status, and command prompt.
- No customer filenames, paths, personal data, screenshots, or proprietary
  drawing content.

## Decision Log

| Decision | Alternatives | Reason |
| --- | --- | --- |
| Create three coordinated concepts | Select one concept | The user wants all three for channel testing and comparison. |
| Use polished UI recreation | Authentic screenshot; hybrid | Real layouts cannot be included, and a recreation gives complete control over privacy and clarity. |
| Lead with "Native CAD for Mac" | Performance; open source; workflow | This is the clearest differentiated product position for the target audience. |
| Use dark precision styling | Bright macOS; blueprint editorial; monochrome | It best conveys professional CAD density and premium native software. |
| Target Mac CAD professionals | Open-source developers; plant teams; broad Mac users | This audience most directly benefits from the product proposition. |
| Export SVG and PNG | PNG only; SVG only | SVG supports maintenance while PNG is immediately shareable. |
| Use 2500 x 1000 masters | Channel-specific dimensions | One exact 5:2 master remains versatile across GitHub and social channels. |

## Risks And Mitigations

- Small UI details may disappear in social feeds. Keep headlines and primary
  scene silhouettes readable without relying on labels.
- A recreated UI can overstate product fidelity. Base the structure on actual
  NovaCAD surfaces and avoid depicting unsupported workflows.
- Dense geometry can compete with copy. Reserve deliberate dark zones around
  each headline and limit accent colors.
- Font substitution can change layout. Use conservative fallback stacks and
  convert critical display text to stable SVG positioning.
