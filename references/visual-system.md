# Visual System

## Historical languages and their jobs

| Language | Productive use | Common failure |
|---|---|---|
| Renaissance painting | perspective, human gesture, gaze, foreground–background relationships, credible scale | adding statues and calling the result classical |
| Rococo design | asymmetric S/C curves, natural growth, local virtuosity, lightness against density | mirrored corner flourishes, continuous gold borders, generic palace furniture |
| Baroque and old-master painting | dramatic light and spatial tension when relevant | treating all dark theatrical painting as Renaissance |
| Fashion-editorial historicism | meaningful collision of eras, contemporary interruption, curated strangeness | copying a brand logo, campaign prop, stripe, or product layout |
| Collage and cut paper | real edges, occlusion, scale jumps, material transitions, mutable composition | a sticker pack, global noise overlay, identical torn edges on every card |
| Editorial web typography | navigation, hierarchy, long-form reading, direct interaction | rasterizing text to preserve a look |

Choose a dominant spatial language, then a dominant material handoff. Do not average every influence into one decorative soup.

## Fixed system, variables, residue

**Keep across pages:** type roles, relationship between reading paper and ink, chapter identity, link/focus/return behavior, crop language, edge vocabulary, and at least one spatial or chromatic anchor.

**Allow to vary:** brightness, local palette, scene density, image share, header scale, and chapter motion. Variation follows content rather than switching component-library themes.

**Do not inherit automatically:** source text, brands, signatures, people, dates, exact objects, and exact compositions.

## Composition

- Establish visual weight, eye path, and silhouette at full-viewport scale before refining fibers or ornament.
- A rich screen still needs one primary event: a gesture, object, opening, title, or collision of scale.
- Create density gradients. Let sky, wall, paper, shadow, or low-information image areas support intricate zones.
- Use asymmetry, cropping, off-center balance, and controlled overflow. Avoid equal cards and repeated centered section formulas.
- Align entrances with a visible direction in the scene. Keep labels legible; symbolism does not replace navigation.
- Check horizon, convergence, contact, cast shadow, and focus depth. Surreal violations should look intentional rather than pasted incorrectly.
- Do not force a hero image onto content that has no useful visual source. Type, measure, chapter color, and edge relationships can carry an image-light article.

## Material language

| Material | Preserve | Avoid |
|---|---|---|
| painting or print | different brush/detail densities, pigment layering, original value structure | waxy faces, fake-oil filters, uniform sharpening |
| torn paper | macro contour variation, occasional fibers, exposed paper color, a few pressure points | periodic waves, thick white sticker outline, identical tears, raggedness everywhere |
| cut paper | decisive cut contour, matte color, possible pin or placement evidence | treating every cut edge as torn or using blur as material |
| engraving or metal | sourced curvature, mark structure, coherent contact shadow and light | generic gold gradient, glow outline, embossed controls, plastic bevels |
| paper and ink | stable tone, subtle tooth, restrained ink variation | dirty yellow aging, coffee stains, heavy vignette, animated noise beneath prose |

Attach masks and texture to decorative or image layers. Keep the reading surface stable. Flat print collage and deep pictorial space can coexist, but the scene must establish how light and shadow behave.

## Color and type by role

Define roles from the actual source instead of defaulting to cream, terracotta, and a high-contrast serif:

- `surface-reading`: quiet long-form surface, warm or cool.
- `ink-primary` / `ink-secondary`: tested against the surface and texture.
- `scene-ground`: the environment color of the current chapter.
- `chapter-accent`: a source-derived hue for a key object, word, or state.
- `material-highlight`: paper edge, pigment, or local metal; not automatically the brand color.
- `focus-ring`: unmistakable over light and dark scenery.

Use the fewest type families that can distinguish display, article, and functional UI. Test the real scripts and punctuation. A refined Latin display face does not excuse a mismatched CJK fallback. Avoid decorative script for routine controls and body text.

## Component responsibilities

- `SiteShell`: navigation, chapter state, return behavior, focus, global roles.
- `SceneStage`: immersive image space and authored motion; never the sole copy of content.
- `MaterialBoundary`: visual handoff between scene and reading or gallery surface.
- `CollectionLayout`: scalable browsing and filtering.
- `ArticleLayout`: title, summary, metadata, prose, footnotes, contents, reading settings.
- `ArtworkView`: authoritative work, dimensions, zoom, adjacent works, accessible description.

A component library may provide accessible primitives. Override semantic tokens and a small number of domain components; do not install several complete UI libraries to manufacture personality.

## Failure corrections

| Failure | Correct the mechanism |
|---|---|
| luxury template | remove generic perimeter treatment; re-establish source, focal event, and light |
| sticker collage | let one contour, sightline, or color cross layers; reduce unrelated fragments |
| CSS wave paper | use non-periodic contour, calm segments, and local fiber pressure points |
| abrupt generic inner page | restore shared type roles, crop, chapter mark, edge, and navigation behavior |
| unreadable art-directed prose | quiet the text field and move density to header, margin, or chapter passage |
| tasteful but empty minimalism | enlarge the real work and strengthen one image or typographic event |

