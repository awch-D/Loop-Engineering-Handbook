# Loop Engineering Handbook · Loop 工程学习手册

> A practical handbook on **Loop Engineering** — the emerging paradigm for building self-running AI agents. From ReAct to Claude Code's `/loop`.

<p align="center">
  <a href="https://awch-d.github.io/Loop-Engineering-Handbook/"><img src="https://img.shields.io/badge/preview-online-5b6cff?style=flat-square" alt="preview"/></a>
  <a href="LICENSE"><img src="https://img.shields.io/badge/license-MIT-34c759?style=flat-square" alt="license"/></a>
  <img src="https://img.shields.io/badge/format-single--html-ff9500?style=flat-square" alt="single html"/>
  <img src="https://img.shields.io/badge/lang-中文-1d1d1f?style=flat-square" alt="zh-CN"/>
  <img src="https://img.shields.io/badge/style-Apple%20Glass-ff3b30?style=flat-square" alt="apple glass"/>
</p>

---

## 📖 简介

2026 年 6 月，**Loop Engineering（循环工程）** 作为新的工程范式被正式命名。它位于 Prompt → Context → Harness → Loop 这条 AI 工程化链路的最上层，回答的是同一个问题：**当模型已经会用工具、能读上下文、有合适提示之后，谁来按下"下一步"按钮？**

本仓库是一份**单文件 HTML 学习手册**，系统梳理了 Loop 工程的来龙去脉、核心架构、主流模式、工程实践与常见误区。所有结论均可追溯到 Anthropic、LangChain、Addy Osmani、Lilian Weng 等一手来源。

---

## ✨ 特性

- 🎯 **12 章完整体系** — 从一句话定义、范式金字塔到学习路径，循序渐进
- 🍎 **Apple Glass 风格** — 浅色主题 + 毛玻璃质感 + 柔和径向渐变
- 📦 **单文件零依赖** — 一个 `index.html` 即可，无需任何构建步骤
- 🎨 **30+ 内嵌 SVG 图标** — 全部本地化，无外部 CDN
- 📱 **完全响应式** — 桌面 / 平板 / 移动端自适应
- 🧭 **滚动联动侧边栏** — `IntersectionObserver` 实现章节高亮
- 🔗 **10+ 一手引用** — 每条结论可回溯到原始论文或官方博客
- 🇨🇳 **中文优先** — 面向中文 AI 圈读者的术语解释与例证

---

## 📚 章节目录

| # | 章节 | 核心内容 |
|---|---|---|
| 01 | 什么是 Loop 工程 | 一句话定义、与 Prompt/Context 工程的区别 |
| 02 | 工程化范式金字塔 | Prompt → Context → Harness → Loop 四层递进 |
| 03 | 起源与演进时间线 | 从 ReAct (2022) 到 Loop Engineering 命名 (2026) |
| 04 | 核心架构 | 单步 Agent Loop（ASCII 流程图）与五大要素 |
| 05 | Addy Osmani 六大组件 | Automations / Worktrees / Skills / MCP / Sub-agents / State |
| 06 | LangChain 四层循环堆叠 | L1 Agent → L2 Verify → L3 Event → L4 Hill-Climb |
| 07 | 代码片段速览 | LangGraph create_agent / Claude Code /goal / MCP 子 Agent 配置 |
| 08 | 主流循环模式对比 | ReAct / Reflexion / Self-Refine / ToT / Evaluator-Optimizer |
| 09 | 主流产品如何实现 Loop | Claude Code / Codex / LangGraph / Cursor / Devin / Swarm / Aider |
| 10 | 关键挑战与解法 | 上下文爆炸、Token 成本、终止条件、安全权限 |
| 11 | 五个常见误区 | 把 Loop 等同于 while 循环等典型陷阱 |
| 12 | 推荐学习路径 | 论文 / 博文 / 项目 / 中文资料 四条线索 |
| 13 | 术语速查表 | Harness / Maker-Checker / MCP / Trace / Autoresearch 等 12 个术语 |
| 14 | 常见疑问 FAQ | 什么时候不该用 Loop、Loop 工程 = LangGraph 吗？ |
| 15 | 参考资料 | 10+ 条带置信度标签的一手链接 |

---

## 🚀 在线预览

**👉 [awch-d.github.io/Loop-Engineering-Handbook](https://awch-d.github.io/Loop-Engineering-Handbook/)**

每次推送到 `main` 分支会通过 GitHub Actions 自动重新部署。

本地查看只需双击 `index.html`：

```bash
git clone https://github.com/awch-D/Loop-Engineering-Handbook.git
cd Loop-Engineering-Handbook
open index.html        # macOS
# xdg-open index.html  # Linux
# start index.html     # Windows
```

---

## 🛠️ 技术栈

- **HTML5** + **原生 CSS**（CSS 变量、Grid、Flexbox、`backdrop-filter`）
- **原生 JavaScript** — 仅用于侧边栏滚动联动（约 20 行）
- **内嵌 SVG** — 所有图标本地化，无 CDN 依赖
- **零构建** — 不需要 Node.js、Webpack、任何包管理器

整个手册编译产物就是它本身。

---

## 📂 项目结构

```
Loop-Engineering-Handbook/
├── index.html      # 手册主体（单文件，含全部样式与脚本）
├── README.md       # 你正在看的这个文件
├── LICENSE         # MIT 协议
└── .gitignore
```

---

## 🤝 贡献

欢迎通过以下方式参与：

- **发现错别字 / 链接失效** → 直接提 PR
- **补充新的一手资料 / 论文** → Issue 讨论后 PR
- **修正概念解释** → 请附原始来源链接
- **新增章节** → 先开 Issue 对齐结构

提交前请保持单文件结构（不引入构建工具），并遵循现有视觉风格。

---

## 📜 引用

如果这份手册帮到了你的研究或文章，欢迎引用：

```bibtex
@misc{loop-engineering-handbook,
  title  = {Loop Engineering Handbook: A Practical Guide to Building Self-Running AI Agents},
  author = {Arno},
  year   = {2026},
  url    = {https://github.com/awch-D/Loop-Engineering-Handbook}
}
```

---

## 🔗 核心参考

按一手来源置信度排序：

- [Anthropic · Building Effective Agents (2024-12)](https://www.anthropic.com/engineering/building-effective-agents)
- [Addy Osmani · Loop Engineering (2026-06)](https://addyosmani.com/blog/loop-engineering/) — 术语命名性文章
- [LangChain · The Art of Loop Engineering (2026-06)](https://www.langchain.com/blog/the-art-of-loop-engineering)
- [Lilian Weng · LLM Powered Autonomous Agents (2023-06)](https://lilianweng.github.io/posts/2023-06-23-agent/)
- [Anthropic · Demystifying Evals for AI Agents (2026-01)](https://www.anthropic.com/engineering/demystifying-evals-for-ai-agents)

完整 10 条引用列表见手册第 12 章。

---

## 📄 协议

本仓库以 [MIT License](LICENSE) 开源。引用的第三方文章、论文、产品文档版权归原作者所有。

---

<p align="center">
  <i>Build the loop, stay the engineer.</i><br>
  <sub>— Addy Osmani</sub>
</p>
