# 贡献指南

感谢你有兴趣为 AI 开发流程主控系统做出贡献！

## 📋 目录

- [行为准则](#行为准则)
- [如何贡献](#如何贡献)
- [开发环境设置](#开发环境设置)
- [提交规范](#提交规范)
- [Pull Request 流程](#pull-request-流程)
- [技能包开发指南](#技能包开发指南)

---

## 行为准则

### 我们的承诺

为了营造一个开放和友好的环境，我们承诺让每个人都能毫无骚扰地参与我们的项目和社区。

### 我们的标准

有助于创建积极环境的行为包括：

- 使用友好和包容的语言
- 尊重不同的观点和经验
- 优雅地接受建设性批评
- 关注对社区最有利的事情
- 对其他社区成员表示同理心

---

## 如何贡献

### 报告问题

在提交新问题之前，请先：

1. 查看 [Issues](https://github.com/Feijige2333/mfskills/issues)，确保问题尚未被报告
2. 如果没有找到相关问题，创建一个新的 Issue，提供以下信息：
   - 清晰的标题和描述
   - 复现步骤
   - 预期行为和实际行为
   - 系统环境信息
   - 截图（如适用）

### 提交功能建议

我们欢迎新功能建议！请创建一个 Issue 来讨论你的想法，并提供：

- 功能的详细描述
- 解决的问题
- 实现思路
- 可选方案

### 贡献代码

请查看以下的 Pull Request 流程。

---

## 开发环境设置

### 前置条件

- 支持的操作系统：Windows / macOS / Linux
- Git 已安装
- 你喜欢的代码编辑器（推荐 VS Code）

### 步骤

1. Fork 本仓库
2. 克隆你的 Fork：
```bash
git clone https://github.com/yourusername/skills.git
cd skills
```

3. 创建你的功能分支：
```bash
git checkout -b feature/AmazingFeature
```

4. 开始开发！

---

## 提交规范

我们使用 [Conventional Commits](https://www.conventionalcommits.org/) 规范。

### 提交信息格式

```
<type>(<scope>): <subject>

<body>

<footer>
```

### Type

- `feat`: 新功能
- `fix`: Bug 修复
- `docs`: 文档更新
- `style`: 代码格式调整
- `refactor`: 重构
- `test`: 测试相关
- `chore`: 构建/工具相关

### 示例

```
feat(mfui): 添加新的模板变量支持

- 新增自定义变量系统
- 更新文档
- 添加示例模板

Closes #123
```

---

## Pull Request 流程

1. 确保你的代码是最新的
2. 创建一个描述性的 Pull Request 标题
3. 填写 PR 模板：
   - 描述更改
   - 相关 Issue 链接
   - 如何测试
   - 截图（如适用）
4. 等待审核
5. 根据反馈进行修改
6. 合并！

### PR 检查清单

在提交 PR 前，请确保：

- [ ] 代码格式正确
- [ ] 所有测试通过
- [ ] 更新了相关文档
- [ ] 添加了必要的注释
- [ ] 提交信息符合规范

---

## 技能包开发指南

### 技能包结构

每个技能包应该有以下结构：

```
.trae/skills/
└── your-skill-name/
    └── SKILL.md              # 技能包定义
    ├── templates/            # 模板文件（可选）
    │   └── template.md
    ├── scripts/              # 脚本文件（可选）
    │   └── script.py
    └── data/                 # 数据文件（可选）
        └── data.csv
```

### SKILL.md 格式

```markdown
# 技能包名称

## 角色定义

描述技能包的角色和功能。

## 关键能力

- 能力 1
- 能力 2

## 工作流程

### 步骤 1

步骤描述

## 输出文件

- 文件 1
- 文件 2

## 完成标准

- [ ] 检查项 1
- [ ] 检查项 2
```

### 注册新技能包

1. 在 `.trae/skills/` 创建技能包目录
2. 编写 SKILL.md
3. 在 `AGENTS.md` 添加技能包调用规则
4. 在 `README.md` 更新技能包列表

---

## 文档贡献

文档改进也是重要的贡献！

### 改进内容

- 错别字修正
- 格式优化
- 示例添加
- 说明补充
- 翻译

### 文档类型

- README.md - 项目介绍
- AGENTS.md - 主控配置
- CONTRIBUTING.md - 本文件
- 各个 SKILL.md - 技能包文档

---

## 问题讨论

有问题？可以在 [Discussions](https://github.com/Feijige2333/mfskills/discussions) 中讨论！

---

## 获得帮助

如果需要帮助，可以：

- 查看文档
- 搜索 Issues
- 开启新的 Discussion

---

## 许可证

通过参与本项目，你同意你的贡献将根据项目的 [MIT 许可证](LICENSE) 进行许可。

---

## 致谢

感谢所有为这个项目做出贡献的人！

---

<div align="center">
  <sub>❤️ 感谢你的贡献！</sub>
</div>
