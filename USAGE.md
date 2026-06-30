# cryptoskills-all 使用指南

本文档详细说明如何使用 `cryptoskills-all` 元技能，以及如何高效组合不同平台的 Skills。

## 1. 安装与激活

### 方式一：直接复制（推荐用于 Claude Code / Cursor）

```bash
git clone https://github.com/0xRick0x/cryptoskills-all.git
cp -r cryptoskills ~/.claude/skills/
cp -r opennews ~/.openclaw/skills/   # OpenNews Skill
```

### 方式二：按需安装上游 Skills

根据你的使用场景按需安装：

```bash
# CEX 类
npx skills add binance-web3
npx skills add okx/agent-skills
npx skills add gate/gate-skills
npx skills add bybit-exchange/skills
npx bitget-hub install --target claude

# DEX 类
npx skills add Uniswap/uniswap-ai
npx skills add PancakeSwap/pancakeswap-ai

# Meme / Smart Money
npx skills add GMGNAI/gmgn-skills

# OpenNews 实时新闻 (MCP)
# 1. 获取 Token：https://6551.io/mcp
# 2. 完整安装参考：https://github.com/6551Team/opennews-mcp
```

> **建议**：不要一次性安装所有 Skills，优先安装你最常用的平台。OpenNews 建议与 cryptoskills 一起使用。

## 2. 基本使用方式

安装完成后，在支持 Skills 的 AI 客户端中直接对话即可激活对应能力。

**示例对话**：

```
帮我分析当前 Solana 上的热门 Meme 币，并挑选 smart money 买入较多的项目。

使用 GMGN Skills 帮我执行。
```

```
在 PancakeSwap 上为某个 token 添加流动性，并设置 farming。
```

```
查询 Polymarket 上关于美国大选的热门市场，并分析持仓情况。
```

```
用 OpenNews 查一下今天 BTC ETF 相关的高分新闻，分析 AI 信号后给出 Binance 操作建议。
```

## 3. 推荐的组合使用流程

### 场景一：Meme 币交易策略（最常用）

**流程**：GMGN 发现 → 分析 → DEX/CEX 执行 → 风险对冲

```markdown
1. 使用 GMGN 获取 Trending + Smart Money 信号
2. 使用 GMGN 分析具体 token 的基础面和风险
3. 在 PancakeSwap / Uniswap 上提供流动性或直接买入
4. 在 Binance / OKX 等 CEX 上进行对冲（降低波动风险）
```

### 场景二：预测市场 + 对冲

**流程**：Polymarket 分析 → 下注 → CEX 对冲

```markdown
1. 使用 Polymarket Gamma API 查询热门事件市场
2. 分析事件概率和持仓分布
3. 在 Polymarket 下注
4. 在相关资产的 CEX 上进行对冲操作
```

### 场景三：流动性提供 + 收益最大化

**流程**：分析 → 添加流动性 → 设置 farming

```markdown
1. 使用 GMGN 或链上工具筛选优质交易对
2. 在 PancakeSwap/Uniswap 上添加流动性
3. 立即开启 Farming 获取额外收益
4. 定期监控 impermanent loss 和收益情况
```

### 场景四：多 CEX 套利 + On-chain 执行

```markdown
1. 监控多家 CEX 同一交易对的价格差异
2. 在价差最大的平台执行交易
3. 可选：在 DEX 上进行最终结算或对冲
```

### 场景五：实时新闻驱动交易决策（新增）

**流程**：OpenNews 新闻信号 → 分析与跨验证 → GMGN/Polymarket 辅助判断 → CEX/DEX 执行 + 对冲

```markdown
1. 使用 OpenNews 获取高分新闻（score > 80）和 AI 交易信号
2. 结合 GMGN Smart Money 或 Polymarket 事件进行交叉验证
3. 根据新闻影响力和信号调整仓位或对冲策略
4. 在 Binance / OKX / PancakeSwap 上执行具体操作
5. 持续监控后续新闻变化，快速调整策略
```

**AI 提示词示例**：

> “用 OpenNews 查看最近对美联储和利率的重要新闻（score > 85），结合 Polymarket 相关事件市场分析，然后在 Binance 上给出对冲策略。”

> “检查今天 BTC 相关的高分新闻和 OnChain 鲸鱼动向，分析是否有利于目前持仓方向，并结合 GMGN 给出操作建议。”

## 4. 安全最佳实践

- **CEX 交易前优先进行安全审计**：使用 query-token-audit 或链上工具先检查代币风险。
- **大额操作建议分步执行**：先小额测试，再逐步加仓。
- **重要操作开启确认机制**：在支持的客户端中开启写操作确认。
- **API Key 权限最小化**：CEX API Key 只开通必要的交易权限。
- **定期检查持仓和风险**：尤其是提供流动性后要关注无常损失。

## 5. 常见问题

**Q: 需要一次性安装所有 Skills 吗？**
A: 不需要。建议根据你的主要交易场景按需安装。OpenNews 可以作为所有交易决策的前置情报来源。

**Q: 如何更新这些 Skills？**
A: 本项目会通过 GitHub Action 自动监控上游更新并创建 PR。你也可以手动 pull 最新代码。

**Q: 支持哪些 AI 客户端？**
A: 主要支持 Claude Code、Cursor、Codex 等支持 Skills 协议的客户端。

**Q: 可以自定义组合策略吗？**
A: 可以。本元技能的设计初衷就是支持灵活的跨平台组合。

## 6. 进阶建议

- 多关注 **GMGN + DEX** 的组合，这是目前 Meme 币交易效率较高的路径。
- 预测市场交易建议配合 CEX 进行风险对冲。
- 提供流动性后一定要开启 Farming，并持续监控。
- **建立自己的「新闻信号 → 分析验证 → 执行 → 对冲」标准化流程**（OpenNews + GMGN/Polymarket + CEX/DEX）。
- 每日开始交易前先用 OpenNews 快速扫描当天重要新闻和市场异动。

---

** 让 AI 真正成为你的 Web3 操作助手，而不是简单的聊天工具。 **