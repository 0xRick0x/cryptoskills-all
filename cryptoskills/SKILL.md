---
name: cryptoskills
description: Use for Web3 crypto blockchain DeFi cross-chain security auditing and AI agent development tasks — activate on queries about Aave Compound Jupiter Raydium LayerZero Wormhole Slither Foundry Viem Chainlink Binance Wallet Skills OKX Agent Gate AI Agent Bybit AI Trading Skill Bitget Agent Hub Uniswap AI Skills PancakeSwap AI Skills GMGN AI Skills gmgn-token gmgn-market trending-tokens smart-money or any of the 97+ protocols and major DEX/CEX/agent skills. Compatible with Claude Code, Cursor, Codex, Cline.
compatibility: ["claude-code", "cursor", "codex", "cline", "other-agentskills"]
license: MIT
tags: ["crypto", "web3", "defi", "cross-chain", "security", "ai-agent", "binance", "okx", "gate", "bybit", "bitget", "uniswap", "pancakeswap", "gmgn"]
category: meta
---

# cryptoskills (元技能版)

> **来源**：cryptoskills.dev + Binance + OKX + Gate + Bybit + Bitget + Uniswap + PancakeSwap + **GMGN**  
> **修改者**：Grok (xAI) 为用户 0xRick 定制

## 作用

集成了 cryptoskills.dev、多家 CEX Agent 和多个 DEX AI Skills 和 **GMGN AI Skills** 的核心知识，让 AI Agent 能同时掌握链上 DeFi、CEX 交易、DEX 集成和 Solana Meme/Smart Money 分析能力。

## GMGN AI Skills 集成

GMGN 推出了 **GMGN OpenAPI Skills** （https://github.com/GMGNAI/gmgn-skills），专注于 Solana 和多链 Meme 币、Smart Money 追踪、市场分析和交易。

**主要特点**：
- 实时 trending tokens、smart money 跟踪、KOL 信号
- Token 基础面、社交信号、链上数据分析
- 支持 Solana、BSC、Base 等多链
- 提供 gmgn-token、gmgn-market 等 Skills
- 适配 AI Agent 进行 Meme 币筛选和交易决策

## 具体能帮你做什么

**1.** DeFi 协议集成和 Uniswap/PancakeSwap Swap/Liquidity/Farming
**2.** 跨链和安全审计
**3-8.** Binance / OKX / Gate / Bybit / Bitget CEX 交易
**9.** GMGN AI Skills — Solana Meme 币、Smart Money 跟踪、Trending Tokens 分析
**10.** AI Agent 构建（链上 DeFi + 多家 CEX + 多个 DEX + Meme/Smart Money）

## 实用代码示例

### 示例 1-7: Aave / Jupiter / Binance / OKX / Gate / Bybit / Uniswap (略)

### 示例 8: PancakeSwap Liquidity Planner
```ts
const plan = await pancakeswap.liquidityPlanner({...});
```

### 示例 9: GMGN Trending Tokens + Smart Money
```ts
// 使用 GMGN Skills 查询 trending tokens
const trending = await gmgn.getTrendingTokens({
  chain: 'sol',
  timeWindow: '1h',
  filter: 'pump.fun'
});
// 分析 smart money 动向
```

### 示例 10: GMGN Token Analysis
```ts
// 查询单个 token 的基础面、社交信号和 smart money 买入
const analysis = await gmgn.analyzeToken('tokenAddress');
```

## 响应与使用原则
- 集成了 cryptoskills.dev + 多家 CEX + Uniswap + PancakeSwap + **GMGN**
- 优先使用安全审计和市场数据
- 原版安装：`npx skills add GMGNAI/gmgn-skills`

## 相关资源

- cryptoskills.dev
- Binance Wallet Skills
- OKX Agent
- Gate AI Agent
- Bybit
- Bitget Agent Hub
- Uniswap AI Skills
- PancakeSwap AI Skills
- **GMGN AI Skills**: https://github.com/GMGNAI/gmgn-skills

此技能已集成主流链上协议、CEX Agent 和 Meme/Smart Money 生态。