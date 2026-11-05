# Higgsfield-Structured Product Prompt Patterns

Use these examples as structural references, not fixed copy. The final output must still begin with concrete information for the current product and scene.

## Input decisions

1. Read the product identity from Image 1.
2. Read the final composition, environment, light and product endpoint from Image 2.
3. Determine the camera direction and extend the scene in the opposite direction.
4. Choose 4 seconds for a compact move or 5 seconds for a longer reveal.

Use a discrete FOV from the controlling skill. Product tabletop shots normally use `47°`; wider environmental framing may use `63°`.

Use a fixed white balance from `3200K`, `4000K`, `5600K` or `8500K`.

## Camera left, 4 seconds, scene extended to the right

```text
SCENE CONTEXT
A four-second 1:1 product showcase shows a still <product type> inside a continuous <scene type>. The camera travels left from an unseen right-hand extension into the final composition.

ACTIVE REFERENCES
Image 1 is the sole identity reference for <product name, size and package type>. Preserve the package silhouette, closure, material, color, label layout, readable product text and printed artwork as a 100% match to Image 1. Image 2 is the sole reference for the final environment, product endpoint, lighting and end frame. The final frame matches Image 2 exactly.

LOCATION MAP
Foreground: <nearby surface edge and prop>. Midground: <product support and visible objects>. Background: <wall, backdrop, foliage, fabric or architectural layer>. The camera and product share a level axis at the product's mid-body height. Extend the same surface, props, background depth, perspective and contact shadows toward the right side of Image 2, creating one continuous set.

FIRST FRAME / BLOCKING
The camera begins from the right-hand extension. The product enters near the left edge of frame while the whole set remains fixed. The 47° field of view is level with the product center.

FORMAT MODE
One uninterrupted take on a single camera setup, with the camera moving only along the specified horizontal axis.

OPTICS
47° horizontal field of view, rectilinear tabletop perspective, fixed through the shot. The full product height and label remain inside frame at the endpoint.

CAMERA
The camera faces the set from the front and travels left at 0.3 km/h with a steady slider motion. It settles at the Image 2 camera position at approximately 3 seconds and remains stationary for the final second.

ACTION
The camera passes the extended foreground and midground layers, then enters the Image 2 composition. The product remains fixed in world space. A faint shift in leaf, fabric, steam or liquid reflections continues at low amplitude after the camera stops.

PHYSICS
Foreground objects move across frame faster than the background. The product base keeps a stable contact shadow. The package remains rigid. Any droplets, condensation or liquid surface follow gravity and retain their material weight.

LIGHTING
A motivated <window, softbox, daylight or practical source> reaches the set from <direction> at <3200K, 4000K, 5600K or 8500K>. The fill comes from <opposite side or ambient source>. Shadows retain the same direction and density seen in Image 2.

AUDIO
Quiet studio room tone with <one restrained material sound if appropriate>.

STYLE
Photoreal commercial product photography, clear material response, natural motion blur during the move, crisp packaging type and subtle fine grain.

OUTPUT SETTINGS
1:1 aspect ratio, 4 seconds, real-time playback.

POSITIVE LOCKS
Image 1 remains the sole source of package identity and label content. Image 2 remains the target for final composition, product angle, prop placement and light. The final second holds the settled Image 2 frame while the product stays upright, complete and readable.
```

## Camera right, 5 seconds, scene extended to the left

```text
SCENE CONTEXT
A five-second 1:1 product showcase presents a still <product type> in a continuous <scene type>. The camera travels right from an unseen left-hand extension and finishes on the established product composition.

ACTIVE REFERENCES
Image 1 is the sole product reference for <product name, size and package type>. Preserve the exact package form, closure, material, label typography, icons and artwork as a 100% match to Image 1. Image 2 is the sole scene and last-frame reference for the environment, product angle, object placement and lighting.

LOCATION MAP
Foreground: <near object>. Midground: <product support and hero props>. Background: <backdrop and depth layer>. Extend the right-hand edge of Image 2 into a continuous left-hand set that shares the same ground plane, perspective, surface material, prop scale, depth of field and light direction. The camera travels level with the product center.

FIRST FRAME / BLOCKING
The camera starts on the extended left side with the product visible toward the right of frame. The product stays in place while the environment moves through the frame. The 47° field of view remains level and fixed.

FORMAT MODE
One continuous shot with a single rightward lateral move.

OPTICS
47° horizontal field of view, rectilinear product perspective, fixed focal framing. The complete product and centered label remain visible at the endpoint.

CAMERA
The camera faces the scene from the front and moves right at 0.3 km/h on a straight horizontal axis. The move settles at the Image 2 position around 4 seconds and holds there for the final second.

ACTION
The camera crosses the extended props and arrives at the Image 2 arrangement. The product remains stationary. Soft environmental movement continues after the camera stops while the product holds its position and scale.

PHYSICS
Near foreground objects show stronger parallax than the background. The product base maintains a continuous contact shadow. Package seams, rigid edges and label curvature remain stable throughout.

LIGHTING
The main light comes from <direction> at <3200K, 4000K, 5600K or 8500K>, with a soft fill from <fill source>. The final highlight and shadow pattern matches Image 2.

AUDIO
Low studio room tone and a restrained environmental texture support the product finish.

STYLE
Photoreal commercial product film with clean packaging detail, natural parallax and a restrained real-time finish.

OUTPUT SETTINGS
1:1 aspect ratio, 5 seconds, real-time playback.

POSITIVE LOCKS
Image 1 controls the product and all label details. Image 2 controls the final environment and product orientation. The last second holds the established Image 2 composition with the product complete, stable and unobstructed.
```

## Timing

- 4 seconds: the move settles around 3 seconds; approximately 1 second remains for the held end frame.
- 5 seconds: the move settles around 4 seconds; approximately 1 second remains for the held end frame.

Describe the move and hold as one continuous shot. Do not add a cut when the camera reaches Image 2.

## Direction check

- Camera moves left: scene extension is on the right; camera starts on the right.
- Camera moves right: scene extension is on the left; camera starts on the left.
- Camera moves up: scene extension is below; camera starts below.
- Camera moves down: scene extension is above; camera starts above.

The endpoint is always Image 2.

## Final output

- One standalone English prompt.
- One `text` code block.
- After the code block, add a concise Chinese summary of the reference roles, scene extension, camera path, end-frame hold and product locks.
- Return the prompt and summary directly in chat. Create no Markdown, JSON, TXT or other output files.
- Use `Image 1` and `Image 2`; never use `@`.
- Preserve the controlling skill's block order and positive phrasing.
- Include `1:1`, the chosen duration and the final one-second hold.
