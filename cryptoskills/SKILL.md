---
name: cryptoskills
description: Use for Web3 crypto blockchain DeFi cross-chain security auditing and AI agent development tasks — activate on queries about Aave, Jupiter, Binance, OKX, Gate, Bybit, Bitget, Uniswap, PancakeSwap, GMGN, Polymarket or any major on-chain protocol and CEX/DEX/agent skills. Compatible with Claude Code, Cursor, Codex, Cline.
compatibility: ["claude-code", "cursor", "codex", "cline", "other-agentskills"]
license: MIT
tags: ["crypto", "web3", "defi", "cross-chain", "security", "ai-agent", "binance", "okx", "gate", "bybit", "bitget", "uniswap", "pancakeswap", "gmgn", "polymarket"]
category: meta
---

# cryptoskills (元技能版)

> **来源**：cryptoskills.dev + Binance + OKX + Gate + Bybit + Bitget + Uniswap + PancakeSwap + GMGN + Polymarket
> **修改者**：Grok (xAI) 为用户 0xRick 定制

## 作用

集成了主流链上协议、CEX Agent、DEX AI Skills 和预测市场的核心知识，让 AI Agent 能同时掌握 DeFi 协议集成、CEX 交易、DEX 操作、Meme/Smart Money 分析和预测市场交易能力。

## 集成生态概览

| 类别             | 主要生态                              | 核心能力                           |
|---------------------|------------------------------------------------|---------------------------------------------|
| 链上 DeFi 协议 | cryptoskills.dev + Uniswap + PancakeSwap      | Swap、Liquidity、Farming、Hooks          |
| CEX Agent          | Binance + OKX + Gate + Bybit + Bitget         | Spot/Futures/Options + 机器人            |
| Meme / Smart Money | GMGN                                          | Trending、Smart Money、Token Analysis       |
| 预测市场       | Polymarket                                    | 市场查询、持仓分析、交易     |

## 具体能帮你做什么

### 1. 链上 DeFi 协议集成
- Uniswap / PancakeSwap Swap 和 Liquidity 集成
- Aave、Jupiter、Morpho 等借贷、交换、收益管理

### 2. CEX 交易与自动化
- Binance / OKX / Gate / Bybit / Bitget 现货、永续、期权交易
- 网格、DCA、限价单、批量操作

### 3. Meme 币与 Smart Money 分析
- GMGN Trending Tokens、Smart Money 跟踪、KOL 信号
- Token 基础面 + 社交信号 + 链上数据分析

### 4. 预测市场交易
- Polymarket 市场查询、持仓分析、事件交易

### 5. 开发与安全
- Uniswap v4 Hooks 安全审查
- Slither 快速审计、viem/wagmi 集成

## 实用代码示例

### 示例 1: Uniswap / PancakeSwap Swap
```ts
const quote = await uniswap.getQuote({ tokenIn, tokenOut, amountIn });
const tx = await uniswap.executeSwap(quote);
```

### 示例 2: PancakeSwap Liquidity + Farming
```ts
// 创建 LP 位置
const lpTx = await pancakeswap.addLiquidity({ token0, token1, amount0, amount1 });

// 设置农场并收益
const farmTx = await pancakeswap.farming.stake(lpPosition);
const rewards = await pancakeswap.farming.harvest();
```

### 示例 3: CEX 交易（多家通用模式）
```ts
// Binance / OKX / Gate / Bybit / Bitget 均可适用
const order = await exchange.placeOrder({
  symbol: 'BTCUSDT',
  side: 'BUY',
  type: 'MARKET',
  quantity: '0.01'
});
```

### 示例 4: GMGN Smart Money + Trending
```ts
// 获取 trending tokens
const trending = await gmgn.getTrendingTokens({ chain: 'sol', timeframe: '1h' });

// 分析某 token 的 smart money 动向
const analysis = await gmgn.analyzeSmartMoney(tokenAddress);
```

### 示例 5: Polymarket 查询市场 + 下单
```ts
// 查询热门预测市场
const markets = await polymarket.gamma.getMarkets({ limit: 10, order: 'volume' });

// 下单购买某事件
const order = await polymarket.clob.placeOrder({
  market: marketId,
  outcome: 'Yes',
  side: 'BUY',
  price: 0.72,
  size: 50
});
```

### 示例 6: Uniswap v4 Hook 安全审查
```ts
// 使用 v4-security-foundations 审查 Hook 风险
// AI 会自动检查 beforeSwapReturnDelta、afterSwapReturnDelta 等潜在风险
```

## 响应与使用原则
- 优先使用安全审计和市场数据
- CEX 交易前建议先进行安全审计
- 原版安装方式参见各自官方文档

## 相关资源

- cryptoskills.dev
- Binance Wallet Skills
- OKX Agent
- Gate AI Agent
- Bybit
- Bitget Agent Hub
- Uniswap AI Skills
- PancakeSwap AI Skills
- GMGN AI Skills
- Polymarket API: https://docs.polymarket.com/cn/api-reference/introduction

此技能已集成主流链上协议、CEX Agent、DEX Skills 和预测市场生态。