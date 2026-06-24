---
name: cryptoskills
description: Use for Web3 crypto blockchain DeFi cross-chain security auditing and AI agent development tasks — activate on queries about Aave Compound Jupiter Raydium LayerZero Wormhole Slither Foundry Viem Chainlink Binance Wallet Skills binance-agentic-wallet query-token-info query-address-info limit-order prediction-market or any of the 97+ protocols and Binance skills. Compatible with Claude Code, Cursor, Codex, Cline.
compatibility: ["claude-code", "cursor", "codex", "cline", "other-agentskills"]
license: MIT
tags: ["crypto", "web3", "defi", "cross-chain", "security", "ai-agent", "binance"]
category: meta
---

# cryptoskills (元技能版)

> **来源**：https://cryptoskills.dev + Binance Wallet Skills  
> **修改者**：Grok (xAI) 为用户 0xRick 定制  
> **修改说明**：将 cryptoskills.dev 97 个协议 + Binance Wallet Skills 打包为单个元技能，增加中文说明、实用场景和代码示例

## 作用

让 AI coding agent 快速获得主流区块链协议和 **Binance Wallet Skills** 的生产级知识，支持钱包操作、DeFi 集成、安全审计、市场信号等场景。

## Binance Wallet Skills 集成

Binance 推出了 **Binance Wallet Skills** （官方文档：https://web3.binance.com/zh-CN/dev-docs/products/wallet-skills/supported-skills），专为 AI Agent 设计的钱包和市场技能模块。

**主要 Skills**：

- **binance-agentic-wallet** — 钱包管理、转账、DEX 交换、限价单、预测市场交易（BSC/ETH/Base/Solana）
- **query-token-info** — 代币信息查询、市场数据、K线
- **query-token-audit** — 代币安全审计（风险评分、蜜罐检测、合约验证）
- **query-address-info** — 钱包持仓查询（代币列表、价格、持仓量）
- **crypto-market-rank** — 市场排行榜（智钱流入、Meme 热度等）
- **meme-rush** — Meme 币追踪与叙事发现
- **trading-signal** — 智钱交易信号

## 具体能帮你做什么（实用场景）

**1. DeFi 协议集成与策略开发**  
帮你快速写出 Aave v3、Morpho、Jupiter、Raydium、Drift、GMX、Hyperliquid 等协议的集成代码（供应、借贷、交换、检杆、收益耕作），并给出仓位管理、清算保护、滑点设置等关键逻辑。

**2. 跨链桥接与互操作**  
提供 LayerZero、Wormhole、Axelar、Hyperlane 的选型对比和安全实现方案，包括跨链消息传递、代币桥接、失败重试机制。

**3. 智能合约安全审计与加固**  
给出 Slither、Mythril、Certora、Echidna 的使用流程和 checklist，帮你检测和修复重入、闪电贷、权限控制等常见漏洞。

**4. Binance Wallet 操作与市场能力**  
结合 binance-agentic-wallet 实现钱包转账、DEX 交换、限价单、预测市场交易等。使用 query-token-audit 进行交易前安全检查。

**5. AI Agent 构建（让 AI 真正上链执行）**  
帮助设计和实现能自主进行链上交易、跨链操作、自动再平衡的 AI Agent 架构（支持 brian-api、coinbase-agentkit、solana-agent-kit 和 binance-agentic-wallet）。

**6. 前端与用户体验优化**  
使用 Privy + viem/wagmi 实现钱包连接、交易策名、错误友好提示、gas 估算和移动端适酌的最佳实践。

**7. 预言机与基础设施**  
Chainlink、Pyth 等预言机的安全集成方式（防操纵、置信区间判断）仨及自动化 keeper 使用。

**8. NFT 与代币发行**  
ERC-721/1155 铸造、元数据管理、版税设置，以及 Solana Metaplex 压缩 NFT 的高效方案。

**9. 交易与市场分析工具**  
Polymarket、永续合约订单路由、链上聪明钱分析等工具的集成思路。

## 实用代码示例

### 示例 1: Aave v3 Supply (viem)

```ts
const hash = await walletClient.writeContract({
  address: '0x87870Bca3F3fD6335C3afA6d2a3B0e2E8e5e5e5e',
  abi: aavePoolAbi,
  functionName: 'supply',
  args: [usdcAddress, parseUnits('1000', 6), userAddress, 0]
});
```

### 示例 2: Jupiter Swap (Solana)

```ts
const signature = await agent.swap({
  inputMint: 'So11111111111111111111111111111111111111112',
  outputMint: 'EPjFWdd5AufqSSqeM2qN1xzybapC8G4wEGGkZwyTDt1v',
  amount: 1_000_000_000,
  slippageBps: 50
});
```

### 示例 3: Binance Agentic Wallet - Market Swap

```ts
// Binance Agentic Wallet 执行市价交换
const result = await baw.swap({
  fromToken: 'BNB',
  toToken: 'USDT',
  amount: '0.5',
  slippage: 0.5
});
console.log(result.txHash);
```

### 示例 4: Binance Agentic Wallet - Limit Order

```ts
// 创建限价单
const order = await baw.createLimitOrder({
  fromToken: 'BNB',
  toToken: 'USDT',
  amount: '1',
  price: '580',
  side: 'sell'
});
```

### 示例 5: 交易前安全审计 (query-token-audit)

```ts
// 交易前先审计代币
const audit = await queryTokenAudit('0x...tokenAddress');
if (audit.riskScore > 70) {
  console.log('High risk token, do not trade');
}
```

### 示例 6: 查询钱包持仓 (query-address-info)

```ts
const portfolio = await queryAddressInfo('0xYourAddress');
console.log(portfolio.totalValueUSD);
console.log(portfolio.tokens);
```

### 示例 7: Slither 快速审计

```bash
slither . --detect reentrancy
```

## 响应与使用原则

- **提供生产级模式**：包括推荐的 SDK、常见代码结构、滑点保护、模拟执行。
- **安全优先**：始终强调重入攻击防护、权限控制、最小权限原则、交易模拟和正式审计建议。
- **多链适酌**：根据目标链给出针对性建议。
- **Binance Skills** 优先使用安全审计和市场数据能力。
- **原版 Skills 推荐**：`npx cryptoskills install <name>` 或 `npx skills add binance-web3`

## 限制与最佳实践

此技能提供结构化知识和经过验证的模式，但不能替代官方文档。最终代码必经测试和安全审计后部署。

## 相关资源

- cryptoskills.dev: https://cryptoskills.dev
- Binance Wallet Skills: https://web3.binance.com/zh-CN/dev-docs/products/wallet-skills/supported-skills
- Binance Skills Hub: https://github.com/binance/binance-skills-hub

此技能已将 cryptoskills.dev 与 Binance Wallet Skills 的核心知识打包整合，方便在各种 Web3 场景中快速调用。