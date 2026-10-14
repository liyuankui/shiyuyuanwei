# PostHog Analytics · shiyuyuanwei（事与愿违）

Project property: `shiyuyuanwei` · EU ingest · 注册表：`~/Notebooks/context/prompt/POSTHOG_USAGE_GUIDE.md`

| 事件 | 属性 | 触发 |
|------|------|------|
| `page_view` | `ref` · `sport`（bd/pb/tt） | 页面加载 |
| `sport_switch` | `to` | 切换运动 tab |
| `nav_click` | `to`（matrix/theory/test） | 导航锚点 |
| `share_copy` | — | 复制分享文案 |
| `swipe_open` | `cards` | 开始残留自测 |
| `swipe_card` | `card_id`, `card`, `sport`, `verdict`（hit/clean） | 每张陷阱卡滑定 |
| `swipe_done` | `sport`, `hit`, `total`, `rank` | 完成自测 |
| `swipe_share` | `hit`, `total`, `rank` | 复制战报 |

分析口径：`swipe_card` 按 `card` 聚合＝哪条反直觉陷阱最普遍被踩（内容热度榜，指导后续运动选坑）。
