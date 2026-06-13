# Component Rules

Use these component rules after applying [visual-foundations.md](visual-foundations.md).

## Top Navigation

Use an iOS / mini-program-like navigation bar.

- Width: `375px`
- Total top navigation height: about `93px`
- Status bar height: about `51px`
- Center title: 15-16px, Medium, black
- Left side: close or back icon
- Right side: more icon
- Optional bottom divider: 1px, very light
- Background: usually white, or blended with a pale green top atmosphere

Keep the navigation light. Use simple line icons in black or dark gray. Do not add heavy shadows or complex decoration.

## Background Atmosphere

Default page background:

```css
background: #F7F7F7;
```

For city selection and search pages, a subtle top atmosphere may be used:

```css
background:
  linear-gradient(180deg, rgba(211, 255, 246, 0.9) 3%, rgba(245, 245, 245, 0) 46%),
  #F7F7F7;
```

Use the gradient only as a soft atmosphere. Do not use dark tech backgrounds, complex light effects, neon, or large glassmorphism.

## Cards

Cards are the main information container.

```css
background: #FFFFFF;
border-radius: 8px;
padding: 14px 12px;
box-shadow: none;
```

Common values:

- Width: `351px`
- Left and right margin: `12px`
- Radius: `8px`
- Internal spacing: `10-14px`

Card content structure:

```text
Module title 16px Medium #333
↓
Body / list / tags / action entry
```

Separate cards mainly through background, radius, and spacing. Avoid obvious shadows.

## Search Box

Use search boxes for city search and service search.

```css
height: 32px;
background: #FFFFFF;
border-radius: 40px;
padding: 7px 10px;
font-size: 12px;
color: #999999;
```

Structure:

```text
Search icon 12px
Placeholder 12px #999999
```

Use a capsule shape, line icon, and 7-10px outer vertical spacing.

## Lists

Use clean list styling for city lists, search results, and service lists.

```css
font-size: 14px;
font-weight: regular;
color: #333333;
border-bottom: 1px solid rgba(0,0,0,0.04);
padding-bottom: 10px;
```

Rules:

- Letter group labels: `#A9A9A9`, 14px Medium.
- Main row content: `#333333`, 14px Regular.
- State tags: green text with pale green background.
- Filter entries: 12px, `#999999`.
- Keep row rhythm even.
- Keep dividers extremely light.
- Align row content left and state tags right.
- If using a right-side letter index, keep it weak, around 12px.

## Tags

Opened / available tag:

```css
background: rgba(199, 246, 235, 0.20);
color: #1DC2A5;
border-radius: 4px;
padding: 2px 6px;
font-size: 11px;
font-weight: Medium;
```

Use tags only for state. Keep copy short, such as「已开通」「已完成」「待确认」.

## Buttons

### Primary Button

Use for the most important page action:「查看其他城市」「立即投票」「确认提交」.

```css
height: 44px;
border-radius: 82px;
background: linear-gradient(133deg, #24D2A3 5%, #22BEA3 106%);
color: #FFFFFF;
font-size: 14px;
font-weight: Bold;
```

Layout:

- Common width: `335px`
- Horizontal margin: `20px`
- Capsule radius
- Centered text
- No strong shadow

Feedback states:

- Pressed / touched
- Loading
- Success
- Failure
- Disabled

Pressed states may use slight opacity, darker background, small scale change, or subtle shadow. Keep the change restrained.

Loading states must prevent duplicate submission. Disabled states must lower contrast, block clicking, and keep text readable.

### Secondary Button

Use white, light-gray, or weak-outline styling. Text should be `#333333` or `#777777`.

### Action Text

For lightweight actions such as「重新定位」:

```css
font-size: 12px;
font-weight: Medium;
color: #1DC2A5;
```

## Interaction Feedback

Design every meaningful step: input, search, location, selection, submit, confirm, cancel, return, retry, loading, empty result, error, and success.

Every clickable button, icon button, and text button needs feedback. Feedback can be pressed state, loading, toast, dialog, status text, list refresh, disabled button, success page, or error hint.

Network, location, submission, and voting actions require loading and failure retry paths. Destructive or irreversible actions require confirmation. Cancel, return, and close actions still need clear hit areas and immediate response.

## Bottom Action Panel

Use bottom panels for voting, confirmation, and success flows.

- Stick close to the bottom.
- Width: `375px`
- Background: white
- Optional top gradient from pale green to white
- Content padding: `20px`
- Button width: `335px`
- Button height: `44px`
- Preserve iPhone home indicator safe area

The panel should feel like a mobile bottom content area, not a backend modal.

## Data Module

Use for vote count, order count, amount, or other key data.

```css
background: #F7F7F7;
border-radius: 8px;
padding: 30px 0;
```

Number style:

```css
font-family: "Source Han Sans CN", "思源黑体", sans-serif;
font-size: 36px;
font-weight: Bold;
color: linear-gradient(180deg, #24D2A3, #22BEA3);
letter-spacing: -1px to -2px;
```

Text style:

```css
font-size: 13px;
font-weight: Medium;
color: #333333;
```

Numbers are the focus. Very light leaf, sparkle, or soft-shadow details are acceptable only when restrained.

## Empty / Not Opened State

Use for unavailable city, no data, and no search result states.

- Center illustration.
- Low-saturation light gray, pale green, and white.
- Suitable metaphors: map, location pin, box, task, ticket.
- Copy color: `#999999`.
- Keep the illustration moderate in size.

Recommended structure:

```text
Top navigation
↓
Centered light empty-state illustration
↓
Description 13px #999999
↓
Bottom action panel / guide button
```

## Dialog

Use centered dialogs for vote confirmation and important reminders.

```css
width: 300px;
background: #FFFFFF;
border-radius: 8px;
```

Overlay:

```css
background: rgba(0,0,0,0.70);
```

Content:

- Title: 16px Medium, `#333333`, centered or left aligned.
- Body: 13px Regular, `#777777`, using auto / normal line height.
- Bottom button height: about `50px`.
- Two buttons: equal widths with a light divider.
- Confirm button: `#1DC2A5`.

## Icons

- Use line icons.
- Common sizes: 12px, 14px, 16px, 20px, 22px.
- Common colors: `#333333`, `#999999`, `#1DC2A5`.
- Icons should be rounded, light, modern, and recognizable.
- Use normal UI icons such as back, close, search, location, more, check, warning, and arrow.
- Do not use Emoji as icons, button icons, state icons, or decoration.
- Do not use a boxed Chinese character such as「搜」「定」「返」「选」「关」as an icon.
- Do not use mojibake, random letters, single characters, or symbol blocks as icons.
- Keep icon-text spacing stable at `4-6px`.

## Illustrations

- Use light flat or light 3D style.
- Prefer light gray, white, and pale green.
- Use illustrations for empty and success states only as support.
- Success states may use a pale green badge, check mark, sparkle, or small decoration.
- Avoid exaggerated memes, Emoji, and sticker-like cartoon decoration.
