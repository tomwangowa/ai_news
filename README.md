# AI News Archive

AI 產業新聞存檔與深度分析，由 [Claude Code](https://claude.ai/claude-code) 的 `ai-weekly-insight` skill 自動產出。

## Content Types

| 類型 | 檔名格式 | 頻率 | 說明 |
|------|----------|------|------|
| **Daily Insight** | `[AI-Daily-Insight] <摘要> YYYY-MM-DD` | 每日 | Top 3 新聞，完整三維分析 |
| **Weekly Insight** | `[AI-Weekly-Insight] <摘要> YYYY-MM-DD` | 每週 | Top 5 新聞，完整三維分析 + 四層建議 |
| **News Summary** | `[AINews] <標題> YYYY-MM-DD` | 每日（已停刊） | 早期 AI News mail list 摘要 |

## Analysis Framework

每則新聞均包含三維深度分析，對應 TrendLife AI Taskforce 的四維分享框架：

- 💡 **技術突破** — 核心創新、工程痛點、差異化
- 🚀 **業務影響** — TrendLife 具體應用場景、機會與風險、立即可做 / 短期實驗 / 中期佈局
- ⚖️ **競爭分析** — 巨頭策略、Trend Micro 應採取的立場（compete / collaborate / watch）

## Deduplication

報告產出前會自動掃描近 7 天的歷史報告，避免重複新聞。同一事件的後續重大發展仍可報導，但會標註「延續 [日期] 報導的 [主題]」。

## Workflow

```
觸發（"AI 日報" / "AI 週報"）
  → WebSearch 蒐集候選新聞
  → 去重比對
  → Deep Research（每則 2-5 輪搜尋）
  → 三維分析
  → Executive Summary
  → 寫入 Obsidian
  → 提交到此 repo（或發布 Confluence）
```

## Related

- **Obsidian**: 報告同步存放於 Obsidian vault 的 `AI News` 目錄
- **Confluence**: Weekly Insight 可選擇發布至 TrendLife AI Taskforce 的 Confluence space
- **Skill**: [`~/.claude/skills/ai-weekly-insight/`](https://github.com/tomwangowa/agent-skills/tree/main/ai-weekly-insight)
