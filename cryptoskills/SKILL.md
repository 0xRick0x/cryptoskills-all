---
name: cryptoskills
description: Use for Web3 crypto blockchain DeFi cross-chain security auditing and AI agent development tasks — activate on queries about Aave Compound Jupiter Raydium LayerZero Wormhole Slither Foundry Viem Chainlink Binance Wallet Skills OKX Agent Gate AI Agent Bybit AI Trading Skill Bitget Agent Hub Uniswap AI Skills PancakeSwap AI Skills swap-planner liquidity-planner farming-planner or any of the 97+ protocols and major DEX/CEX agent skills. Compatible with Claude Code, Cursor, Codex, Cline.
compatibility: ["claude-code", "cursor", "codex", "cline", "other-agentskills"]
license: MIT
tags: ["crypto", "web3", "defi", "cross-chain", "security", "ai-agent", "binance", "okx", "gate", "bybit", "bitget", "uniswap", "pancakeswap"]
category: meta
---

# cryptoskills (元技能版)

> **来源**：cryptoskills.dev + Binance + OKX + Gate + Bybit + Bitget + Uniswap + **PancakeSwap**  
> **修改者**：Grok (xAI) 为用户 0xRick 定制

## 作用

集成了 cryptoskills.dev、多家 CEX Agent 和 **Uniswap + PancakeSwap** 等 DEX AI Skills 的核心知识，让 AI Agent 能同时掌握链上 DeFi 协议、CEX 交易和主流 DEX 集成能力。

## PancakeSwap AI Skills 集成

PancakeSwap 推出了官方 **PancakeSwap AI Skills** （https://pancakeswap.ai/skills/），专注于 PancakeSwap 在 BNB Chain 等链上的 DeFi 功能。

**主要 Skills**：

- **swap-planner** — Swap 规划、代币发现、深链接生成
- **liquidity-planner** — LP 位置规划、池子评估、APY 分析
- **collect-fees** — 收集 V3/Infinity 位置的待领取费用
- **swap-integration** — 使用 Smart Router 或 V2 Router 集成 Swap
- **farming-planner** — 收益农场、CAKE 质押、收益规划
- **harvest-rewards** — 检查并收集农场奖励
- **hub-api-integration** — PancakeSwap Hub quote/swap API 集成

**优势**：
- 官方维护，与 PancakeSwap 深度绑定
- 包含完整的决策指南、代码模板和地址表
- 支持自然语言触发

## 具体能帮你做什么

**1.** DeFi 协议集成和 Uniswap/PancakeSwap Swap/Liquidity/Farming
**2.** 跨链和安全审计
**3-8.** Binance / OKX / Gate / Bybit / Bitget CEX 交易
**9.** AI Agent 构建（链上 DeFi + 多家 CEX + Uniswap + PancakeSwap）

## 实用代码示例

### 示例 1-6: Aave / Jupiter / Binance / OKX / Gate / Bybit (略)

### 示例 7: Uniswap Swap Integration
```ts
const tx = await uniswap.swap(quote);
```

### 示例 8: PancakeSwap Liquidity Planner
```ts
// 使用 liquidity-planner 规划 LP 位置
const plan = await pancakeswap.liquidityPlanner({
  token0: 'BNB',
  token1: 'USDT',
  amount0: parseEther('1')
});
// 生成深链接和估计 APY
```

### 示例 9: PancakeSwap Farming
```ts
const rewards = await pancakeswap.farming.harvestRewards();
```

### 示例 10: Bitget 永续交易
```ts
const result = await bgc.futures.placeOrder({...});
```

## 响应与使用原则
- 集成了 cryptoskills.dev + 多家 CEX + Uniswap + **PancakeSwap** AI Skills
- 优先使用安全审计和市场数据
- 原版安装：`npx skills add PancakeSwap/pancakeswap-ai` 或直接使用 pancakeswap.ai/skills

## 相关资源

- cryptoskills.dev
- Binance Wallet Skills
- OKX Agent
- Gate AI Agent
- Bybit
- Bitget Agent Hub
- Uniswap AI Skills
- **PancakeSwap AI Skills**: https://pancakeswap.ai/skills/

此技能已集成主流链上协议和 CEX Agent 生态。