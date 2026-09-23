# AyayaUsage

Claude Code 每日花费、token 与 5 小时 / 7 天额度用量：https://ayaya114514.github.io/AyayaUsage/

`data.json` 由本机 `~/.claude/scripts/cc_cost.py publish` 生成：每次 Claude Code 会话结束
（SessionEnd hook）后在后台汇总 transcript 与 statusline 的 `rate_limits`，commit 并 push。
只发布每日聚合，不含项目名、路径和 session id。

- 花费是按 API 价格折算的等价值，不是订阅的实际账单。
- 额度是账号级百分比（整数），同时段其他客户端的消耗也会计入。
