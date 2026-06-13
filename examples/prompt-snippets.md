# Prompt Snippets

Use these snippets when writing prompts for AI image or UI generation tools.

## Common Suffix

```text
请严格生成 375×812px 的用户端移动端 App / 小程序 UI 页面，所有内容必须完整适配当前画板 / 视口，不要出现页面级滚动条或画板外溢出内容。页面整体使用浅灰背景、白色卡片、绿色品牌强调色，保持清爽、轻量、亲和的 C 端到家服务风格。页面必须使用 Source Han Sans CN / 思源黑体，禁止使用 Inter 字体。禁止设置 line-height / 行高，只使用字体自身的 auto / normal 行高。页面必须符合自动布局逻辑，模块层级清晰，组件间距统一，便于后续在 Figma 中拆分为导航栏、搜索框、卡片、列表项、按钮、标签和底部操作区。每一个按钮和可点击操作都必须有明确反馈状态，异步操作必须包含 loading、成功、失败和重试路径。页面中禁止出现 Emoji 表情。所有图标必须是正常、清晰、可识别的 UI 图标，不要使用方框加单字、字母、乱码或符号块代替图标。不要生成后台、网页、大屏、平板、暗黑科技风或复杂玻璃拟态效果。
```

## City Selection Prompt

```text
Use $field-service-system-style to design a 375×812 mobile city selection screen for 小精邻到家. Include top navigation, capsule search box, current city card, all cities card, city list with opened tags, and a subtle pale green top atmosphere. Apply the common suffix constraints.
```

## City Search Prompt

```text
Use $field-service-system-style to design a 375×812 mobile city search screen for 小精邻到家. Include a top navigation row with back icon and search input, search result list rows with location line icons, a weak loaded-complete hint, and bottom safe area. Apply the common suffix constraints.
```

## City Voting Prompt

```text
Use $field-service-system-style to design a 375×812 city voting screen for a not-yet-opened service city. Include an empty-state illustration, short unavailable-city copy, bottom voting panel, vote count data module, and green gradient capsule primary button. Apply the common suffix constraints.
```

## Review Prompt

```text
Use $field-service-system-style to review this mobile UI. Point out where it breaks the style guide, especially viewport fit, typography, colors, cards, icons, scrollbars, auto-layout readiness, and interaction feedback states.
```
