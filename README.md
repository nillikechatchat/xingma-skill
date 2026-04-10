# 行吗 (Xingma) Skill

## 简介
「行吗」是一个 AI Agent 技能，专注于 **合规性检查与法律框架分析**。它可以帮助用户评估特定行为、项目或文档是否符合相关的法律法规，并提供基于法律框架的建议。

## 触发词
当对话中包含以下词汇或意图时，Agent 将尝试加载此技能：
- 行吗 (Xingma)
- 合规 (Compliance)
- 法律风险 (Legal Risk)
- 是否合法 (Is it legal?)
- 法律框架 (Legal Framework)

## 安装方法

如果你正在使用 **HiClaw** 或兼容的 Agent 平台：

1. **克隆此仓库**:
   ```bash
   git clone https://github.com/{your-org}/xingma-skill.git
   ```

2. **移动到技能目录**:
   将 `xingma-skill` 文件夹移动到你的 Agent 的 `active_skills` 目录中：
   ```bash
   mv xingma-skill /path/to/your/agent/active_skills/xingma-skill
   ```

3. **重启 Agent**:
   重新启动你的 Agent 服务以加载新技能。

## 使用示例

**用户**: "我们在用户协议里加上这一条：'公司有权在任何情况下随时删除用户数据'，行吗？"
**Agent**: *(触发「行吗」技能)*
> "根据相关数据保护法律框架（如 GDPR 或《个人信息保护法》），这种单方面、无限制的删除条款可能存在合规风险。建议修改为：'在法律法规允许的范围内，且在不影响用户已产生权益的前提下，公司有权...'"

## 包含文件

- `SKILL.md`: 技能的主要配置文件，定义了技能的行为和逻辑。
- `references/research/`: 包含支持性的法律研究文档。
  - `01-legal-framework.md`: 基础法律框架分析。

## 贡献

欢迎提交 Issue 或 Pull Request 来完善法律案例库。

## 许可证

[MIT License](LICENSE)