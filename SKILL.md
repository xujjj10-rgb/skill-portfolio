---
name: interactive-memory-website
description: Design or refine personal birthday, anniversary, and memory websites using supplied stories, photographs, stickers, gifts, and future wishes. Use for narrative scene planning and interaction implementation; not generic business landing pages or standalone image generation.
---

# Interactive Memory Website

Turn personal material into a coherent, usable experience. The website should convey the relationship through content and interactions rather than through decoration alone.

## Establish the working brief

Read the user's existing project and instructions before proposing a redesign. Inventory available photographs, character sheets, gift images, music and copy. Record which are approved, missing, private or of unknown provenance. Never upload material just to inspect it.

Separate settled decisions from open ones: photograph order, character identity, whether stickers remain static, palette, typography, privacy expectations and publishing scope. A prior request to remove motion remains in effect until the user changes it.

If a decision materially changes the experience, ask a narrow question. Otherwise state a reversible assumption and proceed. Do not invent dates, shared memories or quotations attributed to the people.

## Choose one coherent world

Offer a small number of genuinely different spatial concepts when the user requests a new direction. Changing colors or borders while retaining the same structure is a restyle, not a new concept.

Use a connecting setting when it serves the story: for example, an apartment whose album opens memories and whose globe opens future travel wishes. Do not impose that setting on every project. Distinguish remembered events from imagined future trips.

Before implementation, give a compact palette, type hierarchy, content sequence and interaction plan. If the user requests approval first, show representative static views and wait before implementing that design. Read [references/story-and-assets.md](references/story-and-assets.md) for mapping media into scenes.

## Preserve the media

Keep real photographs large enough to read and uncropped unless the user chooses otherwise. Use object-fit containment where framing is uncertain. Attach decorations to the frame, avoiding faces and important details.

Use the approved identity reference for each character generation; do not use a chain of newly generated faces as the only identity source. Inspect the result, and describe remaining variation honestly. Prefer retaining approved static characters when animation is unnecessary.

Inspect the actual pixel dimensions of sticker sheets. Grid cells may include neighboring art or be irregularly spaced. Specify a source rectangle for each selected sticker, verify edges against a light background, and inspect every used pose. Do not repeatedly conceal contamination with broader CSS masks that also cut off hair or accessories.

Do not flatten the entire experience into an image: keep navigation, labels, controls and state text live, keyboard-accessible elements. Avoid duplicating baked-in image titles with HTML headings.

## Implement interactions with explicit states

Read [references/interaction-states.md](references/interaction-states.md) when implementing albums, gift reveals, or scene navigation. Keep each interaction understandable before adding motion.

Offer pointer, touch and keyboard access to essential actions. A drag or swipe needs a visible button alternative. Make interactive locations discoverable with restrained outlines or labels if their clickability is otherwise ambiguous.

Match the requested implementation scope. Work in a copy when the user asks to preserve the original. A local preview is not authorization to publish, invite collaborators, or change account visibility.

## Verify and deliver

Check the main path with actual UI interactions: entry, album navigation, gift reveal, close/reopen, scene return. Also check rapid inputs, loading failure handling, keyboard focus, reduced motion and phone layout where available. Report unavailable checks as limits, not passes.

Keep large photos and static stickers static when requested. Use transitions to show a user's action; avoid decorative continuous motion. Ensure fixed controls do not obscure content or focus.

Read [references/release-and-privacy.md](references/release-and-privacy.md) before packaging or sharing. Deliver a preview with concise notes about what works, what is still a static mockup, and which copy remains a draft. Do not present an image hotspot prototype as independent 3D object animation.
