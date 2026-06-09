# Field-Service-System-Skills

这是一个用于「小精邻到家」用户端移动端界面设计的 Codex Skill。

它把上门服务、本地生活、城市选择、城市搜索、城市投票、投票确认、投票成功等页面的 UI 风格规范沉淀为可复用的 AI 工作指引，用于让 Codex 或其他 AI 工具在生成、评审、优化页面时保持统一的视觉语言和组件规则。

## Skill 名称

`field-service-system-style`

## 适用场景

- 设计用户端 App / 小程序页面
- 生成 375×812px 移动端 UI 页面
- 统一小精邻到家的颜色、字体、卡片、按钮、标签、图标和布局规范
- 检查 AI 生成页面是否符合移动端自动布局和组件化要求
- 编写可投放到文生图 AI / UI 生成 AI 的页面提示词

## 核心风格

- 浅灰背景：`#F7F7F7`
- 白色卡片承载内容
- 绿色品牌强调：`#21B88F`、`#1DC2A5`
- 主按钮绿色渐变：`#24D2A3 → #22BEA3`
- 轻量、清爽、亲和、可信赖
- 面向 C 端到家服务和本地生活场景
- 页面内容完整适配目标视口，不出现页面级滚动条
- 禁止后台风、暗黑科技风、复杂玻璃拟态、Emoji 图标和不可拆解的整图式 UI

## 仓库结构

```text
.
├── SKILL.md              # Skill 主体说明与完整 UI 规范
├── agents/
│   └── openai.yaml       # Codex Skill 展示元数据
└── README.md             # 仓库说明
```

## 使用方式

把本仓库作为一个 Skill 放到 Codex skills 目录中，或在支持 Skill 的环境里引用本仓库。

示例提示：

```text
Use $field-service-system-style to design a 375x812 mobile city selection screen for 小精邻到家.
```

也可以用于评审页面：

```text
Use $field-service-system-style to review this mobile UI and point out where it breaks the style guide.
```

## 后续维护

主要维护入口是 `SKILL.md`。后续如果增加新的页面类型、组件规范、禁用规则、提示词模板或 Figma 组件化要求，优先更新 `SKILL.md`，再提交到 GitHub。
