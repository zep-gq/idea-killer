<div align="center">

# 🔪 Idea Killer

### _Kill fast. Kill often. Kill before you invest time._

**A structured startup idea evaluation tool** — helping solo founders (OPCs) and small teams<br>kill bad ideas fast with real data, before wasting a single weekend.

[![Version](https://img.shields.io/badge/version-1.2.0-blue.svg)](https://github.com/zep-gq/idea-killer)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![Made for Claude Code](https://img.shields.io/badge/Made%20for-Claude%20Code-orange.svg)](https://claude.com/claude-code)

English · [中文](README.md)

</div>

---

<br>

## ✨ Core Belief

> **90%+ of ideas should be killed in the first 5 minutes.**
> If you can't build it in a weekend, can't run it alone, and can't back it with real data — it's a bad idea.
> Killing fast beats picking right. Killing ≠ rejecting — but hesitating = wasting time.

<br>

## 🧩 Features at a Glance

| | | |
|:---:|:---:|:---:|
| ⚡ **Dual Mode** | 👥 **Dual Perspective** | 📊 **8 Evaluation Models** |
| Quick (5-min verdict)<br>Deep (full research + report) | OPC (Solo Founder)<br>Team | Traffic Light → Domain Check → Value Matrix<br>Five Forces → Fatal Assumptions → Lean Canvas<br>RICE → Levels Validation |
| | | |
| 🏗️ **12 Industry Checks** | 🔍 **3 Research Agents** | 🌏 **Region Adaptive** |
| Social · Fintech · Healthcare · Education<br>E-commerce · Media · SaaS · AI<br>Food · Real Estate · Transport · Gaming | Competitor Research<br>Case Studies<br>MVP Theory | Chinese/English search strategy<br>Auto-switches based on target market |

<br>

## 🚀 Quick Start

### Installation

Place the `idea-killer` directory in your Claude Code skills path.

### Triggering

In Claude Code conversations, the following phrases will auto-trigger the skill:

```
"Help me evaluate this idea"
"Is this idea worth pursuing?"
"I want to build a..."
"Should I build this?"
"Take a look at this direction"
```

### Quick Mode — 5-Minute Verdict

```
💬 You: "Quick check — I want to build a freelance job board for developers"

🔪 Idea Killer:
   → Traffic Light evaluation ✅🟡🔴
   → Domain risk scan
   → Fatal assumption check
   → Levels quick validation
   → Verdict + Silver linings + Pivot directions
```

### Deep Mode — Full Research + MVP Document

```
💬 You: "Deep evaluate this — I want to build an AI therapy chatbot, solo founder, weekend project"

🔪 Idea Killer:
   → Launch 3 research agents in parallel (competitors / cases / MVP theory)
   → Sequential analysis through 8 evaluation models
   → Terminal summary + MVP document saved to working directory
```

<br>

## 📐 Evaluation Flow

### Quick Mode

```
User describes idea
    │
    ▼
🚦 Traffic Light (5 dimensions)
    │
    ├── 🔴 Multiple reds → Kill immediately
    │
    ├── 🟡 Domain risk scan → High-risk industry?
    │
    └── 🟢 / Few yellows
         │
         ▼
    💀 Fatal Assumptions quick check
         │
         ▼
    ⚡ Levels Quick Validation (3 questions)
         │
         ▼
    📋 Quick Assessment Report
```

### Deep Mode

```
User describes idea
    │
    ▼
Confirm perspective + extract core info
    │
    ├─────┬─────┐
    ▼     ▼     ▼
  🔎Competitors 📖Cases 🧪MVP    ← 3 Agents search in parallel
    │     │     │
    └─────┴─────┘
          │
          ▼
    Data reliability check ⚠️
          │
          ▼
  1. 🚦 Traffic Light
  2. 🏗️ Domain Check        ← NEW: 12 industries × compliance + risks
  3. 📊 Value-Complexity
  4. ⚔️ Five Forces
  5. 💀 Fatal Assumptions   ← Early termination possible
  ─ ─ ─ ─ ─ ─ ─ ─
  6. 📋 Lean Canvas
  7. 🎯 RICE Prioritization
  8. ⚡ Levels Validation
          │
          ▼
    📄 Terminal Summary + MVP Document
```

<br>

## 🧠 Evaluation Models

| # | Model | File | One-Liner |
|---|-------|------|-----------|
| 1 | 🚦 Traffic Light | `models/traffic-light.md` | Must-build, could-build, or don't-build? |
| 2 | 🏗️ Domain Check | `models/domain-check.md` | What industry-specific traps await? |
| 3 | 📊 Value-Complexity | `models/value-complexity.md` | Is the ROI worth it? |
| 4 | ⚔️ Five Forces | `models/five-forces.md` | Is the market landscape favorable? |
| 5 | 💀 Fatal Assumptions | `models/fatal-assumptions.md` | Can your core assumptions hold up? |
| 6 | 📋 Lean Canvas | `models/lean-canvas.md` | Have you thought through the business model? |
| 7 | 🎯 RICE Prioritization | `models/rice.md` | If you build it, where do you start? |
| 8 | ⚡ Levels Validation | `models/levels-method.md` | Can you validate it in a weekend? |

<br>

## 📂 Project Structure

```
idea-killer/
├── 📄 SKILL.md                          # Main entry point
├── 📁 agents/                           # Research Agents (Deep mode only)
│   ├── competitor-research.md           #   Competitors + death list
│   ├── case-study.md                    #   Success/failure cases
│   └── mvp-theory.md                    #   MVP methodology
├── 📁 models/                           # Evaluation models
│   ├── traffic-light.md                 #   Traffic Light (tech + ops + compliance)
│   ├── domain-check.md                  #   Domain-specific (12 industries × 4 dims)
│   ├── value-complexity.md              #   Value-Complexity Matrix
│   ├── five-forces.md                   #   Porter's Five Forces
│   ├── fatal-assumptions.md             #   Fatal Assumptions
│   ├── lean-canvas.md                   #   Lean Canvas
│   ├── rice.md                          #   RICE Prioritization
│   └── levels-method.md                 #   Levels Quick Validation
├── 📁 modes/                            # Execution modes
│   ├── quick.md                         #   Quick flow (5 min)
│   └── deep.md                          #   Deep flow (full research)
└── 📁 templates/                        # Output templates
    ├── quick-report.md                  #   Quick assessment report
    ├── deep-report.md                   #   Deep assessment summary
    └── mvp-doc.md                       #   MVP document (core + extended)
```

<br>

## ⚖️ Iron Rules

> 🔴 **No research, no opinion** — Every conclusion must be backed by searched data
>
> ⚡ **Kill fast, not accurately** — Stop at red lights, don't try to save a bad idea
>
> ⏱️ **Can you ship it in a weekend?** — OPC standard; teams get two weeks
>
> 🌐 **Follow the user's language** — Respond in whatever language the user speaks
>
> 💡 **Killing ≠ rejecting** — Even when recommending to drop, acknowledge silver linings and offer pivot directions

<br>

## 📜 Version History

| Version | Date | Description |
|---------|------|-------------|
| **v1.2.0** | 2026-06-06 | 🏗️ Domain-specific checks (12 industries) + Agent region adaptation + Data reliability safeguards + 3D OPC feasibility |
| **v1.1.0** | 2026-06-06 | 👥 Dual perspective support (OPC / Team) + Missing files added |
| **v1.0.0** | 2026-06-06 | 🎉 Initial release: dual mode + 7 models + 3 agents |

<br>

## 🛡️ License

MIT License — Free to use, modify, and distribute.

---

<div align="center">

**Kill bad ideas with data. Save your time for the good ones.** 🔪💡

</div>
