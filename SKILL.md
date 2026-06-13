---
name: field-service-system-style
description: Apply the Xiaojinglin Daojia user-side mobile UI style guide for field-service, local-life, appointment, city selection, city search, city voting, voting confirmation, and voting success screens. Use when Codex needs to design, generate, review, or refine App or mini-program UI for this field-service system with consistent colors, typography, components, icons, spacing, mobile layout, Figma auto-layout readiness, interaction feedback, or AI UI-generation prompts.
---

# Field Service System Style

Use this skill to keep「小精邻到家」用户端移动端 App / 小程序界面统一、清爽、轻量、亲和、可信赖。

## Workflow

1. Identify the requested page type: city selection, city search, city voting, voting confirmation, voting success, empty state, service list, appointment flow, or another user-side mobile screen.
2. Design only for mobile App / mini-program screens unless the user explicitly asks for another platform.
3. Apply the core foundations before page-specific details: `375×812px`, `#F7F7F7` page background, white cards, green brand accents, `Source Han Sans CN / 思源黑体` typography, 8px cards, capsule primary buttons, and normal line icons.
4. Fit the screen into the target viewport without visible page-level scrollbars. Compress spacing, split dense content into tabs/pages, or use fixed internal panels when content is too long.
5. Keep output editable and componentized for Figma: navigation bar, search box, cards, list items, tags, buttons, bottom panel, dialog, and empty-state illustration should be separable.
6. Account for every meaningful user interaction step. Every clickable control needs visible feedback; async actions need loading, success, failure, and retry paths.
7. Reject conflicting directions such as desktop dashboards, dark technology themes, emoji icons, heavy shadows, large glassmorphism, single-character icon boxes, page-level scrollbars, or unstructured free-floating UI.
8. When writing AI image or UI-generation prompts, include the common constraints and adapt them to the requested page.

## Read References As Needed

- For colors, typography, dimensions, spacing, layout, and auto-layout rules, read [references/visual-foundations.md](references/visual-foundations.md).
- For navigation, backgrounds, cards, search, lists, tags, buttons, bottom panels, data modules, empty states, dialogs, icons, and illustrations, read [references/components.md](references/components.md).
- For city selection, city search, city voting, and voting success screens, read [references/page-patterns.md](references/page-patterns.md).
- For global generation constraints, forbidden styles, and the one-sentence design direction, read [references/generation-constraints.md](references/generation-constraints.md).
- For reusable AI prompt suffixes and example task prompts, read [examples/prompt-snippets.md](examples/prompt-snippets.md).

## Non-Negotiables

- Generate or implement `375×812px` vertical mobile App / mini-program UI by default.
- Use `#F7F7F7` page background, white cards, and green brand accents: `#21B88F`, `#1DC2A5`, `#24D2A3 → #22BEA3`.
- Use `"Source Han Sans CN", "思源黑体", sans-serif`; do not use `Inter`.
- Do not set fixed `line-height`; rely on the font's auto / normal line height.
- Do not use Emoji as icons or decoration.
- Do not use a boxed single Chinese character, random letter, mojibake, or symbol block as a functional icon.
- Do not create page-level scrollbars or content that spills outside the target viewport.
- Make interactions explicit: pressed, loading, disabled, success, failure, retry, confirm, cancel, and return states where relevant.
