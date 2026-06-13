# Visual Foundations

Use these rules for every「小精邻到家」user-side mobile App / mini-program screen.

## Design Direction

The interface should feel clean, light, friendly, trustworthy, service-oriented, local-life, and suitable for at-home service workflows.

Prefer a C-end mobile style: white cards, low-saturation gray background, green brand emphasis, rounded components, concise lists, and low-noise hierarchy.

Do not use heavy admin-dashboard styling, strong technology screen styling, dark backgrounds, or complex decorative effects.

## Keywords

- 清爽干净
- 绿色到家服务感
- C 端移动应用
- 轻量卡片化
- 低饱和背景
- 柔和圆角
- 明确信息层级
- 少阴影或无阴影
- 适合小程序 / App 页面
- 适合本地生活、上门服务、城市服务、预约服务类产品

## Color System

### Brand Colors

| Usage | Value | Notes |
|---|---:|---|
| Brand primary | `#21B88F` | Main brand identity and high-level brand scenes |
| Brand secondary | `#1DC2A5` | Frequent emphasis, action text, state tags, positioning, current state |
| Primary button gradient start | `#24D2A3` | Primary buttons, success data, key numbers |
| Primary button gradient end | `#22BEA3` | Primary buttons, success data, key numbers |

### Text Colors

| Usage | Value | Notes |
|---|---:|---|
| Primary title / emphasized text | `#333333` | Page titles, module titles, main list content |
| Secondary body | `#777777` | Explanations and secondary descriptions |
| Weak info | `#999999` | Placeholders, helper text, weak hints, empty-state copy |
| Disabled / index | `#A9A9A9` | Letter indexes, unavailable information |
| Very weak | `#C9C9C9` | Lowest priority hints or disabled text |
| Pure black | `#000000` | iOS navigation title, system icons, status bar |
| White | `#FFFFFF` | Text on primary buttons or brand backgrounds |

### Functional Colors

| Usage | Value | Notes |
|---|---:|---|
| Error / danger | `#F53F3F` | Error, failed states, destructive operations |
| Warning / pending | `#FF7D00` | Warnings, pending states, prompts |
| Success | `#00B42A` | Successful feedback and completed states |

### Backgrounds And Borders

| Usage | Value | Notes |
|---|---:|---|
| Default page background | `#F7F7F7` | Page base and light content background |
| White background | `#FFFFFF` | Cards, search boxes, navigation, dialogs |
| Overlay | `rgba(0,0,0,0.70)` | Dialog masks and modal overlays |
| Card border | `#E5E5E5` | Spec cards; use carefully in product UI |
| Light border | `#DCDCDC` | Weak boundaries on white blocks |
| List divider | `rgba(0,0,0,0.04)` | Row separators |
| Navigation divider | `rgba(0,0,0,0.10)` | Top navigation bottom line |

Use green for key actions and important information only. Do not turn ordinary body text green.

## Typography

Use Chinese sans-serif typography that is modern, clean, and readable.

Required CSS family:

```css
font-family: "Source Han Sans CN", "思源黑体", sans-serif;
```

Rules:

- Use `Source Han Sans CN / 思源黑体` for all page text.
- Do not use `Inter`.
- Do not use `PingFang SC`, `Noto Sans SC`, or other primary fonts unless the user explicitly asks for fallback documentation.
- Use the same font for data numbers, success titles, and marketing titles. Use size, weight, color, and spacing for emphasis instead of introducing another font.
- Do not set fixed `line-height`. Use auto / normal line height.
- When density needs adjustment, tune font size, spacing, container height, and content amount instead of forcing line height.

### Type Scale

| Scene | Size | Weight | Color |
|---|---:|---|---|
| Top navigation title | 15-16px | Medium | `#000000` |
| Module title | 16px | Medium | `#333333` |
| List body | 14px | Regular | `#333333` |
| Description body | 13px | Regular | `#777777` |
| Action text | 12px | Medium | `#1DC2A5` |
| Placeholder | 12px | Regular | `#999999` |
| Tag text | 11px | Medium | `#1DC2A5` |
| Primary button text | 14px | Bold / Medium | `#FFFFFF` |
| Key number | 36px | Bold | Gradient `#24D2A3 → #22BEA3` |

## Canvas And Layout

Default canvas:

```text
375 × 812 px
Vertical phone interface
iPhone / mini-program ratio
```

Do not generate landscape, tablet, desktop, dashboard, or large-screen web layouts unless explicitly requested.

Default content must fully fit the `375×812px` viewport. Avoid page-level scrollbars. When content is too much, reduce visual noise, tighten spacing, group or collapse content, paginate, or split the flow into multiple pages.

### Spacing

| Scene | Value |
|---|---:|
| Page horizontal safe margin | 12px |
| Card horizontal padding | 12-20px |
| Search bar outer margin | 10px left and right |
| Primary button horizontal margin | 20px |
| Bottom panel content padding | 20px |
| Module spacing | 10-14px |
| List item horizontal rhythm | Around 12px |

### Common Page Structure

```text
Status bar / navigation bar
↓
Search bar or core page entry
↓
White card modules
↓
List / state / content area
↓
Bottom safe area or bottom action area
```

Use vertical composition. Avoid complex grids. A common card width is `351px`, leaving `12px` on each side of a `375px` canvas.

## Auto-Layout Rules

- Use a top-to-bottom vertical root structure.
- Keep the root container within the target canvas / viewport height.
- Maintain clear parent-child hierarchy for titles, descriptions, lists, and buttons.
- Reuse consistent spacing, radius, type, and alignment for cards, list items, buttons, tags, and search boxes.
- Keep module vertical spacing stable at around `10-14px`.
- Keep page left and right margins consistent.
- Use horizontal layout inside list rows: main information on the left, status, arrow, or action on the right.
- Make buttons, search boxes, cards, and tags reusable components instead of image-like blocks.
- Pin bottom action areas above the safe area and keep them visually separate from main content.
- For large lists, prefer fixed-height internal panels, pagination, filters, or a "more" entry instead of page-level scrollbars.

Avoid floating text, icons, or buttons; inconsistent card gaps; inconsistent list row heights; broken alignment; and decorative elements that damage reading order.
