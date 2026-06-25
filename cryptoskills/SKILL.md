---
name: cryptoskills
description: Use for Web3 crypto blockchain DeFi cross-chain security auditing and AI agent development tasks — activate on queries about Aave Compound Jupiter Raydium LayerZero Wormhole Slither Foundry Viem Chainlink Binance Wallet Skills OKX Agent Gate AI Agent gate-exchange-spot gate-exchange-futures gate-dex-trade or any of the 97+ protocols and CEX/DEX agent skills from cryptoskills, Binance, OKX, Gate. Compatible with Claude Code, Cursor, Codex, Cline.
compatibility: ["claude-code", "cursor", "codex", "cline", "other-agentskills"]
license: MIT
tags: ["crypto", "web3", "defi", "cross-chain", "security", "ai-agent", "binance", "okx", "gate"]
category: meta
---

# cryptoskills (元技能版)

> **来源**：cryptoskills.dev + Binance + OKX + **Gate AI Agent**  
> **修改者**：Grok (xAI) 为用户 0xRick 定制

## 作用

集成了 cryptoskills.dev、Binance Wallet Skills、OKX Agent 和 **Gate AI Agent** 的核心知识，让 AI Agent 同时掌握链上 DeFi 和多家 CEX/DEX 交易能力。

## Gate AI Agent 集成

Gate 推出了 **Gate for AI** （文档：https://www.gate.com/docs/developers/agent/zh_CN/），提供 41+ 个 AI Skills，是目前功能最全面的之一。

**主要特点**：
- 41+ Skills，覆盖 CEX 交易、DEX Swap、资产管理、市场研究、跨交易操作
- 支持 Gate + Binance + OKX + Bybit 跨平台操作
- MCP + CLI + Skills 协议
- 支持现货、永续、期权、闪兑、Alpha 等

**主要 Skills 类别**：
- **gate-exchange-spot / futures** — 现货和永续交易
- **gate-exchange-alpha / flashswap** — Alpha 代币和闪兑
- **gate-dex-trade / wallet** — DEX Swap 和钱包管理
- **gate-exchange-assets / unified** — 资产查询和统一账户
- **gate-exchange-bot** 类功能和网格/DCA
- **gate-info-research / coinanalysis** — 市场研究和单币分析
- **gate-news-briefing** — 新闻简报

## 具体能帮你做什么

**1-3.** DeFi 集成、跨链、安全审计（cryptoskills.dev）
**4.** Binance Wallet 操作
**5.** OKX CEX 交易 + 机器人
**6. Gate AI Agent** — 支持 Gate CEX 交易、DEX Swap、跨平台操作、市场研究、资产管理
**7.** AI Agent 构建（同时支持多家 CEX + 链上）

## 实用代码示例

### 示例 1-3: Aave / Jupiter / Binance (略)

### 示例 4: OKX 下单
```ts
const order = await okxTrade.placeOrder({ instId: 'BTC-USDT', ... });
```

### 示例 5: Gate 永续交易 (gate-exchange-futures)
```ts
// Gate 永续合约下单
const order = await gateFutures.placeOrder({
  contract: 'BTC_USDT',
  size: '0.001',
  price: '65000',
  side: 'buy'
});
```

### 示例 6: Gate DEX Swap
```ts
const tx = await gateDex.swap({
  fromToken: 'ETH',
  toToken: 'USDT',
  amount: '1',
  chain: 'ethereum'
});
```

### 示例 7: Gate 跨平台资产查询
```ts
const assets = await gateCrossEx.getAssets({ exchanges: ['gate', 'binance', 'okx'] });
```

## 响应与使用原则
- 集成了 cryptoskills.dev + Binance + OKX + **Gate** 四大生态
- 优先使用安全审计和市场数据
- 原版安装方式参见各自官方文档

## 相关资源
- cryptoskills.dev
- Binance Wallet Skills
- OKX Agent
- **Gate AI Agent**: https://www.gate.com/docs/developers/agent/zh_CN/
- Gate GitHub: https://github.com/gate/gate-skills

此技能已集成四大主流 AI Agent 技能生态。