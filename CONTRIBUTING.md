# 贡献指南 (CONTRIBUTING)

感谢你有兴趣贡献到 `cryptoskills-all` 项目！

本项目是一个集成了 **cryptoskills.dev** + **Binance** + **OKX** + **Gate** + **Bybit** + **Bitget** + **Uniswap** + **PancakeSwap** + **GMGN** + **Polymarket** + **OpenNews** 等多个生态的 **元技能 (Meta Skill)** 集合。目标是让 AI Agent 更安全、更高效地进行 Web3 交易、市场分析和新闻驱动决策。

## 如何贡献

### 1. 提交 Issue

如果你发现了 bug、想要新功能或有任何建议，请提交 Issue，并附上：

- 清晰的标题
- 复现步骤（如果有）
- 你的环境信息（AI 工具版本、操作系统等）

### 2. 提交 Pull Request

1. Fork 本仓库
2. 创建新分支 (`git checkout -b feature/your-feature-name`)
3. 在分支上进行修改
4. 提交 PR 前，请确保：
   - 代码/文档格式符合项目风格
   - 已测试过
   - 提交信息清晰

### 3. 欢迎的贡献类型

- 新增实用代码示例（特别是多平台组合场景）
- 优化现有说明和结构
- 修复错别字或表达不清楚的内容
- 新增实用交易场景说明（先特别欢迎新闻驱动类型）
- 改进 README、USAGE.md 等文档
- 添加新的技能包（可参考 opennews/ 目录结构）

### 4. 添加新技能包的建议

如果你想添加新的技能包（如新的 CEX、DEX 或新闻源）：

- 在项目根目录下创建 `your-skill/SKILL.md`
- 参考 `opennews/SKILL.md` 的格式（包含 frontmatter + 详细使用说明 + 中英文示例）
- 在 README.md 和 USAGE.md 中更新集成表格和示例
- 更新 `.github/workflows/check-upstream-updates.yml` 添加上游监控
- 在 PR 中说明新技能的来源和优势

### 5. 更新 `cryptoskills/SKILL.md` 元技能的建议

- 保持中文说明为主
- 新增示例时请附上简单的使用场景说明
- 优先推荐安全相关、市场数据类和新闻驱动类 Skills
- 更新后请在 PR 中说明更新理由

### 6. Commit 规范

- `feat:` 新功能
- `fix:` 修复 bug
- `docs:` 文档更新
- `chore:` 其他不影响代码逻辑的修改

## 联系方式

如果你有任何疑问，可以通过 Issue 联系维护者。

再次感谢你的贡献！

---

**Let’s make AI better at Web3 together.**