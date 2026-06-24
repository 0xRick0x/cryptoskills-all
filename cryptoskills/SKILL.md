---
name: cryptoskills
description: Use for Web3 crypto blockchain DeFi cross-chain security auditing and AI agent development tasks — activate on queries about Aave Compound Jupiter Raydium LayerZero Wormhole Slither Foundry Viem Chainlink or any of the 97 protocols in cryptoskills.dev across 15 chains. Compatible with Claude Code, Cursor, Codex, Cline and other agentskills.io compliant tools.
compatibility: ["claude-code", "cursor", "codex", "cline", "other-agentskills"]
license: MIT
tags: ["crypto", "web3", "defi", "cross-chain", "security", "ai-agent"]
category: meta
---

# cryptoskills (元技能版)

> **来源**：https://cryptoskills.dev (原始项目： kukapay/crypto-skills)  
> **修改者**：Grok (xAI) 为用户 0xRick 定制  
> **修改说明**：将原 97 个独立 skills 打包为单个元技能，增加中文说明 + 具体实用场景 + 兼容更多 AI coding agent（Claude Code、Cursor、Codex、Cline 等）

## 作用

让各种 AI coding agent（Claude Code、Cursor、Codex 等）快速获得主流区块链协议的**生产级知识**，无需每次都从零学习协议细节、SDK 使用方式、安全模式和常见坑。从而大幅提升开发 DeFi、跨链、合约审计、AI 交易代理等 Web3 项目的效率和准确性。

## 具体能帮你做什么（实用场景）

**1. DeFi 协议集成与策略开发**  
帮你快速写出 Aave v3、Morpho、Jupiter、Raydium、Drift、GMX、Hyperliquid 等协议的集成代码（供应、借贷、交换、检杆、收益耕作），并给出仓位管理、清算保护、滑点设置等关键逻辑。

**2. 跨链桥接与互操作**  
提供 LayerZero、Wormhole、Axelar、Hyperlane 的选型对比和安全实现方案，包括跨链消息传递、代币桥接、失败重试机制。

**3. 智能合约安全审计与加固**  
给出 Slither、Mythril、Certora、Echidna 的使用流程和 checklist，帮你检测和修复重入、闪电贷、权限控制等常见漏洞。

**4. 智能合约开发与多链部署**  
推荐 Foundry、Hardhat、viem、solana-kit 等工具链的最佳实践，并提供 Arbitrum、Base、Optimism、Solana 等多链部署方案。

**5. AI Agent 构建（让 AI 真正上链执行）**  
帮助设计和实现能自主进行链上交易、跨链操作、自动再平衡的 AI Agent 架构（支持 brian-api、coinbase-agentkit、solana-agent-kit 等）。

**6. 前端与用户体验优化**  
使用 Privy + viem/wagmi 实现钱包连接、交易策名、错误友好提示、gas 估算和移动端适酌的最佳实践。

**7. 预言机与基础设施**  
Chainlink、Pyth 等预言机的安全集成方式（防操纵、置信区间判断）以及自动化 keeper 使用。

**8. NFT 与代币发行**  
ERC-721/1155 铸造、元数据管理、版税设置，以及 Solana Metaplex 压缩 NFT 的高效方案。

**9. 交易与市场分析工具**  
Polymarket、永续合约订单路由、链上聪明钱分析等工具的集成思路。

## 响应与使用原则

- **提供生产级模式**：包括推荐的 SDK（优先 viem、ethers.js、Solana web3.js 等）、常见代码结构、滑点/截止时间保护、模拟交易后再执行。
- **安全优先**：始终强调重入攻击防护、权限控制、最小权限原则、交易模拟和正式审计建议。
- **多链适酌**：根捧你的目标链（EVM vs Solana vs Aptos 等）给出针对性 SDK 和 gas 策略。
- **常见误区纠正**：主动指出开发者常犯的错误（如硬编码地址、忽略事件监听、缺少错误处理）。
- **原版 Skills 推荐**：如果用户想在自己的 Claude Code、Cursor、Cline 等工具中直接使用这些 skills，建议运行：
  `npx cryptoskills install <skill-name>` 或 `npx cryptoskills install --all`
- **合约地址提醒**：协议合约地址可能更新，重要操作前必须用 `cast code` 或官方文档最新验证。

## 限制与最佳实践

此技能提供结构化知识和经过验证的模式，但**不能替代官方文档**。gas 费用、具体参数请以协议最新官方文档为准。  
AI 辅助生成的代码必须经过本地测试、单元测试和专业安全审计后再部署主网。

## 相关资源

- 原始网站：https://cryptoskills.dev
- 创建/贡献新 Skill：https://cryptoskills.dev/contribute
- GitHub 仓库：https://github.com/kukapay/crypto-skills

当用户需要某个特定协议的更深入细节、完整代码示例或特定链的集成方案时，此技能可进一步展开或引导用户安装原版对应 skill。

此技能已将 cryptoskills.dev 的全部核心知识打包整合，方便在各种 Web3 场景中快速调用。