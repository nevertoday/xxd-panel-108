---
name: xxd-panel-108
description: "Turn each source photograph into a strict 50:50 top-bottom or left-right poster whose transformed half distils the subject into contemporary folk-art paper-cut collage with print texture and generous whitespace. Use when the user invokes xxd-panel-108 or requests this exact independent Panel style."
---

# XXD Panel 108

Create finished PNG artwork from the current user-supplied photograph or image directory. The complete Chinese source brief at `references/original-prompt/zh-CN.md` is the sole creative and aesthetic authority. Read it in full immediately before every generation; do not summarise, translate, merge, or replace it with this file, a README, a sample, or another Panel.

## Delivery contract

- Every source is its own isolated job. Never combine source photographs, reuse another source's wording, or feed a generated result through a second style pass.
- The source brief's canonical presentation is a 3:4 portrait canvas with two equal horizontal regions: faithful photograph above and the transformed design below, exactly 50:50.
- Support four explicit modes: `top-bottom` (reality above, design below), `left-right` (reality left, design right), `design-only` (full-canvas design, source remains reference only), and `wallpaper-pack` (one complete design per device). Selected comparison modes always have exactly two equal regions and no header, footer, inset panel, grid, collage, or third band.
- Resolve all runtime variables before generation: source, one or more modes, one or more sizes, text mode, locale, wallpaper relationship, device sizes, and output root. Never invent a silent ratio or locale.
- A directory input is explicit batch intent. Inventory supported raster files in stable order, report the count, resolve shared settings once, generate each source independently, and account for every success or failure.

## Prompt authority and runtime variables

For each output, concatenate the complete verbatim Chinese source brief, then a short delivery preamble, exactly one selected mode contract, exactly one text contract, and the user's explicit non-style requirements. Runtime additions may change only delivery variables (mode, canvas, source visibility, device, wallpaper relation, language, or exact user copy). Never add an outer palette, title, slogan, or aesthetic theory.

Text modes are `prompt` (model writes source-grounded concise copy in the requested locale), `exact` (user copy is passed verbatim), and `none` (no letters, numbers, logos, labels, or pseudo-text). Do not infer language from the image or filename.

The built-in image tool is preferred. If it is exposed, follow the installed `imagegen` Skill and make one complete-canvas call per distinct output. If no compatible image route is available, ask the user to enable one or provide an API key voluntarily; never expose secrets. Use `scripts/compose_panel.py` only for exact raster sizing, source preservation, or read-only audits, never to invent the design.

## Output and acceptance

Write every final PNG directly into one fresh task directory under `~/Desktop/xxd/xxd-panel-108/` (or the explicit `--out` root). Use names such as `source-001-name-top-bottom-3x4-1536x2048.png`; do not create source/mode/size subdirectories or contact sheets. Inspect every result at full size and thumbnail size. Accept only fresh PNGs with the requested ratio, source visibility, strict split direction and 50:50 midpoint, direct transformation from the current original source, faithful adherence to the Chinese brief, requested text behaviour, and no watermark, SVG substitute, UI, hidden third band, or second-pass artefact.

For linked wallpapers, create one anchor from the original source, then independently recompose each remaining device with the original source plus that anchor. Independent wallpapers receive only the original source.

## References

- `references/original-prompt/zh-CN.md` — canonical source brief used at runtime
- `references/original-prompt/README.md` — translation index and authority note
- `references/runtime-preferences.md` — safe delivery-preference reuse
- `references/xxd-panel-108-prompt.zh-CN.md` and `.en.md` — concise runtime adapter notes
