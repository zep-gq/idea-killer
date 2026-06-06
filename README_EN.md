<div align="center">

# 🔪 Idea Killer

### _Kill fast. Kill often. Kill before you invest time._

**Kill bad ideas with data. Save your time for the good ones.** 🔪💡

A structured startup idea evaluation tool — helping solo founders (OPCs) and small teams<br>kill bad ideas fast with real data, before wasting a single weekend.

[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)

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

## 🚀 Installation

### Option 1: One-liner

```bash
npx skills add zephyrgq/idea-killer
```

Supports 55+ AI agent runtimes (Claude Code, Codex, Cursor, Gemini CLI, etc.). Specify a runtime with `-a`:

```bash
npx skills add zephyrgq/idea-killer -a claude-code
```

### Option 2: Manual install

```bash
git clone https://github.com/zephyrgq/idea-killer.git
```

Place the `idea-killer` directory in your agent's skills directory. Common paths:

| Runtime | Skills Directory |
|---------|------------------|
| Claude Code | `~/.claude/skills/` |
| Cursor | `.cursor/skills/` |
| Codex | `.codex/skills/` |
| Others | Check your runtime's docs |

### Option 3: Direct use

Even if your runtime doesn't support the skills protocol, just paste `SKILL.md` content into your conversation — it's just a markdown document.

<br>

## 🎯 Triggering

Idea Killer auto-triggers when you describe a startup or product idea:

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

## 📋 Real Case Studies

> These are real evaluations performed by Idea Killer. All conclusions are backed by searched market data.

---

### 🔴 Case 1: Anonymous Social Confession App — Deep Mode

**Idea**: A platform where anyone can anonymously share emotions and secrets. Solo founder, weekend project.

**Verdict: 🔴 Kill it**

| Model | Result | Key Finding |
|-------|--------|-------------|
| 🚦 Traffic Light | 🔴 Kill | 3 red lights (differentiation, willingness to pay, OPC feasibility), 0 green |
| 🏗️ Domain Check | 🔴 High risk | Social: content moderation costs spiral + cyberbullying + compliance red lines |
| 📊 Value-Complexity | 🔴 No point | Low value × high complexity — worst quadrant |
| ⚔️ Five Forces | 🔴 Hostile | All 5 dimensions unfavorable |
| 💀 Fatal Assumptions | 🔴 Failed | 3 of 5 fatal assumptions likely invalid |
| 📋~⚡ | ⏭️ Skipped | Early termination: verdict already clear |

**Agent Research Findings**:
- ~90% mortality rate: Secret, Yik Yak, Sarahah, Formspring all shut down
- 100% of failures linked to content moderation / safety management failure
- All successes relied on piggybacking large platforms (NGL → Instagram, Sendit → Snapchat)

**Silver Linings & Pivots**:

> 💡 The "emotional need" direction is right — the vehicle is wrong.

| Pivot | Description | Feasibility |
|-------|-------------|-------------|
| 🅰️ Anonymous interaction mini-app | Don't build standalone — use WeChat mini-program, offload moderation | ⭐⭐⭐ |
| 🅱️ Vertical anonymous venting | Focus on devs / exam prep / specific communities — lower moderation burden | ⭐⭐⭐ |
| 🅲️ **AI emotional companion (highly recommended)** | Remove social — user vents, AI responds. No moderation, no cold start, weekend-buildable | ⭐⭐⭐⭐⭐ |

> 🪞 _"Do users want 'anonymous socializing' or 'a judgment-free space'? If the latter, AI companionship may serve the need better — without the moderation nightmare."_

---

### 🟡 Case 2: AI Therapy Chatbot — Quick Mode

**Idea**: An AI chatbot that uses psychological methods to help people manage anxiety and low moods. Solo founder, weekend project.

**Verdict: 🟡 Needs Validation**

| Dimension | Light | Reasoning |
|-----------|-------|-----------|
| Necessity | 🟡 | Real demand but many alternatives (Calm, Headspace, Character.ai) |
| Differentiation | 🟡 | More interactive than meditation apps, cheaper than real therapy — but Woebot/Wysa exist |
| Reachability | 🟢 | "Anxiety" and "mental health" are search hotspots, clear content marketing path |
| Willingness to Pay | 🟡 | Category has paying users (Calm $69.99/yr), but "AI chat therapy" payment habit unproven |
| OPC Feasibility | 🟡 | Tech ✅ + Ops ✅ (1-to-1 chat needs no moderation) + Compliance ⚠️ (mental health gray zone) |

**Domain Check Triggered**:

```
Matched domains: 🤖 AI/Data + 🏥 Healthcare

⚠️ Compliance risks:
  • Generative AI requires filing (China's "Interim Measures")
  • Must position as "emotional support tool", not "diagnosis/treatment"
  • AI output causing delayed medical care = potential legal liability
```

**Levels Quick Validation**: 3/3 ✅

| Pivot | Description |
|-------|-------------|
| 🅰️ Vertical AI companion | "Exam anxiety buddy" or "new mom emotional support" — narrower = lower compliance risk |
| 🅱️ **AI mood journal** | Users write, AI gives psychology-framework feedback. Lighter product, lower risk |
| 🅲️ Launch overseas first | FDA is lenient on "wellness" apps — validate abroad, then consider China |

---

### 🟢 Case 3: Chrome Extension — Auto Price Comparison for Cross-Border Sellers — Quick Mode

**Idea**: A Chrome extension that automatically shows Amazon prices and profit margins when sellers browse 1688/Taobao.

**Verdict: 🟢 Go for it**

| Dimension | Light | Reasoning |
|-----------|-------|-----------|
| Necessity | 🟢 | Core pain point — manual price comparison is extremely time-consuming |
| Differentiation | 🟢 | 1688 → Amazon auto-comparison has no direct competitor |
| Reachability | 🟢 | Sellers cluster in TikTok/WeChat groups/Zhihu — precise targeting |
| Willingness to Pay | 🟢 | Sellers already pay for ERP tools ($20-50/mo) — paying habit established |
| OPC Feasibility | 🟢 | Chrome extension + simple API, weekend-buildable |

**Levels Quick Validation**: 3/3 ✅

**Recommendation**: Build MVP immediately, validate in one cross-border seller WeChat group.

---

### ⚔️ Case 4: College Student Skill Swap Platform — Deep Mode

**Idea**: A platform where college students can exchange skills (PS, coding, English) with each other, no money involved. 3-person team.

**Verdict: 🟡 Modify and Proceed**

| Model | Result | Key Finding |
|-------|--------|-------------|
| 🚦 Traffic Light | 🟡 Validate | Necessity 🟢 + Differentiation 🟡 + Reach 🟢 + WTP 🔴 + Team Feasibility 🟢 |
| 🏗️ Domain Check | 🟡 Social + Education | Cold start valley + campus promotion costs |
| 📊 Value-Complexity | 🟡 Fill | Medium value × medium complexity |
| ⚔️ Five Forces | 🟡 Average | Many substitutes (clubs, Xianyu, WeChat groups), but free skill swap is untapped |
| 💀 Fatal Assumptions | ⚠️ Uncertain | "Students prefer skill swapping over paying" — needs validation |

**Key Risk**: Willingness to pay is red — pure free model has no revenue. Need a value-added monetization path.

**Recommended Modification**: Don't do "skill swap" — do "skill paid + first lesson free trial" — preserves community feel but has clear monetization.

---

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

## 🛡️ License

MIT License — Free to use, modify, and distribute.
