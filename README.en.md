<div align="center">

# XXD Panel 108｜New Folk Paper-Cut Journal

Cut the photograph's identity into a quiet paper composition with cultural character

[![Codex Skill](https://img.shields.io/badge/Codex-Skill-000000?style=flat-square)](./SKILL.md)

<a href="README.md">简体中文</a> · <strong>English</strong> · <a href="README.ja.md">日本語</a> · <a href="README.ko.md">한국어</a> · <a href="README.ar.md">العربية</a>

</div>

## Sample works

This repository does not include unreviewed images or samples borrowed from another Panel. Independently generated and reviewed samples will be added here after the first release batch.

Some photographs already carry a strong identity and mood, but need a more deliberate visual reorganisation. **Panel 108** keeps the reality of the photograph and translates the other half through its own independent visual language, for art posters, independent publishing, exhibitions, social content, and design-only outputs.

It addresses the common problems of image and design talking past each other, over-decoration, weak whitespace, and inconsistent delivery across formats.

- One photograph becomes one isolated finished asset; photos are never combined.
- Top-bottom and left-right comparisons are strict 50:50 with no third band.
- Directory inputs are processed independently without cross-source subjects, copy, or results.
- `design-only` and wallpaper modes use the photo as reference only; the untransformed photo is not shown.

## Original prompt · five languages

[简体中文](references/original-prompt/zh-CN.md) · [English](references/original-prompt/en.md) · [日本語](references/original-prompt/ja.md) · [한국어](references/original-prompt/ko.md) · [العربية](references/original-prompt/ar.md)

The Chinese file preserves this project’s original prompt and is the sole creative and aesthetic authority at runtime; the other versions are for reading, documentation, and sharing.

**Keywords:** new folk paper-cutting · flat paper-cut collage · printmaking texture · 2–4 source-derived colours · seal-like key visual · generous negative space

## Four output modes

- `top-bottom`: native 3:4 portrait structure, with the reality photograph above and Panel 108's design below, exactly 50% each.
- `left-right`: reality photograph left and design right, exactly 50% each; never rotated into a top-bottom structure.
- `design-only`: the full canvas contains only this Panel's design transformation; the photograph is reference material only.
- `wallpaper-pack`: generate a complete canvas separately for each device rather than mechanically cropping one image.

Supports multiple ratios, exact pixels, prompt-generated／exact／no-text modes, directory batches, and `linked` or `independent` wallpaper relationships. Each invocation creates one fresh task directory and delivers PNG files.

## Best-fit situations and problems solved

Panel 108 is for photographs whose identity is strong but whose background or ordinary treatment dilutes it. It retains the faithful photograph and rebuilds the design region through contemporary folk paper-cutting: silhouettes, flat colour, carved lines, positive–negative forms, print grain, and generous warm-paper space.

- Choose it for art posters, independent publishing, and exhibition work that need cultural and hand-made character without becoming rustic or childish.
- It removes irrelevant detail, selects 2–4 recognisable source colours, and keeps one seal-like visual centre instead of competing focal points.
- It avoids realistic illustration, glossy vectors, 3D rendering, commercial headline stacks, and template-like craft products.

## Quick fit check

| Question | Panel 108's answer |
|---|---|
| Result | One complete poster pairing faithful reality with a new-folk paper-cut transformation |
| Signature | Flat cut-paper shapes, print grain, a seal-like focal form, and expansive warm whitespace |
| Source fidelity | Identity, structure, pose, light, and colour remain recognisable; only irrelevant information is removed |

## Transformation logic

`read subject and narrative → retain defining anchors → select 2–4 source colours → reduce to silhouettes, paper shapes, carved lines, and negative forms → add print texture and editorial whitespace`

## Complete capability and boundaries

Comparison modes always contain exactly two 50:50 regions with no third band. Design-only and wallpaper outputs show only the transformed design. Each asset is generated directly from its current source in one pass, never from an intermediate result or another Panel. Multiple ratios are independently recomposed; text may be prompt-generated, exact, or absent. Final delivery is PNG raster artwork—never SVG, HTML, Canvas, or programmatic drawing.

## Getting started

```bash
git clone https://github.com/nevertoday/xxd-panel-108.git
mkdir -p ~/.codex/skills
ln -s "$(pwd)/xxd-panel-108" ~/.codex/skills/xxd-panel-108
```

You can also install it directly with `npx skills`:

```bash
npx skills add https://github.com/nevertoday/xxd-panel-108 --skill xxd-panel-108
```

The command fetches the repository from GitHub and installs the same-named Skill. For a user-level Codex installation, append `--global --agent codex --yes`; then restart the agent session and invoke:

```text
$xxd-panel-108
```

Complete specification: [SKILL.md](SKILL.md) · [runtime adapter](references/xxd-panel-108-prompt.en.md) · [original prompt](references/original-prompt/zh-CN.md)

## License

This project is released under the **PolyForm Noncommercial License 1.0.0**. See [LICENSE](LICENSE) for the complete legal text and <https://polyformproject.org/licenses/noncommercial/1.0.0> for the official page.

- Personal study, research, experiments, testing, hobbies, private entertainment, and the noncommercial organisations defined by the license are permitted.
- For noncommercial purposes you may use, copy, modify, create derivative works, and distribute, provided you include the license and every `Required Notice:` supplied by the author.
- Commercial products or services, paid delivery, selling access, and anticipated commercial applications are prohibited; obtain separate written permission for commercial use.
- Only the stated copyright and limited patent rights are granted. No trademark or other unstated rights are granted, and you may not sublicense or transfer the license.
- After written notice of a violation, correct it within 32 days or the licenses end. The project is provided as is, without warranties.
<!-- xxd-panel-catalog:start -->
## XXD Panel catalogue

Each of the 108 Panels keeps its own original prompt and aesthetic logic. This directory lists every project continuously from 001 to 108; the current project is bold.

| Project | Style |
|---|---|
| [xxd-panel-001](https://github.com/nevertoday/xxd-panel-001) | NAÏVE LINE · RETRO PAPER · MIXED MEDIA · WITTY METAPHOR · WARM SPACE |
| [xxd-panel-002](https://github.com/nevertoday/xxd-panel-002) | NARRATIVE CONTOUR · HESITANT LINE · ANALOGOUS COLOUR · SELECTIVE ENLARGEMENT · MISREGISTERED TYPE |
| [xxd-panel-003](https://github.com/nevertoday/xxd-panel-003) | CONTINUOUS BLACK LINE · PUBLIC ISSUE · FORCE POINTS · SILENT SPACE · RELEASE |
| [xxd-panel-004](https://github.com/nevertoday/xxd-panel-004) | LOCAL REALITY · PRECISE SINGLE LINE · GEOMETRIC PERSPECTIVE · THEME COLOUR · CITY-BRAND TYPE |
| [xxd-panel-005](https://github.com/nevertoday/xxd-panel-005) | BLUNT MASSES · DARK STRUCTURAL FIELD · PARTIAL REVEAL · THREE-LAYER COLOUR · SCREENPRINT × PASTEL |
| [xxd-panel-006](https://github.com/nevertoday/xxd-panel-006) | 10–20% SUBJECT · 80–90% PAPER · FINE HAND LINE · FOUR COLOURS MAX · FLAT ACRYLIC |
| [xxd-panel-007](https://github.com/nevertoday/xxd-panel-007) | OBJECT-LIKE MINIATURES · CLOSE-UP / SECTION / REPEAT · STAGGERED PAPER · THIN BLACK NOTES |
| [xxd-panel-008](https://github.com/nevertoday/xxd-panel-008) | ORTHOGRAPHIC ISOMETRIC · PLATFORMS / STAIRS / DOORS · SPATIAL PARADOX · DYNAMIC PASTELS · MATTE 3D |
| [xxd-panel-009](https://github.com/nevertoday/xxd-panel-009) | TINY ANCHOR · VAST NEGATIVE SPACE · ONE SPATIAL RELATION · SPOT COLOUR · HALFTONE SCREENPRINT |
| [xxd-panel-010](https://github.com/nevertoday/xxd-panel-010) | ROUGH BLACK SILHOUETTE · WHITE FEATURE CUTOUT · DRY-MEDIA PAPER · SPARSE SETTING MARKS · PICTURE-BOOK TYPE |
| [xxd-panel-011](https://github.com/nevertoday/xxd-panel-011) | ONE CORE IMAGE · ONE RELATION · CONTINUOUS BLACK LINE · ACTIVE SILENCE · ONE MEMORY COLOUR |
| [xxd-panel-012](https://github.com/nevertoday/xxd-panel-012) | DENSE EMERGENCE · SPARSE DIFFUSION · GEOMETRIC RESTRAINT · ONE VITAL COLOUR · BLACK-GREY MICROTYPE |
| [xxd-panel-013](https://github.com/nevertoday/xxd-panel-013) | ONE HORIZONTAL TICKET · 74/26 SPLIT · HEALING WATERCOLOUR · IVORY SPACE · LOCALISED INFORMATION STUB |
| [xxd-panel-014](https://github.com/nevertoday/xxd-panel-014) | FOLD AND FACET · LAYER AND NEST · SOURCE-LED WEIGHT · REAL PAPER FIBRE · READABLE PAPER TYPE |
| [xxd-panel-015](https://github.com/nevertoday/xxd-panel-015) | DECONSTRUCT–SELECT–DISTIL–RECONSTRUCT · FEW FORMS · STRICT COLOUR ROLES · IVORY SPACE · ART-BOOK MICROTYPE |
| [xxd-panel-016](https://github.com/nevertoday/xxd-panel-016) | ONE SUBJECT · ONE MOTION · A LARGE FIELD OF AIR |
| [xxd-panel-017](https://github.com/nevertoday/xxd-panel-017) | ROUNDED FORM · ROUGH BROKEN LINE · PURE FLAT FILL · BRIGHT FIELDS · LIVELY ASYMMETRY |
| [xxd-panel-018](https://github.com/nevertoday/xxd-panel-018) | ONE VISUAL ANCHOR · FEW DEPTH LAYERS · WARM-IVORY SPACE · MATTE PAPER · COMPLETE MICROTYPE |
| [xxd-panel-019](https://github.com/nevertoday/xxd-panel-019) | RECOGNISE FIRST · REDUCE WITH INTENT · COMPOSE WITH TYPE |
| [xxd-panel-020](https://github.com/nevertoday/xxd-panel-020) | IMPASTO ISLAND · DIMENSIONAL MINIATURE · REAL KNIFE MARKS · GENEROUS PAPER SPACE · RESTRAINED EDITORIAL TYPE |
| [xxd-panel-021](https://github.com/nevertoday/xxd-panel-021) | PURE-BLACK RECTANGLE · SUBJECT MOSTLY INSIDE · ONE FEATURE BREAKS OUT · JITTERY PHOTOCOPY LINE · WHITE NEGATIVE FORM |
| [xxd-panel-022](https://github.com/nevertoday/xxd-panel-022) | PURE-BLACK RECTANGLE · SUBJECT MOSTLY INSIDE · ONE FEATURE BREAKS OUT · CLEAN ELASTIC LINE · ONE COLOUR SIGNAL |
| [xxd-panel-023](https://github.com/nevertoday/xxd-panel-023) | SOURCE-CHOSEN WINDOW · PALE BREATHING GROUND · LIVING COLOURED LIGHT · SPRAY GRAIN · DIFFUSE PROJECTION |
| [xxd-panel-024](https://github.com/nevertoday/xxd-panel-024) | PHOTOGRAPHIC SUBJECT · NARROW PALE WINDOW · SOURCE-ADAPTIVE DIRECTION · EASTERN WHITESPACE · PREMIUM EDITORIAL TYPE |
| [xxd-panel-025](https://github.com/nevertoday/xxd-panel-025) | FIRST-GLANCE SUBJECT · SECOND-GLANCE IMAGE · FIGURE–GROUND REVERSAL · 2–4 MORANDI COLOURS · PHYSICAL SCREENPRINT |
| [xxd-panel-026](https://github.com/nevertoday/xxd-panel-026) | RECOGNISE QUIETLY · REDUCE GENTLY · LET THE PAPER BREATHE |
| [xxd-panel-027](https://github.com/nevertoday/xxd-panel-027) | HEAVY IVORY PAPER · EMBOSS AND DEBOSS · FINE INCISION · MATTE-GOLD FOCUS · MUSEUM ORDER |
| [xxd-panel-028](https://github.com/nevertoday/xxd-panel-028) | ORTHOGRAPHIC ISOMETRIC · SMALL PAPER BASE · SOURCE-DERIVED PALETTE · FINE INK · EDITORIAL MODEL |
| [xxd-panel-029](https://github.com/nevertoday/xxd-panel-029) | HORIZONTAL FIELD · LIGHT WAX PASTEL · ROUGH HANDMADE PAPER · RISOGRAPH GRAIN · RELAXED HANDWRITING |
| [xxd-panel-030](https://github.com/nevertoday/xxd-panel-030) | REAL BOTANICAL MATERIAL · RECTANGULAR FIELD · NATURAL CROSSING · MINIMAL BLACK LINE · EDITORIAL WHITESPACE |
| [xxd-panel-031](https://github.com/nevertoday/xxd-panel-031) | ONE CORE MOTIF · SOURCE-DERIVED GEOMETRY · FOLK CATALOGUE · ROUGH INTERNAL INK · CRISP ORDER |
| [xxd-panel-032](https://github.com/nevertoday/xxd-panel-032) | TEXT–IMAGE UNITY · NATIVE LETTERING · SOURCE FEATURE · OPTICAL SPACING · GENEROUS WHITESPACE |
| [xxd-panel-033](https://github.com/nevertoday/xxd-panel-033) | RECOGNISABLE MOTIF · LAYERED COLLAGE · SCALE CONTRAST · VIVID SOURCE COLOUR · COVER TYPE |
| [xxd-panel-034](https://github.com/nevertoday/xxd-panel-034) | SMALL STAMP · 2–4 SPOT INKS · HAND-CARVED LINE · WARM PAPER · FIELD ANNOTATION |
| [xxd-panel-035](https://github.com/nevertoday/xxd-panel-035) | ONE BLOCK SUBJECT · VIVID SOURCE COLOUR · MATTE ABS · QUIET FIELD · MODULAR TYPE |
| [xxd-panel-036](https://github.com/nevertoday/xxd-panel-036) | ONE RELATION · FINE LINE · 2–4 COLOUR FIELDS · WATERCOLOUR EDGE · BREATHING SPACE |
| [xxd-panel-037](https://github.com/nevertoday/xxd-panel-037) | ONE BADGE · SOURCE ENAMEL · WHITE-METAL RIM · GILDED DETAIL · REAL SHADOW |
| [xxd-panel-038](https://github.com/nevertoday/xxd-panel-038) | SOURCE FABRIC · FRAYED EDGE · HAND STITCH · ACTIVE WHITESPACE · HIDDEN FEELING |
| [xxd-panel-039](https://github.com/nevertoday/xxd-panel-039) | ONE IMAGE · ONE ESSENCE · SILK DIRECTION · CLEAN GROUND · EASTERN SILENCE |
| [xxd-panel-040](https://github.com/nevertoday/xxd-panel-040) | TRUTHFUL ANCHOR · BLACK-LINE FIGURES · MICRO-NARRATIVE · ACTIVE WHITESPACE |
| [xxd-panel-041](https://github.com/nevertoday/xxd-panel-041) | THEME METAPHOR · ISOMETRIC ORDER · PALE MANUSCRIPT · JAPANESE COLOUR · EASTERN SPACE |
| [xxd-panel-042](https://github.com/nevertoday/xxd-panel-042) | ORIGINAL VIEW · 2–5 TRUE LAYERS · STABLE ANCHOR · TRANSLUCENT WATERCOLOUR · EDITORIAL NOTE |
| [xxd-panel-043](https://github.com/nevertoday/xxd-panel-043) | REAL LATHER · FRONTAL FLAT-LAY · SOURCE-DARK GROUND · MICRO-BUBBLE EDGE · QUIET SPACE |
| [xxd-panel-044](https://github.com/nevertoday/xxd-panel-044) | THIN GOLD · FRONTAL PLANE · SOURCE-DARK GROUND · HAMMERED TRACE · QUIET ORDER |
| [xxd-panel-045](https://github.com/nevertoday/xxd-panel-045) | ROUNDED MODULE · SOURCE COLOUR · ISOMETRIC DEPTH · MATTE TOUCH · EDITORIAL MICROTYPE |
| [xxd-panel-046](https://github.com/nevertoday/xxd-panel-046) | BRIGHT GROUND · VIVID IMPASTO · MINIATURE VOLUME · DIAGONAL FIELD · WARM LIGHT |
| [xxd-panel-047](https://github.com/nevertoday/xxd-panel-047) | ISOMETRIC MINIATURE · THEMATIC IMPASTO · REAL CONTACT · WARM-WHITE PAPER · LUMINOUS COLOUR |
| [xxd-panel-048](https://github.com/nevertoday/xxd-panel-048) | TRANSPARENT STRUCTURE · SCIENTIFIC ILLUSTRATION · LUCID MONOCHROME · PRECISE ANNOTATION · EDITORIAL SPACE |
| [xxd-panel-049](https://github.com/nevertoday/xxd-panel-049) | LIMITED-COLOUR WOODCUT · HAND-CARVED MARKS · MATTE INK · WARM PAPER · BROKEN EDGES |
| [xxd-panel-050](https://github.com/nevertoday/xxd-panel-050) | BESPOKE TRAVEL SCENE · AIRY BLUE · MINIMAL FLAT VECTOR · EDITORIAL WHITESPACE · ONE IMAGE, ONE IDENTITY |
| [xxd-panel-051](https://github.com/nevertoday/xxd-panel-051) | MINIATURE PAPER CRAFT · HORIZONTAL FLOATING LANDSCAPE · HANDMADE EVIDENCE · AIRY BLUE · VAST WHITESPACE |
| [xxd-panel-052](https://github.com/nevertoday/xxd-panel-052) | PAPER-CRAFT MINIATURE · HORIZONTAL FLOATING STRIP · HANDMADE MATERIAL · AIRY COOL BLUE · GENEROUS SPACE |
| [xxd-panel-053](https://github.com/nevertoday/xxd-panel-053) | OBSERVATIONAL PEN · TRANSPARENT WASH · MUSICAL RHYTHM · NEAR-WHITE PAPER · ACTIVE WHITESPACE |
| [xxd-panel-054](https://github.com/nevertoday/xxd-panel-054) | SELECTIVE MEMORY · MAIN VISUAL · SIX STICKERS · MATTE PRINT · AIRY BLUE |
| [xxd-panel-055](https://github.com/nevertoday/xxd-panel-055) | SUBJECT NARRATIVE · HEALING PASTELS · LIGHT OIL TEXTURE · AIRY BLUE · EDITORIAL SPACE |
| [xxd-panel-056](https://github.com/nevertoday/xxd-panel-056) | CORE IMAGE · VAST WHITESPACE · WARM–COOL JUMPS · NAIVE HAND · VISUAL METAPHOR |
| [xxd-panel-057](https://github.com/nevertoday/xxd-panel-057) | GEOMETRIC COMPOSITION · INTELLIGENT MOSAIC · ARCHITECTURAL DIAGRAM · ART MAP · WARM–COOL FIELDS |
| [xxd-panel-058](https://github.com/nevertoday/xxd-panel-058) | SUBTEXT READING · GEOMETRIC MINIMALISM · CONCEPTUAL LANDSCAPE · SOFT HANDMADE TEXTURE · PALE SPACE |
| [xxd-panel-059](https://github.com/nevertoday/xxd-panel-059) | HAND-DRAWN STORYTELLING · CHILDLIKE METAPHOR · WARM PAPER · GENTLE HUMOUR · POETIC ASIDE |
| [xxd-panel-060](https://github.com/nevertoday/xxd-panel-060) | BLACK PRIMARY FORM · IMMENSE NEGATIVE SPACE · HALFTONE DISSOLUTION · ZEN REFLECTION · FRAGMENTS OF THOUGHT |
| [xxd-panel-061](https://github.com/nevertoday/xxd-panel-061) | SELECTIVE MEMORY · 3–6 FRAGMENTS · CUT-PAPER COLOUR · RISOGRAPH · IMPROVISED EDITORIAL LAYOUT |
| [xxd-panel-062](https://github.com/nevertoday/xxd-panel-062) | MINIMAL BLACK LINE · ONE ACCENT COLOUR · CLEVER AWKWARDNESS · PALE PAPER · PROFESSIONAL WHITESPACE |
| [xxd-panel-063](https://github.com/nevertoday/xxd-panel-063) | CORE MASK · PIXEL FORMS · NESTED NEGATIVE SPACE · SUBTLE GLITCH · LIMITED PALETTE |
| [xxd-panel-064](https://github.com/nevertoday/xxd-panel-064) | TORN PAPER · AGED COLLAGE · PENCIL AND INK · TYPEWRITER MICROCOPY · POETIC ARCHIVE |
| [xxd-panel-065](https://github.com/nevertoday/xxd-panel-065) | BLACK STRUCTURE · TWO SOURCE-COLOUR LINES · MISREGISTRATION · VINTAGE PRINT RHYTHM · MICROTYPE |
| [xxd-panel-066](https://github.com/nevertoday/xxd-panel-066) | CHILDLIKE NARRATIVE · AWKWARD BLACK LINE · 3–6 FLAT COLOURS · HEALING PALETTE · HANDWRITTEN OBSERVATION |
| [xxd-panel-067](https://github.com/nevertoday/xxd-panel-067) | FIXED RED–BLUE INK · HAND-DRAWN DUAL INK · CHILDLIKE HUMOUR · EVERYDAY OBSERVATION · PALE PAPER |
| [xxd-panel-068](https://github.com/nevertoday/xxd-panel-068) | CHINESE XIEYI PLACEMENT · WHITE AS INK · INK LINE AND PALE COLOUR · INSCRIPTION TYPE · MODERN EDITORIAL |
| [xxd-panel-069](https://github.com/nevertoday/xxd-panel-069) | BROAD-BRUSH WINDOW · VITAL SOURCE COLOUR · FINE CONTOURS · BOUNDARY CROSSINGS · WARM-WHITE SPACE |
| [xxd-panel-070](https://github.com/nevertoday/xxd-panel-070) | HAND-DRAWN CONTOURS · BRIGHT IMPASTO／TRANSLUCENT COLOUR · MINIATURE SUBJECT · WARM-WHITE SPACE · TYPEWRITER EDITORIAL TYPE |
| [xxd-panel-071](https://github.com/nevertoday/xxd-panel-071) | SOFT PASTEL · PASTEL CRAYON · SOLUBLE PENCIL · NEAR-WHITE PAPER · FLOATING MEMORIES · POETIC HANDWRITING |
| [xxd-panel-072](https://github.com/nevertoday/xxd-panel-072) | TRANSLUCENT FROSTED WINDOWS · REGIONAL SOFT FOCUS · MINIMAL GEOMETRY · RECOGNISABLE SILHOUETTE · MODERN TYPE |
| [xxd-panel-073](https://github.com/nevertoday/xxd-panel-073) | ISOMETRIC MINIATURE ARCHITECTURE · CUT CUBE · CONTINENTAL-SHELF SECTION · RATIONAL SCAFFOLDING · TEXTURED PAPER |
| [xxd-panel-074](https://github.com/nevertoday/xxd-panel-074) | STANDARD ROUNDED SQUARE · FRONT PSEUDO-3D／2.5D · SOURCE-SOUL EXTRACTION · MATTE SCULPTURE · BRAND ICON |
| [xxd-panel-075](https://github.com/nevertoday/xxd-panel-075) | DARK CRAYON · IVORY HANDMADE PAPER · SOFT IRREGULAR FIELD · RISOGRAPH GRAIN · WHITESPACE · PRIVATE TYPEWRITER NOTE |
| [xxd-panel-076](https://github.com/nevertoday/xxd-panel-076) | ROUGH DARK CRAYON · CHARCOAL · BRIGHT MACARON BLOCKS · 45% CONTINUOUS WHITESPACE · NATURAL PAPER · OBSERVATION NOTES |
| [xxd-panel-077](https://github.com/nevertoday/xxd-panel-077) | MINIMAL PAPER SCULPTURE · CLEAR CUT-PAPER CONTOUR · LAYERED PLANES · SOFT SHADOW · HUMANIST MACARON · TRAVEL EDITORIAL |
| [xxd-panel-078](https://github.com/nevertoday/xxd-panel-078) | IVORY COTTON PAPER · DEEP DEBOSS · RECESSED CHAMPAGNE FOIL · FINE-LINE MARK · BLIND PRESSURE · UNDERSTATED LUXURY |
| [xxd-panel-079](https://github.com/nevertoday/xxd-panel-079) | GEOMETRIC STRAIGHTS · FREE ORGANIC CURVES · PEN AND WASH · UNFINISHED QUALITY · BROAD PAPER WHITE · EDITORIAL TYPE |
| [xxd-panel-080](https://github.com/nevertoday/xxd-panel-080) | SOFT ORGANIC GEOMETRY · DIGITAL GOUACHE · CRAYON GRAIN · BOTANICAL COLOUR · SOURCE-BORN METAPHOR · EMOTIONAL SPACE |
| [xxd-panel-081](https://github.com/nevertoday/xxd-panel-081) | EVEN-WEIGHT COLOURED MONOLINE · OPEN CONTOUR · DENSITY HIERARCHY · 2–4 SPOT INKS · RISOGRAPH GRAIN · KEEPSAKE NARRATIVE |
| [xxd-panel-082](https://github.com/nevertoday/xxd-panel-082) | IRREGULAR WATERCOLOUR FIELD · NAÏVE + WONKY · ISOMETRIC／2.5D · CHILDLIKE CONTOUR · VIVID COLOUR · SPATIAL PROTAGONIST |
| [xxd-panel-083](https://github.com/nevertoday/xxd-panel-083) | UGLY-CUTE DOODLE · WONKY TREMBLING CONTOUR · CONTROLLED WRONGNESS · ONE COMIC PROTAGONIST · ROUGH CRAYON · SPARSE-STRANGE-CLUMSY-ACCURATE |
| [xxd-panel-084](https://github.com/nevertoday/xxd-panel-084) | MINIMAL URBAN LINEWORK · GEOMETRIC SCAFFOLD · DENSITY-BASED STIPPLING · LEADING LINES · RESTRAINED COLOUR · POETIC WHITESPACE |
| [xxd-panel-085](https://github.com/nevertoday/xxd-panel-085) | HANDMADE MINIATURE STAGE · COLLECTIBLE DIMENSIONAL COVER · CLAY AND FELT · CUT PAPER AND STRING · MATTE TACTILITY · ARTFUL WHITESPACE |
| [xxd-panel-086](https://github.com/nevertoday/xxd-panel-086) | mid-century modernist limited-colour screen print · silhouette geometry · 2–4 spot inks · dry-brush drag · one focus · generous whitespace |
| [xxd-panel-087](https://github.com/nevertoday/xxd-panel-087) | physical pin-and-string relationship map · vermilion thread · emergent geometry · handwritten notes · research-wall whitespace |
| [xxd-panel-088](https://github.com/nevertoday/xxd-panel-088) | experimental typographic image · text as image · deconstructed type · dot-matrix contour · density gradient · visual poetry |
| [xxd-panel-089](https://github.com/nevertoday/xxd-panel-089) | personal life-journal vignette · one protagonist · a few daily fragments · loose hand line · watercolour and coloured pencil · mature whitespace |
| [xxd-panel-090](https://github.com/nevertoday/xxd-panel-090) | schematic visual thinking map · concept centre · text nodes · geometric scaffold · trajectory arrows · visual notation · generous whitespace |
| [xxd-panel-091](https://github.com/nevertoday/xxd-panel-091) | monochrome blue-pen narrative sketch · cobalt／pen blue／ultramarine／indigo · directional hatching · searching lines · natural paper white |
| [xxd-panel-092](https://github.com/nevertoday/xxd-panel-092) | Expressive pen · loose contours · geometric and scribble hatching · negative-space composition |
| [xxd-panel-093](https://github.com/nevertoday/xxd-panel-093) | Independent original aesthetic · photo-grounded transformation · flexible multi-format delivery |
| [xxd-panel-094](https://github.com/nevertoday/xxd-panel-094) | Fine pen-and-ink · selective solid black · source-derived spot colour · vast negative space · vintage book illustration |
| [xxd-panel-095](https://github.com/nevertoday/xxd-panel-095) | Independent original aesthetic · photo-grounded transformation · flexible multi-format delivery |
| [xxd-panel-096](https://github.com/nevertoday/xxd-panel-096) | Independent original aesthetic · photo-grounded transformation · flexible multi-format delivery |
| [xxd-panel-097](https://github.com/nevertoday/xxd-panel-097) | Mid-century vernacular commercial graphic · schematic line drawing · two-colour spot printing · functional humour |
| [xxd-panel-098](https://github.com/nevertoday/xxd-panel-098) | faux-naïve watercolour picture-book illustration · loose ink line · flat watercolour／gouache · symbolic form · innocent perspective · mature narrative composition |
| [xxd-panel-099](https://github.com/nevertoday/xxd-panel-099) | flat vector brand mascot · bold black contour · rounded geometry · exaggerated proportion · 2–4 branded colours · oversized type background |
| [xxd-panel-100](https://github.com/nevertoday/xxd-panel-100) | naïve folk-inspired flat narrative · primitive forms · simplified silhouettes · flattened perspective · crayon／oil-pastel grain · warm paper · vivid limited colour |
| [xxd-panel-101](https://github.com/nevertoday/xxd-panel-101) | 3×3 memory icons · private-journal feeling · naïve doodles · retro candy colour · handwritten notes |
| [xxd-panel-102](https://github.com/nevertoday/xxd-panel-102) | soothing geometry · soft shapes · flat composition · warm healing colour · easy negative space |
| [xxd-panel-103](https://github.com/nevertoday/xxd-panel-103) | vivid abstract assembly · large colour blocks · abstract disassembly and recombination · bright palette · bold rhythm |
| [xxd-panel-104](https://github.com/nevertoday/xxd-panel-104) | halftone print · coloured linear interventions · one visual centre · contemplative negative space |
| [xxd-panel-105](https://github.com/nevertoday/xxd-panel-105) | intelligent aesthetic selection · one visual centre · poetic minimalist paper collage · monoprint／screen print／Risograph texture · soft limited palette · generous negative space |
| [xxd-panel-106](https://github.com/nevertoday/xxd-panel-106) | pastel pixel memory · 2–4 visual anchors · regular grid · modular colour blocks · local dithering · one visual core · generous negative space |
| [xxd-panel-107](https://github.com/nevertoday/xxd-panel-107) | image-word poetry · readable rebus sentence · modern hand-drawn image words · luminous soft blocks · exact 50:50 pairing · generous whitespace |
| **[xxd-panel-108](https://github.com/nevertoday/xxd-panel-108)** | contemporary folk paper-cut collage · simplified silhouettes · torn edges · vivid source colour · print texture · generous whitespace |
<!-- xxd-panel-catalog:end -->
