# 🚀 AI 开发流程主控系统

<div align="center">

[![Version](https://img.shields.io/badge/version-1.0.0-blue.svg?style=flat-square)](https://github.com/yourusername/skills)
[![License](https://img.shields.io/badge/license-MIT-green.svg?style=flat-square)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](CONTRIBUTING.md)

智能 AI 开发流程调度系统，协调产品经理、UI设计师、全栈开发工程师、邮件通知、魔方模板开发、魔方财务插件等专业技能包

</div>

## ✨ 特性

- 🎯 **智能流程调度** - 根据用户需求和项目状态，自动选择合适的技能包
- 📊 **状态管理** - 自动检测项目进度，智能判断 0-1 模式或迭代模式
- 🔌 **指令路由** - 解析用户指令，调用对应技能包处理请求
- ✅ **质量控制** - 确保每个阶段的输出符合要求，才能进入下一阶段
- 📧 **邮件通知** - 任务完成后自动发送变更通知和代码片段
- 🎨 **UI/UX 设计** - 支持多种前端技术栈和设计风格
- 🔌 **插件扩展** - 支持魔方财务的模板和插件开发

## 🛠️ 技术栈

<table>
  <tr>
    <td align="center"><img src="https://img.icons8.com/color/48/000000/python.png" width="40" height="40"/><br/>Python</td>
    <td align="center"><img src="https://img.icons8.com/color/48/000000/php.png" width="40" height="40"/><br/>PHP</td>
    <td align="center"><img src="https://img.icons8.com/color/48/000000/javascript.png" width="40" height="40"/><br/>JavaScript</td>
    <td align="center"><img src="https://img.icons8.com/color/48/000000/html.png" width="40" height="40"/><br/>HTML</td>
    <td align="center"><img src="https://img.icons8.com/color/48/000000/css.png" width="40" height="40"/><br/>CSS</td>
  </tr>
</table>

## 📦 技能包列表

| 技能包                      | 功能描述                                         |
| ------------------------ | -------------------------------------------- |
| **product-spec-builder** | 产品经理 - 通过追问收集需求，检测逻辑冲突，生成产品文档                |
| **ui-prompt-generator**  | UI设计师 - 自动生成原型图提示词，提供视觉风格和配色方案               |
| **dev-builder**          | 全栈开发工程师 - 自动判断项目类型和技术栈，实现功能代码                |
| **email-notifier**       | 邮件通知 - 配置邮件地址，任务完成后自动发送变更通知                  |
| **mfui**                 | 魔方模板开发 - 支持魔方财务系统的模板开发，包含完整变量列表              |
| **mfapp**                | 魔方财务插件开发 - 支持各类插件开发（sms、mail、oauth、addons 等） |
| **ui-refactor**          | UI重构 - 现有项目的前端 UI/UX 重构技能                    |
| **ui-ux-pro-max**        | UI/UX Pro - 专业 UI/UX 设计，支持多种技术栈和设计风格         |

## 🚀 快速开始

### 前置条件

- 确保你的开发环境已配置好
- 支持的操作系统：Windows / macOS / Linux

### 安装使用

1. 克隆或下载项目到本地

```bash
cd d:\桌面\skills
```

1. 查看可用指令

```bash
/help
```

1. 开始你的第一个项目

```bash
/prd
```

## 📋 可用指令

| 指令          | 功能描述                                                                                             | 前置条件                 |
| ----------- | ------------------------------------------------------------------------------------------------ | -------------------- |
| **/prd**    | 需求收集 - 启动产品经理技能包，通过追问收集需求（0-1模式）或更新现有产品文档（迭代模式）                                                  | 无                    |
| **/ui**     | 生成原型图提示词 - 调用 ui-prompt-generator 技能包，生成 UI-Prompts.md                                           | Product-Spec.md 必须存在 |
| **/dev**    | 开发代码 - 调用 dev-builder 技能包，判断项目类型，选择技术栈，实现功能代码                                                    | Product-Spec.md 必须存在 |
| **/run**    | 本地运行 - 启动项目，验证功能，报告运行结果和问题                                                                       | 无                    |
| **/check**  | 完整度检查 - 对照 Product-Spec.md 检查功能是否完整，列出已实现和未实现的功能，提出补充建议                                          | Product-Spec.md 必须存在 |
| **/status** | 查看进度 - 显示当前项目状态（0-1模式 / 迭代模式），显示已完成的功能列表，显示待办事项                                                  | 无                    |
| **/email**  | 配置邮件通知 - 配置接收任务完成通知的邮件地址，保存配置到 Email-Config.json，每次任务完成后自动发送变更通知和代码片段                            | 无                    |
| **/help**   | 查看帮助 - 列出所有可用指令和功能，显示每个指令的用途说明，提供使用指南                                                            | 无                    |
| **/mfui**   | 魔方模板开发 - 理解魔方财务模板架构，创建和定制 .tpl 模板文件，熟练使用 ThinkPHP 模板语法，支持响应式设计                                   | 无                    |
| **/mfapp**  | 魔方财务插件开发 - 理解魔方财务插件系统，创建各类插件（sms、mail、oauth、certification、addons），正确继承 Plugin 基类，实现插件的安装、卸载和核心功能 | 无                    |

## 🎯 工作流程

### 完整开发流程（0-1 模式）

```mermaid
graph TD
    A[用户说出想法] --> B[/prd - 需求收集]
    B --> C[自动生成 Product-Spec.md]
    C --> D[自动生成 Product-Spec-CHANGELOG.md]
    D --> E[/ui - 原型设计]
    E --> F[生成 UI-Prompts.md]
    F --> G[/dev - 开发代码]
    G --> H[实现功能代码]
    H --> I[/run - 本地运行]
    I --> J[验证功能，报告结果]
```

### 迭代开发流程（有 Product-Spec.md）

```mermaid
graph TD
    A[用户提出修改需求] --> B[/prd - 迭代模式]
    B --> C[更新 Product-Spec.md]
    C --> D[更新 Product-Spec-CHANGELOG.md]
    D --> E[自动调用 /dev]
    E --> F[开发工程师实现代码]
    F --> G[文档和代码同步]
```

## 📁 项目结构

```
skills/
├── .trae/
│   └── skills/
│       ├── dev-builder/              # 全栈开发工程师技能包
│       │   └── SKILL.md
│       ├── email-notifier/           # 邮件通知技能包
│       │   ├── SKILL.md
│       │   └── scripts/
│       │       └── email_sender.py
│       ├── mfapp/                    # 魔方财务插件开发技能包
│       │   └── SKILL.md
│       ├── mfui/                     # 魔方模板开发技能包
│       │   └── SKILL.md
│       ├── product-spec-builder/     # 产品经理技能包
│       │   ├── SKILL.md
│       │   └── templates/
│       ├── ui-prompt-generator/      # UI设计师技能包
│       │   ├── SKILL.md
│       │   └── templates/
│       ├── ui-refactor/              # UI重构技能包
│       │   └── SKILL.md
│       └── ui-ux-pro-max/            # UI/UX Pro技能包
│           └── SKILL.md
├── AGENTS.md                         # AI开发流程主控配置
└── README.md                         # 项目说明文档（本文件）
```

## 🤝 贡献指南

欢迎参与贡献！请查看 [CONTRIBUTING.md](CONTRIBUTING.md) 了解更多详情。

1. Fork 本仓库
2. 创建你的功能分支 (`git checkout -b feature/AmazingFeature`)
3. 提交你的更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 打开一个 Pull Request

## 📄 许可证

本项目采用 MIT 许可证 - 详见 [LICENSE](LICENSE) 文件

## 💬 联系方式

- 项目 GitHub：<https://github.com/yourusername/skills>

  <br />

## 🙏 致谢

感谢所有为这个项目做出贡献的人！

***

<div align="center">
  <sub>如果这个项目对你有帮助，请给个 ⭐ Star 支持一下！</sub>
</div>
