# Motion and Continuity

## Scroll as passage

Scroll can unfold an image, reveal an occluded layer, let paper take over a scene, or move through one spatial axis. It does not require illustrated scroll rods. Keep native vertical scrolling for long-form reading; use local horizontal or camera-like motion only when it carries meaning.

## State system

| State | Visitor task | Continuity anchor | Motion constraint |
|---|---|---|---|
| entrance | feel the world and find directions | panorama, display type, chapter mark | one authored sequence; controls available immediately |
| collection | scan and choose | crop family, chapter color, navigation | bounded selection feedback |
| detail opening | know what opened and where it came from | selected image fragment, title, paper relation | shared element or material handoff |
| article middle | read continuously | type roles, paper, contents, quiet chapter cue | no moving, distorted, or parallax prose |
| artwork view | inspect the original | authoritative image, metadata, nearby context | zoom and navigation respect the work |
| return | resume browsing | selected item and scroll position | do not replay the entrance by force |

Expression moves to a different region as the visitor begins reading. It is not a global opacity slider.

## Three continuity mechanisms

### Paper takeover

Reveal a real paper boundary inside the scene, move it across the viewport, and let the stable article surface already exist beneath it. Preserve a chapter mark, crop, color, or coordinate relationship. Never delay content until the animation completes.

### One object changes role

Let a collection image become the detail header, maintaining focal crop and identity. Then reveal the authoritative full artwork or reading content. Never stretch the work for morphing convenience.

### Spatial continuation

Carry an opening, horizon, side wall, or image fragment into the next state while the content surface changes scale. During long reading, confine scenery to a header, margin, or chapter boundary.

## Motion card

For every important transition, record:

- trigger;
- usable start and end states;
- continuous object or relationship;
- occlusion and layer order;
- interruption behavior for fast scroll, reversal, repeated input, and back navigation;
- reduced-motion composition;
- fallback when an image, mask, or script fails.

Initial timing ranges: 100–200ms for control feedback, 180–320ms for routine UI, and 450–800ms for an authored scene handoff. These are project starting points, not standards. Scroll-linked sequences are defined by progress, not by pretending scroll distance is duration.

## Implementation choices

- CSS transitions and keyframes for bounded declarative states.
- View Transitions or an existing shared-element approach when continuity is the purpose; preserve ordinary navigation as fallback.
- A scroll-sequencing library only for a real authored timeline. Pin and scrub are capabilities, not defaults.
- Three-dimensional rendering only when camera, volume, and interactive depth materially matter. Two-dimensional layers or prepared media may be better.
- Do not let multiple motion libraries compete for the same transform, scroll position, or lifecycle.

Keep meaningful content visible before enhancement. Apply masks to enhancement layers because a failed mask asset can make its target disappear. Stop offscreen loops and measure blur, filters, canvas, and shaders on target devices.

## Accessibility and control

- Provide an intentional `prefers-reduced-motion` state that removes large translation, rotation, parallax, and loops while retaining state feedback.
- Automatically moving content lasting more than five seconds beside other content needs pause, stop, or hide control unless essential.
- Preserve Tab, Enter, Space, Escape, browser back, text selection, find, and ordinary links.
- Deep links open articles and artworks without requiring the entrance sequence.
- Removing JavaScript or an image asset must not remove navigation or prose.

Compare the full path with animation disabled first. If the states share only a cream background, continuity is too weak. If the article requires a painting beneath every line, the reading design is underdeveloped.
