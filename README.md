# Robinhood Smart Money Monitor (RBSM)

罗宾汉聪明钱捕手 — 基于 GMGN OpenAPI 的 Robinhood 链聪明钱追踪工具。

## 功能

- **热点代币** — 实时拉取 Robinhood 链 trending tokens，按市值/交易额/聪明钱数排序
- **聪明钱聚合** — 抓取峰值 MC ≥ $1M 代币的 top traders，按盈利分类（早期建仓/离场赢家/当前持仓/当前盈利）
- **代币详情** — 基本信息 + 安全检查 + Top Traders + Smart Money 持仓
- **CSV 导出** — 导出聪明钱钱包列表
- **纯前端** — 无后端，直接调用 GMGN OpenAPI，API Key 存储在浏览器 localStorage

## 使用

1. 打开 GitHub Pages 链接
2. 在顶部输入框填入 GMGN API Key（从 [gmgn.ai](https://gmgn.ai) 获取）
3. 点击「加载代币」或「聚合聪明钱」开始

## 技术栈

- 纯 HTML/CSS/JS，无框架依赖
- GMGN OpenAPI (`openapi.gmgn.ai`)，支持 CORS
- Robinhood 链数据（trending/trenches/token/holders/traders）

## 数据来源

[GMGN.ai](https://gmgn.ai) OpenAPI
