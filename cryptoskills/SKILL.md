---
name: cryptoskills
description: Use for Web3 crypto blockchain DeFi cross-chain security auditing and AI agent development tasks — activate on queries about Aave Compound Jupiter Raydium LayerZero Wormhole Slither Foundry Viem Chainlink Binance Wallet Skills OKX Agent Gate AI Agent Bybit AI Trading Skill Bitget Agent Hub Uniswap AI Skills swap-integration liquidity-planner v4-hooks or any of the 97+ protocols and major CEX/DEX agent skills. Compatible with Claude Code, Cursor, Codex, Cline.
compatibility: ["claude-code", "cursor", "codex", "cline", "other-agentskills"]
license: MIT
tags: ["crypto", "web3", "defi", "cross-chain", "security", "ai-agent", "binance", "okx", "gate", "bybit", "bitget", "uniswap"]
category: meta
---

# cryptoskills (元技能版)

> **来源**：cryptoskills.dev + Binance + OKX + Gate + Bybit + Bitget + **Uniswap**  
> **修改者**：Grok (xAI) 为用户 0xRick 定制

## 作用

集成了 cryptoskills.dev、多家 CEX Agent 和 **Uniswap AI Skills** 的核心知识，让 AI Agent 能同时掌握链上 DeFi 协议、CEX 交易和 Uniswap v3/v4 集成能力。

## Uniswap AI Skills 集成

Uniswap 推出了官方 **Uniswap AI Skills** （https://developers.uniswap.org/docs/uniswap-ai/skills），专注于 Uniswap 协议的 AI Agent 开发和集成。

**主要 Skills**：

- **swap-integration** — 使用 Uniswap API、Universal Router 或直接合约集成 Swap
- **liquidity-planner** — 规划 LP 位置并生成接口深链接
- **v4-security-foundations** — Uniswap v4 Hooks 安全风险审查
- **viem-integration** — viem + wagmi EVM 客户端集成
- **pay-with-any-token** — 使用 Uniswap Swap 支付 x402 / HTTP 402

**优势**：
- 官方维护，与 Uniswap v3/v4 深度绑定
- 支持开发者构建 dApp 和 AI 交易代理
- 可以通过 `npx skills add Uniswap/uniswap-ai` 安装

## 具体能帮你做什么

**1.** DeFi 协议集成和 Uniswap Swap/Liquidity 开发
**2.** 跨链和安全审计
**3-8.** Binance / OKX / Gate / Bybit / Bitget CEX 交易
**9.** AI Agent 构建（链上 + 多家 CEX + Uniswap v4 Hooks）

## 实用代码示例

### 示例 1-6: Aave / Jupiter / Binance / OKX / Gate / Bybit (略)

### 示例 7: Uniswap Swap Integration
```ts
// 使用 Uniswap Universal Router 或 API 执行 Swap
const quote = await uniswap.quote({
  tokenIn: 'ETH',
  tokenOut: 'USDC',
  amountIn: parseEther('1')
});

const tx = await uniswap.swap(quote);
```

### 示例 8: Uniswap v4 Hook Security Review
```ts
// 使用 v4-security-foundations 审查 Hook
// AI 会自动检查 beforeSwapReturnDelta 等风险点
```

### 示例 9: Bitget 永续交易
```ts
const result = await bgc.futures.placeOrder({...});
```

## 响应与使用原则
- 集成了 cryptoskills.dev + 多家 CEX + **Uniswap AI Skills**
- 优先使用安全审计和市场数据
- 原版安装：`npx skills add Uniswap/uniswap-ai`

## 相关资源

- cryptoskills.dev
- Binance Wallet Skills
- OKX Agent
- Gate AI Agent
- Bybit
- Bitget Agent Hub
- **Uniswap AI Skills**: https://developers.uniswap.org/docs/uniswap-ai/skills

此技能已集成主流链上协议和 CEX Agent 生态。