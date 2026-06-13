# Generation Constraints

Use these rules when generating, reviewing, or refining screens.

## AI UI Generation Requirements

1. Generate `375×812px` vertical phone UI.
2. Generate mobile App / mini-program UI only; do not generate web, admin, tablet, desktop, or landscape UI.
3. Fit all content into the target viewport; do not create page-level scrollbars or canvas overflow.
4. Use `#F7F7F7` light gray page background and white cards.
5. Use green as the brand color, prioritizing `#1DC2A5` and `#21B88F`.
6. Use `#24D2A3 → #22BEA3` green gradient for primary buttons.
7. Avoid strong shadows, complex textures, dark technology backgrounds, and large glassmorphism effects.
8. Keep layout clean, breathable, and clearly layered.
9. Keep Chinese copy short and clear. Avoid dense paragraphs.
10. Keep components consistent in radius, spacing, font size, and line-icon style.
11. A subtle pale green atmosphere gradient is allowed, but it must not harm readability.
12. Do not use Emoji in titles, buttons, tags, empty states, success states, icons, or decorations.
13. Use normal UI icons. Do not replace icons with text boxes, single-character boxes, letter boxes, mojibake, or symbol blocks.
14. Follow auto-layout logic with stable spacing and alignment between modules, components, and list rows.
15. Make the result easy to split in Figma into navigation bar, search box, cards, list items, buttons, tags, and bottom action area.
16. Use `Source Han Sans CN / 思源黑体`; do not use `Inter`.
17. Do not set fixed `line-height`; use auto / normal line height.
18. Design feedback states for every button and clickable operation. Async operations must include loading, success, failure, and retry paths.

## Forbidden Directions

- Do not generate backend management systems.
- Do not generate desktop websites, large-screen dashboards, data boards, or tablet layouts.
- Do not create page-level scrollbars.
- Do not use dark blue technology style, neon, cyberpunk, or strong 3D scenes.
- Do not use large areas of black or dark background.
- Do not use complex shadows, heavy outlines, or large glassmorphism cards.
- Do not use brand green for all text.
- Do not make cards overly dense; preserve mobile breathing room.
- Do not make primary buttons blue, purple, or red. Main actions must stay green.
- Do not make illustrations overly realistic or complex.
- Do not generate unreadable text stacks. Copy should be short, clear, and structured.
- Do not use Emoji.
- Do not use a boxed single character as an icon.
- Do not generate image-like UI that cannot be decomposed into reusable components or Figma auto layout.
- Do not let icons, text, and buttons float outside their component containers.
- Do not use `Inter`.
- Do not set fixed `line-height` in CSS, component props, or design annotations.
- Do not leave buttons, icon buttons, text buttons, or key interactions without feedback.

## One-Sentence Direction

This is a C-end at-home service mobile UI system that uses green brand identity, white cards, and light gray page backgrounds to create a clean, friendly, service-oriented experience; every generated page should prioritize mobile ratio, clear hierarchy, soft green emphasis, concise card structure, normal icon expression, and stable auto-layout rhythm.
