# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

GPSA Rulebook — a Quarto book project that builds three output formats from Markdown source files:

- **HTML website** served at `rulebook.gpsaswimming.org` (via Cloudflare Pages)
- **PDF** with custom GPSA branding (`GPSA-Rulebook.pdf`)
- **ePub** for e-readers (`GPSA-Rulebook.epub`)

Two companion sub-projects render PDF-only documents to the same `docs/` output directory:
- `constitution/` → `GPSA-Constitution.pdf`
- `code-of-conduct/` → `GPSA-Code-of-Conduct.pdf`

## Commands

```bash
# Build all formats (HTML + PDF + ePub)
quarto render

# Build specific format
quarto render --to pdf
quarto render --to html
quarto render --to epub

# Live preview with auto-reload
quarto preview

# Build constitution PDF
cd constitution && quarto render

# Build code of conduct PDF
cd code-of-conduct && quarto render

# Clear build cache
quarto render --cache-refresh
```

**Requirements:** Quarto (`brew install quarto`) and TinyTeX (`quarto install tinytex`) for PDF generation.

## Deployment

Push to `main` → GitHub Actions builds all formats → deploys `docs/` to Cloudflare Pages (`gpsa-rulebook`).

**Required GitHub secrets:**
- `CLOUDFLARE_API_TOKEN` — API token with Cloudflare Pages edit permissions
- `CLOUDFLARE_ACCOUNT_ID` — Found in the Cloudflare dashboard right sidebar

Do not commit the `docs/` directory — GitHub Actions generates it on every push.

## Architecture

### Configuration

| File | Purpose |
|---|---|
| `_quarto.yml` | Book structure, chapter order, all output format settings |
| `_metadata.yml` | Draft mode flag (`gpsa_draft: true/false`) |
| `_custom.scss` | GPSA brand styling for HTML output |
| `filters/` | Lua filters for draft watermark (PDF) and draft banner (HTML) |

### Draft Mode

Uses a **custom `gpsa_draft` flag** in `_metadata.yml` — not Quarto's native `draft:` field, which breaks sidebar navigation.

- `gpsa_draft: true` → diagonal "DRAFT" watermark on PDF, sticky banner on HTML
- `gpsa_draft: false` → production output, no draft indicators

Implemented via Lua filters in `filters/`:
- `draft-watermark.lua` — injects LaTeX watermark for PDF
- `draft-banner.lua` — injects HTML/CSS banner for web

### Output Structure

All three projects write to the root `docs/` directory:
- Rulebook HTML → `docs/` (index, chapters)
- Rulebook PDF → `docs/GPSA-Rulebook.pdf`
- Rulebook ePub → `docs/GPSA-Rulebook.epub`
- Constitution PDF → `docs/GPSA-Constitution.pdf`
- Code of Conduct PDF → `docs/GPSA-Code-of-Conduct.pdf`

### Sub-Projects (`constitution/` and `code-of-conduct/`)

Each is a standalone Quarto PDF-only book. Their `_quarto.yml` sets `output-dir: ../docs` so they land alongside the main rulebook output. The logo path (`../gpsa_logo.png`) resolves to the root-level logo. Both use their own `filters/draft-watermark.lua` copies.

## Content Files

All chapters are Markdown at the root level. Chapter order is defined in `_quarto.yml` under `book.chapters`.

To add a chapter: create the `.md` file, add it to the `chapters` list in `_quarto.yml`, run `quarto render`.

## Key Differences from Standard Quarto

- **Custom draft system** (`gpsa_draft`) instead of native `draft:` — native draft breaks sidebar navigation
- **Extensive LaTeX customization** in `_quarto.yml` for PDF cover page, headers/footers, section numbering
- **Fixed header CSS** in `_custom.scss` overrides Headroom.js scrolling behavior
- **Constitution uses roman numeral section numbering** via `filters/roman-numerals.lua`
