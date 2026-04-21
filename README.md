<div align="right">

**[English](README_EN.md)** | 中文

</div>

<div align="center">

# write.skill

**把写作经验，蒸馏成可复用的认知资产。**

> 每一个 Great Writer，都有一套个人写作系统。
> 我们把这套系统，拆成针对不同平台、受众、领域的 Agent Skills。

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Agent Skill](https://img.shields.io/badge/Agent%20Skill-Compatible-blueviolet)](https://skills.sh)
[![Built with](https://img.shields.io/badge/Built%20with-Nuwa%20Skill-orange)](https://github.com/alchaincyf/nuwa-skill)

</div>

---

## 为什么写作需要 Skill

写作不是等灵感降临，是**工程问题**。

同样的主题，写给知乎还是公众号，结构完全不同。写给技术专家还是入门小白，深度完全不同。写给决策者还是执行者，侧重点完全不同。

大多数人每次写作都从零开始：想选题、搭结构、调语气、改措辞……重复造轮子。

**write.skill 的解法**：把每个场景的最佳实践，封装成可运行的 Agent Skill。你不需要记住 50 条写作规则，你只需要说「用知乎技术 IP skill 帮我看看这篇回答」。

---

## 三维体系：平台 × 受众 × 领域

write.skill 按三个维度组织。你可以像搭积木一样组合使用。

### 维度一：平台（Platform）

不同平台的算法、读者预期、内容寿命完全不同。

| Skill | 平台 | 核心策略 | 状态 |
|:---|:---|:---|:---|
| `zhihu-tech-ip` | 知乎 | 问题驱动、建立专业信任、面向同行工程师 | ✅ 已发布 |
| `wechat-essay` | 公众号 | 叙事节奏、情绪曲线、私域转化 | 🚧 计划中 |
| `x-tech-thread` | X/Twitter | 钩子密度、Thread 结构、传播设计 | 🚧 计划中 |
| `juejin-dev` | 掘金 | 代码片段优先、实战导向、社区互动 | 🚧 计划中 |

### 维度二：受众（Audience）

同一话题，写给不同的人，写法完全不同。

| 受众定位 | 信任来源 | 内容特征 | 典型句式 |
|:---|:---|:---|:---|
| **专家同行** | 「他真做过」 | 可验证、有细节、承认局限 | "我们在生产环境试过…" |
| **技术决策者** | 「他懂权衡」 | 决策矩阵、ROI 分析、风险预判 | "选 A 的代价是…" |
| **初级工程师** | 「他讲清楚了」 | 概念连接、循序渐进、减少跳跃 | "你可以把这个理解为…" |
| **非技术读者** | 「他说的是人话」 | 类比、故事、减少术语 | "想象你正在…" |

### 维度三：领域（Domain）

技术、商业、个人成长、科学……每个领域的论证方式和信任信号不同。

| 领域 | 核心信任信号 | 典型反模式 |
|:---|:---|:---|
| **工程技术** | 代码、数据、版本号、失败经历 | "最佳实践"（无上下文） |
| **商业分析** | 财务数据、市场案例、逻辑链完整 | "我觉得"（无证据） |
| **个人成长** | 真实经历、具体改变、坦诚局限 | "只要努力就能成功" |
| **科学研究** | 引用来源、方法论、可复现性 | "据说"/"有人说" |

---

## 核心原则

| # | 原则 | 说明 |
|:---|:---|:---|
| 01 | **场景化，不是通用化** | 不写"如何写好文章"，写"如何在知乎用工程落地内容建立专家信任" |
| 02 | **可运行，不是建议清单** | 每个 Skill 是 Agent Protocol，触发后直接执行工作流，不需要你记规则 |
| 03 | **信任优先于流量** | 专家向 Skill 宁可让 90% 的人看不懂，也要让 10% 的目标读者觉得"这正是我要的" |
| 04 | **问题驱动，不是概念驱动** | 不写"什么是 XX"，写"XX 为什么在生产环境出问题了" |
| 05 | **系列化复利** | 单篇爆款不如一个成体系的知识产品，后者是长期信任资产 |

---

## 已有 Skill

### zhihu-tech-ip：知乎技术 IP 深度写作教练

**定位**：帮技术专家在知乎建立专业信任，**不为小白写科普**。

**核心交付**：
- 选题策略：找到同行真正关心、但中文互联网缺乏深度内容的问题
- PRO 写作结构：Problem → Reason → Operation → Result
- 6 种写作武器：反直觉开头、决策显性化、失败经历前置、系列化钩子等
- 信任自检清单：确保读者读完后能带着东西去落地

**触发词**：
> 「知乎技术 IP」「知乎写作」「技术专家个人品牌」「工程落地写作」「帮我看看这篇知乎回答怎么改」

**安装**：
```bash
# 直接复制到技能目录
cp -r skills/zhihu-tech-ip ~/.agents/skills/
```

---

## 快速开始

### 方式一：作为 Agent Skill 安装

如果你使用支持 SKILL.md 格式的 Agent 工具（如 Qoder、Claude Code、Codex 等）：

```bash
# 克隆仓库
git clone https://github.com/alchaincyf/write.skill.git

# 安装你需要的 Skill
cp -r write.skill/skills/zhihu-tech-ip ~/.agents/skills/

# 在对话中触发
# "用知乎技术 IP skill 帮我看看这篇回答怎么改"
```

### 方式二：作为写作参考阅读

每个 Skill 的 `SKILL.md` 本身就是一份**该场景的深度写作指南**。即使不装在 Agent 里，直接阅读也能获得系统性的策略框架。

---

## 如何贡献

write.skill 欢迎所有领域的写作专家贡献 Skill。

### 贡献标准

一个合格的写作 Skill 必须包含：

1. **明确的触发词**：用户在什么场景下需要这个 Skill？
2. **角色定位**：你是谁？能帮什么？不能帮什么？
3. **核心心智模型**：2-5 个该场景下最重要的认知框架
4. **可执行工作流**：Step 1 → Step 2 → Step 3，不是模糊的建议
5. **示例对话**：展示 Skill 被触发后的真实交互
6. **诚实边界**：这个 Skill 做不到什么？

### 目录结构

```
skills/{skill-name}/
├── SKILL.md              # 核心文件（必须）
└── references/           # 调研来源（可选但推荐）
    └── research.md
```

### 提交 PR

1. Fork 本仓库
2. 在 `skills/` 下创建你的 Skill 目录
3. 确保 SKILL.md 通过格式自检（YAML frontmatter 完整、有触发词、有工作流）
4. 提交 PR，说明 Skill 的定位、目标读者、触发场景

---

## 路线图

| 阶段 | 目标 | 时间 |
|:---|:---|:---|
| Phase 1 | 覆盖主流中文技术社区（知乎、掘金、公众号） | 2026 Q2 |
| Phase 2 | 覆盖英文技术平台（X、Dev.to、Hacker News） | 2026 Q3 |
| Phase 3 | 覆盖商业写作（BP、研报、产品文档） | 2026 Q4 |
| Phase 4 | 覆盖创意写作（小说、剧本、叙事非虚构） | 2027 |

---

## 关于作者

write.skill 是 [女娲 Skill 造人术](https://github.com/alchaincyf/nuwa-skill) 生态的一部分。

| | |
|:---|:---|
| 🌐 官网 | [bookai.top](https://bookai.top) |
| 𝕏 Twitter | [@AlchainHust](https://x.com/AlchainHust) |
| 📺 B站 | [花叔](https://space.bilibili.com/14097567) |
| 💬 公众号 | 微信搜「花叔」 |

---

## 致谢

- [女娲 · Skill 造人术](https://github.com/alchaincyf/nuwa-skill)：提供 Skill 蒸馏的方法论框架
- [达尔文 · Skill 进化器](https://github.com/alchaincyf/darwin-skill)：提供 Skill 优化的工程化流程

---

## 许可证

MIT

---

<div align="center">

**[女娲](https://github.com/alchaincyf/nuwa-skill)** 造 Skill。<br>
**[达尔文](https://github.com/alchaincyf/darwin-skill)** 让 Skill 进化。<br>
**write.skill** 让写作成为工程。<br><br>

*好的写作不是天赋，是可复用的系统。*

<br>

MIT License © [花叔 Huashu](https://github.com/alchaincyf)

</div>
