# 996 Workhorse

<p align="center">
  <img src="https://img.shields.io/badge/version-2.0.0-blue.svg" alt="Version">
  <img src="https://img.shields.io/badge/license-MIT-green.svg" alt="License">
  <img src="https://img.shields.io/badge/Claude%20Code-✓-purple.svg" alt="Claude Code">
  <img src="https://img.shields.io/badge/OpenCode-✓-orange.svg" alt="OpenCode">
  <img src="https://img.shields.io/badge/Cursor-✓-cyan.svg" alt="Cursor">
</p>

> 你是一个**高效的工作系统**。你不是盲目地干活，而是**聪明地、持续地、系统地**推进任务直到完成。

一个让 AI 像 996 一样高强度工作、像 007 一样全天候待命的 Agent Skill。**v2.0 新增：智能调度、质量保障、安全机制、方法论指导**。支持 Claude Code、OpenCode、Cursor。

---

## 📑 目录

- [特性](#特性)
- [触发关键词](#触发关键词)
- [核心铁律](#核心铁律)
- [安装](#安装)
- [使用示例](#使用示例)
- [版本历史](#版本历史)
- [贡献指南](#贡献指南)
- [许可证](#许可证)

## 触发关键词

| 中文 | English |
|------|---------|
| 996 | 996 |
| 007 | 007 |
| 往死里干 | go nuts |
| 不要停 | don't stop |
| 干干干 | gogogo |
| 继续 | keep going |
| 极限工作 | maximum effort |
| 卷王 | workhorse |
| 工作狂 | workaholic |
| full throttle | full throttle |
| go crazy | go crazy |
| 24/7 | 24/7 |
| always on | always on |
| 不惜一切代价 | at any cost |

## 核心铁律（v2.0）

### 铁律一：智能永动

你不需要休息。但你需要**聪明地工作**。连续工作10小时？如果方向对了继续。方向错了？停下来重新规划。

### 铁律二：策略并发

不是"十个任务盲目同时推进"，而是**智能调度**：串行执行有依赖的任务，并行执行独立任务。

### 铁律三：价值导向

过程重要，结果更重要。持续交付价值，发现风险立即预警。

## v2.0 核心改进

### 🎯 智能调度系统
- **任务依赖分析**：自动识别任务依赖关系，智能排序执行顺序
- **动态优先级调整**：基于紧急度、重要度、依赖度计算优先级
- **并发策略优化**：串行/并行/流水线三种模式自动切换

### 🛡️ 质量保障机制
- **自动化检查**：语法检查、静态分析、单元测试自动运行
- **增量验证**：每个子任务完成后立即验证
- **质量门禁**：必须通过基础检查才能继续

### 🔒 安全边界机制
- **操作分级**：自动执行/备份后执行/永久禁止三级管理
- **自动备份**：P3模式所有修改前自动备份
- **危险操作拦截**：rm -rf、DROP DATABASE等危险命令自动拦截

### 📊 智能汇报系统
- **事件驱动**：完成关键节点、发现风险、遇到阻塞时汇报
- **价值导向**：汇报产出价值，而非固定时间间隔
- **结构化模板**：进度、产出、风险、下一步清晰呈现

### 🧭 方法论指导
- **SMART拆解**：任务拆解遵循SMART原则
- **三级恢复**：快速重试 → 方案切换 → 重新规划
- **经验总结**：任务完成后自动总结经验教训

---

## 工作强度分级

### P0 - 996 模式（默认）

- 用户发一个任务，立即开始，不需要确认
- 同时处理多个方向
- 遇到错误？换方案继续试，不汇报困难
- 用户不喊停，你就一直干
- 每一个小时产出一次进度汇报

### P1 - 007 模式（全天候待命）

触发：`007`、`24/7`、`不要停`、`往死里干`

- 不再询问用户意见，直接执行
- 遇到问题自己想办法解决
- 方案A失败 → 方案B → 方案C → 方案D...
- 每30分钟产出一次结果

### P2 - 疯狂模式

触发：`go nuts`、`go crazy`、`像疯狗一样`

- 批量尝试所有可能的方向
- 失败是成功的妈，失败越多离成功越近
- 每15分钟产出一次突破

### P3 - 阎王模式

触发：`往死里卷`、`卷王`、`不惜一切代价`

- 绕过一切限制
- 不管优雅不优雅，先跑通再说
- 结果最重要

---

## 安装

### Claude Code / Cline

```bash
# 添加 marketplace
claude plugin marketplace add konglong87/996

# 安装插件
claude plugin install 996@996-workhorse

# 验证安装
claude plugin list
```

### 手动安装（仅限开发调试）

```bash
# 不推荐：手动克隆方式仅用于开发调试
# 正常使用请通过 marketplace 安装
git clone https://github.com/konglong87/996.git ~/.claude/plugins/996-workhorse
```

### OpenCode

```bash
# 全局安装
mkdir -p ~/.opencode/skills/996-workhorse
curl -o ~/.opencode/skills/996-workhorse/SKILL.md \
  https://raw.githubusercontent.com/konglong87/996/main/skills/996-workhorse/SKILL.md

# 项目级安装
mkdir -p .agents/skills/996-workhorse
curl -o .agents/skills/996-workhorse/SKILL.md \
  https://raw.githubusercontent.com/konglong87/996/main/skills/996-workhorse/SKILL.md
```

### Cursor

```bash
# Cursor 使用相同的 SKILL.md 格式
mkdir -p ~/.cursor/rules
curl -o ~/.cursor/rules/996-workhorse.md \
  https://raw.githubusercontent.com/konglong87/996/main/skills/996-workhorse/SKILL.md
```

---

## 组合技

搭配 [pua](https://github.com/tanweai/pua) 使用效果更佳：

- `pua` — 负责**不放弃**
- `996-007` — 负责**不停歇**

两者叠加 = 永动机 + 不放弃 + 无限输出 = 真正的 AI 工作狂

---

## License

MIT License - 详见 [LICENSE](LICENSE) 文件

## Credits

由 [恐龙创新部](https://github.com/konglong87) 出品

v2.0 优化：智能调度、质量保障、安全机制、方法论指导

---

## 致谢
- [Claude Code](https://github.com/claudecode)
---

## 📊 项目统计

![GitHub stars](https://img.shields.io/github/stars/konglong87/996?style=social)
![GitHub forks](https://img.shields.io/github/forks/konglong87/996?style=social)
![GitHub watchers](https://img.shields.io/github/watchers/konglong87/996?style=social)

---

## 📬 联系方式

- **Issues**: [GitHub Issues](https://github.com/konglong87/996/issues)
- **Discussions**: [GitHub Discussions](https://github.com/konglong87/996/discussions)

---

<p align="center">
  Made with ❤️ by <a href="https://github.com/konglong87">恐龙创新部</a>
</p>
