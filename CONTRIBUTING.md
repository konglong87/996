# Contributing to 996-workhorse

感谢你有兴趣为 996-workhorse 做贡献！🎉

## 如何贡献

### 报告问题

如果你发现了 bug 或有功能建议，请：

1. 检查 [Issues](https://github.com/konglong87/996/issues) 中是否已有类似问题
2. 如果没有，创建新的 Issue，包含：
   - 清晰的标题和描述
   - 复现步骤（如果是 bug）
   - 期望行为和实际行为
   - 截图或日志（如适用）
   - 环境信息（OS、软件版本等）

### 提交改进

#### 1. Fork 项目

```bash
# Fork 后克隆你的仓库
git clone https://github.com/YOUR_USERNAME/996.git
cd 996
```

#### 2. 创建分支

```bash
git checkout -b feature/your-feature-name
# 或
git checkout -b fix/your-bug-fix
```

#### 3. 进行修改

- 遵循现有的代码风格
- 更新相关文档
- 添加必要的测试（如适用）

#### 4. 提交更改

```bash
git add .
git commit -m "type: description"
```

**提交信息规范**：

- `feat:` 新功能
- `fix:` 修复 bug
- `docs:` 文档更新
- `style:` 代码格式调整（不影响功能）
- `refactor:` 代码重构
- `test:` 测试相关
- `chore:` 构建/工具相关

示例：
```
feat: 添加 P4 极限模式
fix: 修复 P3 模式备份失败问题
docs: 更新安装文档
```

#### 5. 推送到 GitHub

```bash
git push origin feature/your-feature-name
```

#### 6. 创建 Pull Request

1. 访问你 fork 的仓库页面
2. 点击 "New Pull Request"
3. 填写 PR 模板：
   - 描述你的更改
   - 关联相关 Issue（如 `Fixes #123`）
   - 列出测试步骤

## 开发指南

### 项目结构

```
996/
├── skills/
│   └── 996-workhorse/
│       └── SKILL.md          # 核心 skill 文件
├── README.md                 # 项目说明
├── CHANGELOG.md              # 版本历史
├── CONTRIBUTING.md           # 贡献指南（本文件）
├── LICENSE                   # MIT 许可证
├── plugin.json               # 插件配置
└── marketplace.json          # 市场配置
```

### SKILL.md 编写规范

1. **YAML Frontmatter**
   - `name`: skill 名称
   - `description`: 详细描述和触发条件

2. **章节结构**
   - 核心铁律：定义基本行为准则
   - 工作强度分级：P0-P3
   - 方法论：提供具体指导
   - 案例：实际应用示例

3. **格式要求**
   - 使用 Markdown 格式
   - 代码块指定语言
   - 保持缩进一致
   - 中英文之间加空格

### 测试

在提交 PR 前，请确保：

- [ ] SKILL.md 格式正确
- [ ] 在 Claude Code 中测试过
- [ ] 文档已更新
- [ ] 提交信息符合规范

## 行为准则

- 尊重所有贡献者
- 接受建设性批评
- 关注对项目最有利的事情
- 对新手友善

## 获取帮助

如果你有任何问题：

1. 查看 [README](README.md) 和 [文档](skills/996-workhorse/SKILL.md)
2. 搜索 [Issues](https://github.com/konglong87/996/issues)
3. 创建新的 Issue 并标记为 `question`

## 许可证

通过贡献代码，你同意你的贡献将根据 [MIT License](LICENSE) 授权。

---

再次感谢你的贡献！💪