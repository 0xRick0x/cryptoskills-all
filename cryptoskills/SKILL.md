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

### 示例 5: GMGN 信号 + CEX/DEX 执行（组合用法）
```ts
// 1. 获取 GMGN smart money 信号
const signal = await gmgn.getSmartMoneyBuys({ chain: 'sol' });

// 2. 在 CEX 或 DEX 上执行交易
const tx = await exchange.placeOrder({
  symbol: signal.token + 'USDT',
  side: 'BUY',
  type: 'MARKET'
});
```

### 示例 6: Polymarket 查询市场 + 下单
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

### 示例 7: Uniswap v4 Hook 安全审查
```ts
// 使用 v4-security-foundations 审查 Hook 风险
// AI 会自动检查 beforeSwapReturnDelta、afterSwapReturnDelta 等潜在风险
```

## 常见组合用法（高级场景）

### 组合 1: GMGN Smart Money 信号 → CEX/DEX 执行
```ts
// 获取 GMGN smart money 买入信号
const signals = await gmgn.getSmartMoneyBuys({ chain: 'sol', minAmount: 10000 });

// 选择信号最强的 token 并执行交易
const bestToken = signals[0].token;
const tx = await exchange.placeOrder({
  symbol: bestToken + 'USDT',
  side: 'BUY',
  type: 'MARKET'
});
```

### 组合 2: Polymarket 事件分析 → CEX 对冲
```ts
// 1. 分析 Polymarket 事件
const event = await polymarket.gamma.getEvent(eventId);

// 2. 如果判断有利润空间，在 CEX 上对冲
const hedgeOrder = await exchange.placeOrder({
  symbol: relatedAsset + 'USDT',
  side: 'SELL',
  type: 'MARKET'
});
```

### 组合 3: GMGN Meme 币分析 → PancakeSwap/Uniswap 流动性提供
```ts
// 1. 使用 GMGN 分析 hot meme token
const tokenInfo = await gmgn.analyzeToken(tokenAddress);

// 2. 如果质量合格，在 PancakeSwap/Uniswap 上提供流动性
const lpTx = await pancakeswap.addLiquidity({
  token0: 'WBNB',
  token1: tokenAddress,
  amount0: parseEther('0.5')
});
```

### 组合 4: Polymarket 事件交易 → CEX 对冲对冲（高级风险管理）
```ts
// 1. 在 Polymarket 上下注某事件
const pmOrder = await polymarket.clob.placeOrder({ market, outcome: 'Yes', ... });

// 2. 监控 Polymarket 价格变化，并在 CEX 上对冲对冲
const cexHedge = await exchange.placeOrder({
  symbol: correlatedAsset,
  side: 'SELL',
  type: 'MARKET'
});
```

### 组合 5: 多 CEX 价差套利 + On-chain 对冲
```ts
// 1. 监控多家 CEX 价差
const prices = await multiExchange.getPrices('BTCUSDT');

// 2. 在价差最大的交易所执行
const arbTx = await bestExchange.placeOrder({...});

// 3. 可选：在 DEX 上对冲对冲冲
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