# Desktop and Reading System

## Viewports

Use these as starting checks, not fixed canvases:

| CSS viewport | Check |
|---|---|
| 1440×900 | primary composition, navigation, entrance, content beginning |
| 1920×1080 | image resolution, excessive width, spatial tension |
| 1366×768 | low-height laptop, oversized headers, fixed UI |
| 1280×800 | narrow desktop, rail and measure conflicts |
| 390×844 | secondary responsive fallback, full content and function |

Landscape priority does not mean a fixed 16:9 body. Articles scroll vertically. Portrait artworks keep their ratio. Do not lock prose behind viewport height, snap paging, or `overflow: hidden`.

## Long-form layout

- Let scenery bleed while prose has its own stable maximum measure.
- For Latin prose, begin around 45–75 characters per line. For Chinese, test actual glyphs rather than treating `ch` as one Han character; roughly 32–40 Han characters per line is a useful starting range.
- Ordinary web body text starts around 16px; Chinese editorial reading often benefits from roughly 18–20px and 1.8–1.95 unitless line height. Tune to the actual face and content.
- Low-height viewports should reduce header space or rearrange rails before shrinking body copy.
- Permit local overflow for genuinely two-dimensional tables, formulas, or artwork details; ordinary prose must not cause whole-page horizontal scrolling.

## Chinese and bilingual text

- Mark document and local language accurately, such as English interface with `lang="zh-CN"` on Chinese articles.
- Keep Chinese tracking normal by default; do not imitate luxury Latin wordmarks by spacing every Han character.
- Test line-start and line-end punctuation, quotation marks, book-title marks, ellipses, dashes, numbers, Latin text, footnotes, and long titles.
- Paragraph spacing or first-line indentation should be the primary rhythm; avoid double-marking every paragraph without reason.
- Give quotations, poetry, code, captions, footnotes, and bibliography semantic components.
- Preserve link recognition and focus; color alone is insufficient.
- Validate glyph coverage, punctuation, weights, fallback, and Windows rendering for CJK fonts.

## Content and presentation

Store article structure independently from presentation. Markdown, MDX, or editor JSON are viable choices only after the authoring workflow is understood.

| Content | Template responsibility |
|---|---|
| title, date, kind, tags, summary | consistent title and metadata layout |
| headings, prose, quotes, lists, links, emphasis | semantic HTML and stable role scale |
| images, captions, alt text | responsive sizing, caption relation, loading, zoom |
| footnotes, bibliography, formulas | linkable, reversible, readable rendering |
| artwork and work metadata | fidelity, inspection, separation from decorative crops |

If readers can adjust size, line height, or spacing, those preferences must reflow without rewriting the article. Author emphasis, article-level preset, and reader preference are separate layers.

## Browser and enhancement

- Prioritize current Edge on Windows; check Chrome and Firefox core behavior. Report Safari as untested when no environment is available.
- Record browser, CSS viewport, device scale factor, and page zoom.
- Keep the unenhanced DOM visible. Use feature detection for masks, view transitions, and scroll animation; browser support and asset-load success are separate checks.
- Preserve zoom and user text settings. Test equivalent 320 CSS px reflow for normal content and 200% zoom without loss of function.
- Use at least 4.5:1 contrast for ordinary text and 3:1 for text meeting the large-text definition. Fine type on texture needs visual inspection beyond the numeric ratio.
- Test user text-spacing overrides: 1.5× line height, 2× paragraph spacing, 0.12em letter spacing, and 0.16em word spacing where the language uses those properties.

## Performance and assets

Use Web Vitals as targets: LCP at or below 2.5s, INP at or below 200ms, and CLS at or below 0.1 at the 75th percentile. A laboratory run is not field data.

Define a project asset budget rather than assuming every painting, texture, font, mask, and video belongs in the first request. Give images dimensions and responsive sources; prioritize the critical scene, lazy-load later works, and use a still poster before expensive media.

Maintain an asset ledger: source page, creator/work, permission, local original, dimensions, purpose, focal crop, fidelity status, and chapter. A museum or fashion image that can be viewed online is not automatically available as a site asset.
