# Page Patterns

Use these patterns after applying [visual-foundations.md](visual-foundations.md) and [components.md](components.md).

## City Selection Page

Design focus: search entry, current city, city list, and opened-state indicator.

Suggested structure:

```text
iOS top navigation
Search box
Current city card
All cities card
City list
Bottom safe area
```

Requirements:

- Use a subtle pale green top atmosphere.
- Make the current city an independent white card.
- Use a light gray base or pale green icon emphasis for city name tags.
- Use brand green for「重新定位」.
- Use white list cards and very light dividers.

## City Search Page

Design focus: input state, search result list, and loaded-complete hint.

Suggested structure:

```text
Top navigation
Back icon + search input
Search result list
Loaded-complete hint
Bottom safe area
```

Requirements:

- Use a white list container for search results.
- Each result may use a location line icon on the left.
- Result row height should be around `50px`.
- Use very weak gray for「已全部加载」, optionally with short lines on both sides.

## City Voting Page

Design focus: not-opened state, voting guide, vote count, and primary button.

Suggested structure:

```text
Top navigation
Centered empty-state illustration
Not-opened description
Bottom voting panel
Vote count data module
Primary button
Bottom safe area
```

Requirements:

- Use `#F7F7F7` page background.
- Use low-saturation light gray empty-state illustration.
- Use a white bottom panel with subtle pale green top gradient.
- Use green gradient for vote count numbers.
- Use green gradient capsule primary button.

## Voting Success Page

Design focus: success feedback, positive emotion, number emphasis, and next-step guidance.

Suggested structure:

```text
Top navigation
Success illustration / check badge
Success title
Success description
Vote count data card
Primary button: 查看其他城市
```

Requirements:

- Use brand green `#1DC2A5` for the success title.
- Add only restrained success details, such as small sparkles or a green check icon.
- Keep the page simple. Avoid ecommerce-style heavy marketing treatment.
