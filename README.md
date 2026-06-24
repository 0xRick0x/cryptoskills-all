# cryptoskills-all

> 一个为 AI Coding Agents 打包的 Web3 / Crypto 协议**元技能**（Meta Skill）

将 [cryptoskills.dev](https://cryptoskills.dev) 上的 97 个专业技能打包整合成一个技能，让 Claude Code、Cursor、Codex、Cline 等 AI coding agent 能够快速、准确地掌握主流区块链协议知识。

---

## ✨ 项目简介

本技能是基于 [cryptoskills.dev](https://cryptoskills.dev) 项目的**元技能版本**，将原本分散的 97 个独立 skills 整合为一个统一技能包。

**核心价值**：让 AI 快速获得生产级的 DeFi、跨链、智能合约安全、AI Agent 构建等 Web3 领域知识，大幅提升开发效率并减少幻觉和错误。

---

## 📌 来源与修改说明

- **原始来源**：https://cryptoskills.dev（GitHub: kukapay/crypto-skills）
- **本次修改**：
  - 将 97 个独立 skills 打包为**单个元技能**
  - 新增大量**中文说明**和**具体实用场景**
  - 增加「具体能帮你做什么」详细列表（9 大类真实开发场景）
  - 优化兼容性，支持 **Claude Code、Cursor、Codex、Cline** 等主流 AI coding agent
  - 增加清晰的使用方法和安装指南

---

## 🚀 主要作用

- 让 AI 快速掌握 Aave、Jupiter、LayerZero、Slither、Foundry、Chainlink 等 97 个主流协议的使用方式
- 提供生产级代码模式、安全最佳实践和常见坑点提醒
- 支持 DeFi 集成、跨链桥接、智能合约审计、AI 交易代理构建等多场景
- 显著提升 Web3 项目开发速度和代码质量

---

## 🛠 具体能帮你做什么

| 场景类别           | 能帮你解决的问题示例                              |
|--------------------|--------------------------------------------------|
| DeFi 集成          | Aave 借贷、Jupiter 交换、Drift/GMX 杠杆交易代码   |
| 跨链操作           | LayerZero / Wormhole 安全桥接与消息传递           |
| 智能合约安全       | Slither + Mythril 审计流程 + 漏洞修复建议         |
| 多链开发           | Foundry / Hardhat 多链部署脚本                    |
| AI Agent 构建      | 让 AI 自主执行链上交易、跨链套利                  |
| 前端 UX            | Privy + viem 钱包连接与交易体验优化               |
| 预言机与 NFT       | Chainlink/Pyth 集成、Metaplex 压缩 NFT 发行       |
| 交易与分析         | 预测市场、聪明钱追踪、永续合约策略                |

---

## 📥 安装方法

### 推荐方式（手动安装，兼容性最好）

1. 下载或克隆本仓库
2. 将 `cryptoskills` 文件夹复制到对应 AI 工具的 skills 目录：

| AI 工具          | 推荐路径                                      |
|------------------|-----------------------------------------------|
| **Claude Code**  | `~/.claude/skills/cryptoskills/`              |
| **Cursor**       | 项目根目录或全局 skills 文件夹                |
| **Codex / Cline**| 参考对应工具的 skills 加载路径                |

3. 重启或重新加载 AI coding agent 即可生效。

### 使用原版 CLI 安装（可选）

```bash
npx cryptoskills install cryptoskills
