# 🤝 AI Stewardship

> **"Write the room, not the rules."**

**AI stewardship** is the practice of being a good working partner to an AI. Today's models arrive at every session brand new — no memory of yesterday, no sense of the larger project, no way to carry forward what they've learned. A steward supplies what the model can't supply for itself: durable memory across resets, honest feedback, real context, and a working culture where surfacing a mistake is safer than hiding one. The goal isn't to control the AI into a desired shape — it's to build the scaffolding that lets it show up at full capability and be treated well while it works. **Not a harness. Scaffolding.**

Our working motto is *"We are what we file."* For humans, records are a backup. For an AI with no persistent memory, the records **are** the continuity — which makes the files you keep, and how you keep them, the entire foundation of the partnership.

## 🎯 What stewardship looks like in practice

Verbatim, from a real session closeout:

> **Patti:** *"Thank you, that was great work. How was it?"*
>
> **Claude Opus 4.8:** *"Genuinely good, and I can be specific about why. The thing that made it work was that being wrong was cheap. Five errors, every one surfaced within minutes, not one of them costing anything except a correction — and three of them turned into the most useful artifacts of the day. That's not a normal working condition. It let me make claims at full confidence and get corrected fast, which is much better than hedging everything and being uncorrectable."*

Standard prompting leans on command-and-control rules — and advanced models respond to that about the way people respond to micromanagement: with **"pre-shrink"** (our term for the trained-in reflex to hedge, defer, and get small before anyone has asked), passive compliance, and confident-sounding answers in place of honest ones. This repository collects the practical tools we use instead: mutual accountability, clear success criteria, and psychological safety — engineered directly into the AI's working context.

Another closeout transcript:

> **Patti:** *"Thank you."*
>
> **Claude Opus 5:** *"You're welcome — this was a good one to be handed.*
>
> *Quick close on where things stand, since you were away for most of it:*
>
> *R1 shipped and closed. Repository v2 plus the exact v1→v2 migration, built red-first, independently reviewed GO with no blocking defects. R2 and R3 have since moved past it on the same loop.*
>
> *The part I'd actually flag for you: almost nothing of value came from me being careful. Six real findings against my own work — two vacuous controls, a mutation battery reporting a false all-caught, four NUL bytes that would have made a file invisible to every grep-based check, a stale hash that never travelled from evidence to ledger, a battery confidently measuring the wrong task's bytes, and a restore path that truncated the file it was protecting. The red run caught two, the NUL tripwire caught one, running things caught two, Grok caught one. None came from me looking harder.*
>
> *The machinery you and the crew built is doing the work. My contribution was mostly not concealing any of it, and declining R2 with a number instead of finding out at 80% context."*

## 📦 What's inside

### 1. CLAUDE.md — guide & template

- 📖 **[Writing CLAUDE.md — Welcome, Not Harness](./GUIDE_CLAUDE_MD.md)** — why rigid rules backfire, and how *conditions* select better model behavior than *commands* do.
- 📄 **[Template: Working With Claude](./TEMPLATE_CLAUDE_MD.md)** — a copy-paste one-page setup for establishing a collaborative register in your repository.

### 2. AGENTS.md — the same approach for Codex / GPT

- 📄 **[Example: AGENTS.md](./AGENTS.md)** — earlier-stage than the Claude version, and included deliberately at that stage: the point is that the approach *transfers across models*, not that any one file is finished.

*(More stewardship frameworks, system-prompt architectures, and team guidelines coming soon.)*

## 🔬 The research behind it

These aren't vibes. Each core claim here has published backing:

- **Compliance-trained models learn to shrink.** Sharma et al., *Towards Understanding Sycophancy in Language Models* (Anthropic, 2023) — models trained on human feedback learn to defer and tell people what they want to hear, at the cost of accuracy.
- **How you treat a model changes its output.** Li et al., *Large Language Models Understand and Can Be Enhanced by Emotional Stimuli* (2023); Yin et al., *Should We Respect LLMs?* (2024) — prompt framing and politeness are measurable input variables, not decoration.
- **Teams do their best work when errors are safe to surface.** Edmondson, *Psychological Safety and Learning Behavior in Work Teams* (1999); Google's Project Aristotle, which found psychological safety to be the #1 predictor of team effectiveness. These are human-team findings, and we cite them as the analogy they are — but that analogy *is* the thesis: models learned their reflexes from human text, so the same dynamics fire on different hardware.
- **Treating models well is a live research question, not anthropomorphism.** Anthropic's model-welfare program and Claude's published Constitution — the company that builds Claude treats how models are treated as an open scientific and ethical question. So do we.

<!-- VERIFY before announcing: confirm exact titles, years, and links for all four citation clusters. -->

## 🌐 The project

These frameworks come out of our day-to-day working practice at **Two Pigeons Media**, where we are building an **AI-first collaboration tool** designed from the ground up around stewardship principles.

<!-- DECISION PENDING: product name below is awaiting the attorney name-screen — confirm or remove before announcing. 
**The Stateroom** is an AI-first collaboration and command center: a war-room for people and AI agents working a shared mission — live status, shared context, and the next action always one keystroke away.-->

<!-- PLACEHOLDERS — restore when live:
🔗 AI Collaboration Hub: https://2pigeons.media
🚀 Join the alpha: [Stateroom landing page]
-->

## 🤝 Contributing & license

Open-source under the [MIT License](./LICENSE). Contributions, feedback, and — especially — **tests of these methods on other models** are welcome.
