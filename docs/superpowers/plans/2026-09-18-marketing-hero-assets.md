# NovaCAD Marketing Hero Assets Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Produce three coordinated, privacy-safe 5:2 NovaCAD marketing concepts as editable SVG files and ready-to-share PNG exports.

**Architecture:** Each concept is a standalone 2500 x 1000 SVG under `Assets/Marketing`, with self-contained gradients, filters, typography, interface shapes, and original CAD geometry. The three SVGs are independently authored from the approved design brief, then rendered and validated as one batch so dimensions and output behavior remain consistent.

**Tech Stack:** SVG 1.1-compatible vector markup, macOS Quick Look (`qlmanage`) or available SVG renderer, ImageMagick/file metadata tools when available, Git.

---

## File Structure

- `Assets/Marketing/novacad-precision-workspace.svg`: Headline-and-product hero with a large reconstructed app window.
- `Assets/Marketing/novacad-infinite-canvas.svg`: Full-bleed synthetic drawing with floating NovaCAD controls.
- `Assets/Marketing/novacad-technical-triptych.svg`: Three-stage Navigate/Measure/Mark up workflow composition.
- `Assets/Marketing/novacad-precision-workspace.png`: Raster export of the first concept.
- `Assets/Marketing/novacad-infinite-canvas.png`: Raster export of the second concept.
- `Assets/Marketing/novacad-technical-triptych.png`: Raster export of the third concept.
- `docs/marketing-hero-design.md`: Approved brief, constraints, risks, and decision log.

### Task 1: Precision Workspace Source

**Files:**
- Create: `Assets/Marketing/novacad-precision-workspace.svg`

- [ ] **Step 1: Create a 2500 x 1000 SVG root and shared dark-precision definitions**

Use `viewBox="0 0 2500 1000"`, a near-black background, subtle cyan atmosphere, a drafting grid, and restrained shadow/glow filters.

- [ ] **Step 2: Build the left messaging region**

Include `OPEN SOURCE · NATIVE macOS`, the headline `Native CAD` / `for Mac.`, supporting workflow copy, and three compact proof points.

- [ ] **Step 3: Build the reconstructed app window**

Include a title bar, ribbon, layer panel, properties panel, command line, and status bar based on the product's documented structure.

- [ ] **Step 4: Add original industrial geometry and active workflow indicators**

Draw fictional structural bays, equipment cells, pipe routes, dimensions, a cyan selection, a red-orange markup path, OSNAP markers, and a measurement readout.

- [ ] **Step 5: Verify the source contract**

Run: `xmllint --noout Assets/Marketing/novacad-precision-workspace.svg`

Expected: exit code 0 with no output.

### Task 2: Infinite Canvas Source

**Files:**
- Create: `Assets/Marketing/novacad-infinite-canvas.svg`

- [ ] **Step 1: Create a 2500 x 1000 full-bleed drafting surface**

Use original micro-factory geometry, subtle coordinate ticks, and a deliberate dark copy zone in the upper-left.

- [ ] **Step 2: Add the editorial message**

Include `Your drawings.` / `At Mac speed.`, a `NATIVE CAD FOR MAC` badge, NovaCAD identification, and concise open-source DWG/DXF copy.

- [ ] **Step 3: Add floating native controls**

Create a partial ribbon, layer panel, measurement card, command prompt, and compact status controls aligned to the underlying geometry.

- [ ] **Step 4: Add action hierarchy**

Use cyan for selected geometry and warm red-orange for a proposed route, keeping white geometry secondary and original.

- [ ] **Step 5: Verify the source contract**

Run: `xmllint --noout Assets/Marketing/novacad-infinite-canvas.svg`

Expected: exit code 0 with no output.

### Task 3: Technical Triptych Source

**Files:**
- Create: `Assets/Marketing/novacad-technical-triptych.svg`

- [ ] **Step 1: Create the title rail and atmospheric background**

Set the NovaCAD identity, `Native CAD for Mac.`, supporting copy, and oversized ghosted coordinates behind the scene panels.

- [ ] **Step 2: Build the Navigate scene**

Show dense synthetic linework, a search field/result, and highlighted fictional equipment text.

- [ ] **Step 3: Build the dominant Measure scene**

Show a fictional building bay, diagonal measurement, endpoint markers, delta values, and a clear distance readout.

- [ ] **Step 4: Build the Mark up scene**

Show selected geometry, a red-orange proposed route, layer controls, and an active command prompt.

- [ ] **Step 5: Add workflow labels and capability baseline**

Include `01 NAVIGATE`, `02 MEASURE`, `03 MARK UP`, plus `DWG · DXF · XREFS · HUGE DRAWINGS`.

- [ ] **Step 6: Verify the source contract**

Run: `xmllint --noout Assets/Marketing/novacad-technical-triptych.svg`

Expected: exit code 0 with no output.

### Task 4: Raster Exports

**Files:**
- Create: `Assets/Marketing/novacad-precision-workspace.png`
- Create: `Assets/Marketing/novacad-infinite-canvas.png`
- Create: `Assets/Marketing/novacad-technical-triptych.png`

- [ ] **Step 1: Detect the available SVG renderer**

Run: `command -v magick || command -v rsvg-convert || command -v qlmanage`

Expected: one executable path.

- [ ] **Step 2: Render each SVG at its native 2500 x 1000 size**

Use the detected renderer without external resources or network access.

- [ ] **Step 3: Confirm all PNG files are valid images**

Run: `file Assets/Marketing/*.png`

Expected: three PNG image files, each reporting 2500 x 1000 dimensions.

### Task 5: Integrated Quality Gate

**Files:**
- Verify: `Assets/Marketing/*.svg`
- Verify: `Assets/Marketing/*.png`
- Verify: `docs/marketing-hero-design.md`

- [ ] **Step 1: Validate every SVG as XML**

Run: `xmllint --noout Assets/Marketing/*.svg`

Expected: exit code 0 with no output.

- [ ] **Step 2: Verify exact aspect ratio and raster dimensions**

Run: `sips -g pixelWidth -g pixelHeight Assets/Marketing/*.png`

Expected: every file reports `pixelWidth: 2500` and `pixelHeight: 1000`.

- [ ] **Step 3: Inspect raster previews**

Open or read each PNG and confirm there is no clipping, missing text, rendering artifact, or accidental blank region.

- [ ] **Step 4: Audit privacy and claims**

Confirm the images contain no real drawing, customer identifier, personal information, external logo, unsupported product claim, or AutoCAD/Autodesk branding.

- [ ] **Step 5: Review the final diff**

Run: `git status --short && git diff --stat && git diff -- docs/marketing-hero-design.md docs/superpowers/plans/2026-09-18-marketing-hero-assets.md`

Expected: only the approved design documentation and six intended marketing assets are present.
