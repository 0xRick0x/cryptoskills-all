# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.3.5] - 2026-06-30

### Added
- USAGE.md 深度优化「宏观新闻 + 资金费率套利」场景（场景七）：
  - 新增激进型与稳健型两种风险级别版本
  - 增加多层验证决策树
  - 每个版本附带更专业、可直接复制的中文 AI Prompt
- README.md 速查表优化：
  - 新增多个场景行（包含宏观新闻套利、新闻 + Polymarket 事件等）
  - 增加“风险风格参考”列
  - 调整流程描述使表格更清晰实用
- 更新 CHANGELOG 记录本次优化

### Changed
- 宏观相关文档实用性和可操作性大幅提升

## [1.3.4] - 2026-06-30

### Added
- USAGE.md 深度优化「新闻驱动 Meme 币交易」场景：
  - 新增激进型与稳健型两种风险级别版本
  - 增加多层验证决策树
  - 每个版本附带更专业、可直接复制的中文 AI Prompt
- README.md 新增「技能组合速查表」章节（清晰表格汇总主要场景、组合方式、流程和 prompt 关键词）
- 更新 CHANGELOG 记录本次优化

### Changed
- Meme 相关文档实用性和可操作性大幅提升

## [1.3.3] - 2026-06-30

### Added
- 更新 `CONTRIBUTING.md`：反映当前完整生态（包含 OpenNews等），新增“添加新技能包”指南、SKILL.md 格式建议和更详细的贡献流程
- `USAGE.md` 新增「更多高级组合示例」章节，包含 3 个新场景：
  - 新闻驱动 Meme 币交易
  - 宏观新闻 + 资金费率套利
  - OnChain 鲸鱼预警 + CEX 快速响应
- 每个新场景都附带完整流程和专业中文 AI prompt 示例

### Changed
- 文档实用性和交易场景覆盖度进一步提升

## [1.3.2] - 2026-06-30

### Added
- 完善 `USAGE.md`：新增 OpenNews 安装说明、中文示例对话和「场景五：实时新闻驱动交易决策」完整流程
- USAGE.md 进阶建议添加日常新闻监控和标准化流程建议
- README.md 小幅润色（新增 OpenNews 快速上手独立小节，提示词更突出）
- opennews/SKILL.md 中文示例 prompt 更自然、专业，更符合中文用户使用习惯

### Changed
- 整体文档一致性和实用性进一步提升

## [1.3.1] - 2026-06-30

### Added
- 为 `opennews/SKILL.md` 新增完整内容并添加了「中文使用示例」章节（包含 5 个实用 crypto 交易场景 + AI 提示词）
- 优化 `README.md` 中文表达、快速开始部分、OpenNews 提示词示例和结构清晰度
- 更新 CHANGELOG 记录本次优化

### Changed
- `opennews/SKILL.md` 现在更适合中文用户使用，支持与 cryptoskills 元技能无缝组合

## [1.3.0] - 2026-06-30

### Added
- Integrated **OpenNews MCP** (from 6551Team/opennews-mcp) and OpenClaw skill definition.
- Added `opennews/SKILL.md` for real-time financial market news aggregator (84+ sources, AI impact scores, trading signals, onchain alerts, listing news, meme sentiment).
- Added OpenNews to automated upstream monitoring in GitHub Actions workflow.
- Enhanced ecosystem coverage with real-time news for better crypto/equities/macro trading decisions.
- Updated README.md and meta cryptoskills to reference news capabilities.

### Changed
- Expanded "集成生态" and capability sections to include news-driven insights.

## [1.2.0] - 2026-06-24

### Added
- Integrated **Polymarket API** as Skills (Gamma + CLOB).
- Added complex combination examples (GMGN signal → execution, Polymarket analysis → CEX hedge, GMGN Meme → DEX LP).
- Added "常见组合用法（高级场景）" section in SKILL.md.
- Created `CHANGELOG.md`.

### Changed
- Major refactor of `cryptoskills/SKILL.md` for better structure and readability.
- Improved classification of capabilities.
- Synchronized and polished `README.md`.
- Enhanced code examples quality and added more practical combination flows.

## [1.1.0] - 2026-06-24

### Added
- Integrated **GMGN AI Skills** (Trending, Smart Money tracking).
- Integrated **Bitget Agent Hub** + `bitget-skill`.
- Integrated **Bybit AI Trading Skill** and official MCP Server.
- Integrated **Gate AI Agent** (41+ Skills).

### Changed
- Expanded ecosystem coverage significantly.
- Improved example quality across multiple platforms.

## [1.0.0] - 2026-06-24

### Added
- Initial release of `cryptoskills-all` meta-skill.
- Integrated core from cryptoskills.dev.
- Added major CEX Agents: Binance, OKX, Gate, Bybit, Bitget.
- Added DEX AI Skills: Uniswap and PancakeSwap.
- Created initial `SKILL.md` and `README.md`.
- Added automated upstream monitoring via GitHub Actions.

## [0.9.0] - 2026-06-23

### Added
- Project initialization with basic structure.
- Early integration of cryptoskills.dev and first CEX skills.