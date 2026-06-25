---
name: cryptoskills
description: Use for Web3 crypto blockchain DeFi cross-chain security auditing and AI agent development tasks — activate on queries about Aave Compound Jupiter Raydium LayerZero Wormhole Slither Foundry Viem Chainlink Binance Wallet Skills OKX Agent okx-cex-trade okx-cex-market grid-bot or any of the 97+ protocols and CEX agent skills. Compatible with Claude Code, Cursor, Codex, Cline.
compatibility: ["claude-code", "cursor", "codex", "cline", "other-agentskills"]
license: MIT
tags: ["crypto", "web3", "defi", "cross-chain", "security", "ai-agent", "binance", "okx"]
category: meta
---

# cryptoskills (元技能版)

> **来源**：https://cryptoskills.dev + Binance Wallet Skills + OKX Agent  
> **修改者**：Grok (xAI) 为用户 0xRick 定制  
> **修改说明**：将 cryptoskills.dev + Binance + OKX 三大生态打包为统一元技能

## 作用

让 AI Agent 快速获得主流区块链协议、**Binance Wallet Skills** 和 **OKX Agent** 的生产级知识，支持 CEX 交易、DeFi 集成、安全审计和自动化策略。

## OKX Agent 集成

OKX 推出了官方 **OKX Agent Trade Kit** （文档：https://www.okx.com/docs-v5/agent_zh/），专为 AI Agent 设计的交易工具包。

**主要 Skills**：

- **okx-cex-market** — 市场数据（实时价格、深度、K线、资金费率等）
- **okx-cex-trade** — 现货、永续合约、交割合约、期权下单、撤单、批量操作、OCO、追踪止损
- **okx-cex-portfolio** — 资产管理、余额查询、持仓、账单
- **okx-cex-bot** — 网格机器人、DCA 策略创建与管理

**优势**：
- 完整支持 OKX CEX 全品种（现货 / 永续 / 期权）
- 本地运行，API Key 不离开设备（更安全）
- 支持 MCP + CLI + Skills 协议
- 开源（MIT）

## 具体能帮你做什么（实用场景）

**1. DeFi 协议集成**  
Aave、Jupiter、Morpho 等集成代码。

**2. 跨链桥接**  
LayerZero、Wormhole 等安全实现。

**3. 智能合约安全审计**  
Slither、Mythril 等审计流程。

**4. Binance Wallet 操作**  
转账、DEX 交换、限价单、安全审计。

**5. OKX CEX 交易与机器人**  
使用 okx-cex-trade 实现现货/永续下单、批量操作、OCO、追踪止损。使用 okx-cex-bot 创建网格和 DCA 机器人。

**6. AI Agent 构建**  
支持 Binance + OKX + 链上操作的自主交易 Agent。

**7. 前端 UX**  
Privy + viem 钱包连接优化。

**8. 市场数据与信号**  
Binance + OKX 市场数据查询、智钱信号。

## 实用代码示例

### 示例 1: Aave v3 Supply
```ts
const hash = await walletClient.writeContract({ address: pool, abi, functionName: 'supply', args: [...] });
```

### 示例 2: Jupiter Swap
```ts
const sig = await agent.swap({ inputMint: 'So1111...', outputMint: 'EPjFW...', amount: 1e9, slippageBps: 50 });
```

### 示例 3: Binance Agentic Wallet Swap
```ts
const res = await baw.swap({ fromToken: 'BNB', toToken: 'USDT', amount: '0.5', slippage: 0.5 });
```

### 示例 4: OKX 现货市价下单 (okx-cex-trade)
```ts
// 使用 OKX Agent 下单
const order = await okxTrade.placeOrder({
  instId: 'BTC-USDT',
  tdMode: 'cash',
  side: 'buy',
  ordType: 'market',
  sz: '0.001'
});
```

### 示例 5: OKX 创建网格机器人 (okx-cex-bot)
```ts
// 创建网格策略
const bot = await okxBot.createGrid({
  instId: 'BTC-USDT',
  algoOrdType: 'grid',
  gridNum: '20',
  runType: '1'
});
```

### 示例 6: OKX 查询市场数据
```ts
const ticker = await okxMarket.getTicker('BTC-USDT');
console.log(ticker.last);
```

### 示例 7: 交易前安全审计
```ts
const audit = await queryTokenAudit(token);
if (audit.riskScore > 70) { /* 警告 */ }
```

## 响应与使用原则

- **生产级模式** + **安全优先** + **多链/CEX 适酌**
- **Binance + OKX** 优先使用安全审计和市场数据
- **原版安装**：`npx cryptoskills install` / `npx skills add binance-web3` / `npx skills add okx/agent-skills`

## 限制

不能替代官方文档。最终代码需经测试和安全审计。

## 相关资源

- cryptoskills.dev
- Binance Wallet Skills
- **OKX Agent**: https://www.okx.com/docs-v5/agent_zh/
- OKX GitHub: https://github.com/okx/agent-skills

此技能已集成 cryptoskills.dev + Binance + OKX 三大生态。