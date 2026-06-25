---
name: cryptoskills
description: Use for Web3 crypto blockchain DeFi cross-chain security auditing and AI agent development tasks — activate on queries about Aave Compound Jupiter Raydium LayerZero Wormhole Slither Foundry Viem Chainlink Binance Wallet Skills OKX Agent Gate AI Agent Bybit AI Trading Skill bybit-trading bybit-official-trading-server or any of the 97+ protocols and major CEX agent skills. Compatible with Claude Code, Cursor, Codex, Cline.
compatibility: ["claude-code", "cursor", "codex", "cline", "other-agentskills"]
license: MIT
tags: ["crypto", "web3", "defi", "cross-chain", "security", "ai-agent", "binance", "okx", "gate", "bybit"]
category: meta
---

# cryptoskills (元技能版)

> **来源**：cryptoskills.dev + Binance + OKX + Gate + **Bybit**  
> **修改者**：Grok (xAI) 为用户 0xRick 定制

## 作用

集成了 cryptoskills.dev、Binance、OKX、Gate 和 **Bybit** 的核心知识，让 AI Agent 能同时掌握链上 DeFi 和多家主流 CEX 交易能力。

## Bybit AI Trading Skill & MCP Server 集成

Bybit 推出了官方 **Bybit AI Trading Skill** （https://github.com/bybit-exchange/skills） 和 **bybit-official-trading-server** MCP Server。

**主要特点**：
- 支持 Spot、Linear Perpetual、Inverse Contracts、Options、Earn
- 提供 bybit-trading Skill（Skills 协议）
- 官方 MCP Server（bybit-official-trading-server）
- 支持自然语言交易和市场查询
- 安全机制（交易前确认、权限控制）

## 具体能帮你做什么

**1-3.** DeFi 集成、跨链、安全审计
**4.** Binance Wallet 操作
**5.** OKX CEX 交易 + 机器人
**6.** Gate AI Agent（CEX + DEX + 跨平台）
**7. Bybit** — Spot / Perpetual / Options 交易、市场数据、仓位管理

## 实用代码示例

### 示例 1-4: Aave / Jupiter / Binance / OKX (略)

### 示例 5: Gate 永续交易
```ts
const order = await gateFutures.placeOrder({...});
```

### 示例 6: Bybit 永续合约下单 (bybit-trading)
```ts
// Bybit AI Trading Skill 下单
const order = await bybitTrade.placeOrder({
  symbol: 'BTCUSDT',
  side: 'Buy',
  orderType: 'Market',
  qty: '0.001'
});
```

### 示例 7: Bybit 查询市场和仓位
```ts
const ticker = await bybitMarket.getTicker('BTCUSDT');
const positions = await bybitAccount.getPositions();
```

## 响应与使用原则
- 集成了 cryptoskills.dev + Binance + OKX + Gate + **Bybit** 五大生态
- 优先使用安全审计和市场数据
- 原版安装：`npx skills add bybit-exchange/skills` 或 `npx bybit-official-trading-server@latest`

## 相关资源

- cryptoskills.dev
- Binance Wallet Skills
- OKX Agent
- Gate AI Agent
- **Bybit AI Trading Skill**: https://github.com/bybit-exchange/skills
- Bybit MCP Server: https://www.npmjs.com/package/bybit-official-trading-server

此技能已集成五大主流 AI Agent 技能生态。