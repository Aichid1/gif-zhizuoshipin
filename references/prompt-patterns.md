# Compact Product Prompt Pattern

Use this structure as a fill-in template. Write concrete current-product details, remove every placeholder, and do not copy explanatory text into the prompt.

## Hard limits

- Put the English prompt inside one `text` code block.
- Count every character inside that block, including headings and line breaks, excluding the Markdown fences.
- Keep the English prompt at or below `1990` characters.
- Do not create an `AUDIO` block or mention dialogue, ambience, music, sound effects or silence.
- State each control once. Do not repeat reference roles, product stillness, label readability or end-frame rules in multiple sections.
- Keep product identity, package and label, movement direction, extension side, speed, settle time, FOV, color temperature, aspect ratio, duration and final hold.

## Prompt template

```text
SCENE CONTEXT
A <duration>-second 1:1 showcase of <product> in <scene>. The camera moves <direction> from a continuous <opposite-side> extension into Image 2's final composition.

ACTIVE REFERENCES
Image 1 controls <product identity>: silhouette, closure, material, colors, front proportions, all label text and artwork; exclude its white background, angle and lighting. Image 2 controls the environment, prop layout, product endpoint and orientation, and light.

LOCATION MAP
Foreground: <near prop>. Midground: <support and main objects>. Background: <wall and depth layer>. Continue Image 2's surface, props, perspective, depth and light toward <opposite side>.

FIRST FRAME / BLOCKING
Start on the extended side with the full product near <frame side>, label facing camera and unobstructed. Hold <47/63>° horizontal FOV level with the product center.

FORMAT MODE
One uninterrupted lateral move <direction> on a fixed axis; no cuts.

OPTICS
<47/63>° horizontal FOV, rectilinear fixed framing; full product and label visible at endpoint.

CAMERA
Front-facing, fixed height and speed <speed>, moving <direction>. Settle at Image 2 around <3/4> seconds and hold the final second.

ACTION
The camera crosses the extended foreground and midground into the Image 2 arrangement. The product remains still in world space; environmental motion stays subtle.

PHYSICS
Natural depth parallax, stable contact shadow, rigid package and material-consistent reflections; droplets follow gravity.

LIGHTING
Continue Image 2's key from <direction> at <temperature>, with soft fill and matching shadows.

STYLE
Photoreal commercial product photography, clear materials, natural motion blur during the move, crisp label type and subtle grain.

OUTPUT SETTINGS
1:1, <4/5> seconds, real-time playback.

POSITIVE LOCKS
Image 1 owns package and label identity. Image 2 owns the final frame, orientation and lighting. End with the complete, readable product settled in Image 2.
```

## Direction and timing

| Camera direction | Extend scene toward | Start from |
|---|---|---|
| Left | Image right | Right side |
| Right | Image left | Left side |
| Up | Image bottom | Below |
| Down | Image top | Above |

- 4 seconds: settle around 3 seconds; hold about 1 second.
- 5 seconds: settle around 4 seconds; hold about 1 second.
- The endpoint is always Image 2.
- Product tabletop shots normally use `47°`; wider scenes may use `63°`.

## Compression pass

1. Remove background story, process explanations, empty quality claims and repeated adjectives.
2. Merge related facts into their owning section; do not restate them later.
3. Shorten `LOCATION MAP` and `PHYSICS` before touching product identity, motion, label, lighting or timing.
4. Count the complete English block. Rewrite until `length <= 1990` characters.

## Final output

- One standalone English `text` block at or below 1990 characters, with no `AUDIO`.
- One matching Chinese `text` block with the same headings, order and values. Replace `Image 1` and `Image 2` with “图片1” and “图片2”.
- After both blocks, add a concise Chinese summary of reference roles, extension, camera path, final hold and label lock.
- Never use `@`.
