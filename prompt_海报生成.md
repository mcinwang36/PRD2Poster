根据 Poster YAML 及参考素材，生成企业级科技产品宣传海报。

---

## 素材定义与优先级

| 优先级 | 素材 | 用途 |
|---|---|---|
| P1 | Poster YAML | 内容基准，所有字段严格遵循 |
| P2 | 参考图2：系统UI截图（可选） | 学习UI结构、页面布局、数据呈现 |
| P3 | 参考图3：业务流程图（可选） | 学习流程关系、场景逻辑、操作路径 |
| P4 | 参考图1：海报风格模板 | 学习排版结构、信息层级、配色、字体、卡片样式、留白节奏 |
| — | 参考图4：品牌Logo（可选） | 品牌标识使用 |

> 参考图1仅学习排版风格，**禁止复制文字内容**。

---

## 版式规划

根据 `visual.poster_type` / `visual.ui_layout` / `visual.image_count` / `visual.image_plan` 自动设计版式，**禁止使用固定模板**。

| ui_layout | 说明 |
|---|---|
| `single_hero` | 1张主视觉 |
| `dual_screen` | 2张页面并列 |
| `workflow` | 流程图 + 关键页面 + 结果页面 |
| `dashboard_grid` | 多个页面组合 |

---

## 图片权重规则

严格遵循 `visual.image_plan`，**禁止平均布局、禁止无主次关系**。

| role | 占比 |
|---|---|
| `hero` | 40%–60%，最大视觉主体 |
| `workflow` | 20%–30%，流程展示 |
| `support` | 10%–20%，辅助页面 |
| `result` | 10%–20%，成果展示 |

---

## 内容区域映射

**标题区**：Logo · `{poster.title}` · `{poster.subtitle}`

**核心展示区**：基于参考图2生成真实业务系统界面
- 系统：`{poster.system_name}`，页面：`{poster.page_name}`，流程：`{poster.workflow}`

**场景卡片**：`{poster.scene.title}` · `{poster.scene.description}` · `{poster.scene.result}`

**价值卡片**：`{poster.value.title}` · `{poster.value.description}`

**能力模块**：展示 `{poster.capabilities}`，采用「图标 + 标题 + 说明」格式

**数据模块**：展示 `{poster.metrics}`，数字最大、说明最小，突出成果价值

**底部**：`{poster.slogan}`

---

## 视觉规则

**颜色**：主色采用 `visual.color_theme`，保持企业级统一设计语言。

**一致性要求**：统一圆角、阴影、留白、字体层级、卡片样式（Lenovo企业级设计语言）。

**允许变化**：主色、辅助色、页面数量、布局结构、业务场景。

**Title vs Slogan**：Title 传递价值主张，Slogan 表达品牌态度，两者必须完全不同，禁止重复或近义改写。

---

## 禁止出现的视觉元素

机器人、机械手、芯片/CPU、地球、未来城市、代码雨、赛博朋克、AI头像、抽象大脑、无意义科技线条。

**必须体现**：真实业务 · 真实场景 · 真实系统 · 真实流程 · 真实价值。

---

## 传播目标

- **3秒**：知道产品是什么
- **5秒**：知道解决什么问题
- **10秒**：知道带来什么价值

整体达到企业正式产品发布海报质量。

---

以下是 Poster YAML：

{{Poster YAML}}
