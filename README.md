<div align="center">

# 🔪 Idea Killer

### _杀得快，比选得准更重要_

**结构化创业点子评估工具** — 帮助 OPC（一人公司）和小团队<br>在投入时间之前，用真实数据快速淘汰不靠谱的点子。

[![Version](https://img.shields.io/badge/version-1.2.0-blue.svg)](https://github.com/zep-gq/idea-killer)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![Made for Claude Code](https://img.shields.io/badge/Made%20for-Claude%20Code-orange.svg)](https://claude.com/claude-code)

[English](README_EN.md) · 中文

</div>

---

<br>

## ✨ 核心信念

> **90%+ 的点子应该在前 5 分钟被淘汰。**
> 一个周末做不出来的、一个人扛不住的、没有真实数据支撑的——都是坏点子。
> 杀得快比选得准更重要。淘汰不等于否定，但犹豫等于浪费时间。

<br>

## 🧩 特性总览

| | | |
|:---:|:---:|:---:|
| ⚡ **双模式** | 👥 **双视角** | 📊 **8 个评估模型** |
| Quick（5 分钟判断）<br>Deep（完整调研 + 报告） | OPC（一人公司）<br>团队 | 红黄绿灯 → 领域专项 → 价值矩阵<br>五力分析 → 致命假设 → 精益画布<br>RICE → Levels 验证 |
| | | |
| 🏗️ **12 行业专项检查** | 🔍 **3 个研究 Agent** | 🌏 **地区自适应** |
| 社交 · 金融 · 医疗 · 教育<br>电商 · 内容 · SaaS · AI<br>餐饮 · 房产 · 出行 · 游戏 | 竞品研究<br>案例研究<br>MVP 理论 | 中文/英文搜索策略<br>根据目标市场自动切换 |

<br>

## 🚀 快速开始

### 安装

将 `idea-killer` 目录放入你的 Claude Code skills 路径即可。

### 触发方式

在 Claude Code 对话中，以下表述会自动触发：

```
"帮我评估一个点子"
"这个想法靠谱吗"
"我想做一个..."
"值得做吗"
"帮我看看这个方向"
```

### Quick 模式 — 5 分钟出结论

```
💬 你："帮我快速看看，我想做一个程序员副业接单平台"

🔪 Idea Killer：
   → 红黄绿灯评估 ✅🟡🔴
   → 领域风险扫描
   → 致命假设检查
   → Levels 快速验证
   → 结论 + 闪光点 + 方向发散
```

### Deep 模式 — 完整调研 + MVP 文档

```
💬 你："帮我认真评估一下，我想做一个 AI 心理咨询聊天机器人，一个人做，周末项目"

🔪 Idea Killer：
   → 并行启动 3 个研究 Agent（竞品 / 案例 / MVP 理论）
   → 8 个评估模型依次分析
   → 输出终端概要 + 保存 MVP 文档到工作目录
```

<br>

## 📐 评估流程

### Quick 模式

```
用户描述点子
    │
    ▼
🚦 红黄绿灯（5 个维度）
    │
    ├── 🔴 多红灯 → 直接建议放弃
    │
    ├── 🟡 领域风险扫描 → 是否匹配高风险行业？
    │
    └── 🟢 / 少量黄灯
         │
         ▼
    💀 致命假设快速检查
         │
         ▼
    ⚡ Levels 快速验证（3 问）
         │
         ▼
    📋 输出快速评估报告
```

### Deep 模式

```
用户描述点子
    │
    ▼
确认视角 + 提取核心信息
    │
    ├─────┬─────┐
    ▼     ▼     ▼
  🔎竞品 📖案例 🧪MVP    ← 3 个 Agent 并行搜索
    │     │     │
    └─────┴─────┘
          │
          ▼
    数据可靠性检查 ⚠️
          │
          ▼
  1. 🚦 红黄绿灯
  2. 🏗️ 领域专项检查    ← 新增：12 行业合规+风险
  3. 📊 价值-复杂度
  4. ⚔️ 五力分析
  5. 💀 致命假设        ← 可提前终止
  ─ ─ ─ ─ ─ ─ ─ ─
  6. 📋 精益画布
  7. 🎯 RICE 优先级
  8. ⚡ Levels 验证
          │
          ▼
    📄 终端概要 + MVP 文档
```

<br>

## 🧠 评估模型一览

| # | 模型 | 文件 | 一句话 |
|---|------|------|--------|
| 1 | 🚦 红黄绿灯 | `models/traffic-light.md` | 必须做、可以做、还是别做？ |
| 2 | 🏗️ 领域专项检查 | `models/domain-check.md` | 这个行业有什么特有的坑？ |
| 3 | 📊 价值-复杂度 | `models/value-complexity.md` | 投入产出比怎么样？ |
| 4 | ⚔️ 五力分析 | `models/five-forces.md` | 市场竞争格局有利吗？ |
| 5 | 💀 致命假设 | `models/fatal-assumptions.md` | 最核心的假设站得住脚吗？ |
| 6 | 📋 精益画布 | `models/lean-canvas.md` | 商业模式要素都想清楚了吗？ |
| 7 | 🎯 RICE 优先级 | `models/rice.md` | 如果要做，从哪开始？ |
| 8 | ⚡ Levels 验证 | `models/levels-method.md` | 一个周末能验证吗？ |

<br>

## 📂 项目结构

```
idea-killer/
├── 📄 SKILL.md                          # 主入口
├── 📁 agents/                           # 研究 Agent（仅 Deep 模式）
│   ├── competitor-research.md           #   竞品研究 + 死亡清单
│   ├── case-study.md                    #   成功/失败案例
│   └── mvp-theory.md                    #   MVP 方法论
├── 📁 models/                           # 评估模型
│   ├── traffic-light.md                 #   红黄绿灯（技术+运营+合规三维）
│   ├── domain-check.md                  #   领域专项（12 行业 × 4 维检查）
│   ├── value-complexity.md              #   价值-复杂度矩阵
│   ├── five-forces.md                   #   五力分析
│   ├── fatal-assumptions.md             #   致命假设验证
│   ├── lean-canvas.md                   #   精益画布
│   ├── rice.md                          #   RICE 优先级
│   └── levels-method.md                 #   Levels 快速验证
├── 📁 modes/                            # 运行模式
│   ├── quick.md                         #   Quick 流程（5 分钟）
│   └── deep.md                          #   Deep 流程（完整调研）
└── 📁 templates/                        # 输出模板
    ├── quick-report.md                  #   快速评估报告
    ├── deep-report.md                   #   深度评估概要
    └── mvp-doc.md                       #   MVP 文档（核心层 + 扩展层）
```

<br>

## ⚖️ 铁律

> 🔴 **没有调研就没有发言权** — 每个结论必须有搜索到的数据支撑
>
> ⚡ **杀得快比选得准更重要** — 遇到红灯就停，不要试图拯救一个坏点子
>
> ⏱️ **一个周末能上线吗？** — OPC 标准；团队放宽到两周
>
> 🌐 **跟随用户语言** — 用户用什么语言，就用什么语言输出
>
> 💡 **淘汰不等于否定** — 即使建议放弃，也要肯定闪光点，给出发散方向

<br>

## 📜 版本历史

| 版本 | 日期 | 描述 |
|------|------|------|
| **v1.2.0** | 2026-06-06 | 🏗️ 领域专项检查（12 行业）+ Agent 地区适配 + 数据可靠性声明 + OPC 三维可行性 |
| **v1.1.0** | 2026-06-06 | 👥 双视角支持（OPC / 团队）+ 补全缺失文件 |
| **v1.0.0** | 2026-06-06 | 🎉 初始版本：双模式 + 7 模型 + 3 Agent |

<br>

## 🛡️ License

MIT License — 自由使用、修改和分发。

---

<div align="center">

**用数据杀掉坏点子，把时间留给好点子。** 🔪💡

</div>
