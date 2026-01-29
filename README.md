# Teaching at Scale

A methodology for developing and delivering professional certificate programs using structured workflows and automation.

---

## What This Is

This is the **hub** for a system that turns curriculum development from manual, ad-hoc work into repeatable, scalable processes.

If you're here, you probably want one of these:

| I want to... | Go to... |
|--------------|----------|
| **Build course content** (slides, speaker notes) | [curriculum-dev-kit](https://github.com/{your-username}/curriculum-dev-kit) |
| **Automate post-recording** (transcripts, chapters, recaps) | [recording-pipeline](https://github.com/{your-username}/recording-pipeline) |
| **Understand the philosophy** | Keep reading, then see [Conversation Context](project-management/CONVERSATION-CONTEXT.md) |
| **Learn from real delivery experience** | [Lessons Learned](project-management/LESSONS-LEARNED.md) |

---

## The System

```
┌─────────────────────────────────────────────────────────────────────────────┐
│                           TEACHING AT SCALE                                  │
│                                                                             │
│   ┌─────────────────────────────────────────────────────────────────────┐   │
│   │                        BEFORE YOU RECORD                             │   │
│   │                                                                      │   │
│   │   Content Audit → Research → Brief → Slides + Notes                  │   │
│   │                                                                      │   │
│   │   📦 curriculum-dev-kit                                              │   │
│   │      Templates, workflows, and scripts for building course content   │   │
│   └─────────────────────────────────────────────────────────────────────┘   │
│                                    │                                         │
│                                    ▼                                         │
│                            [ LIVE DELIVERY ]                                 │
│                                    │                                         │
│                                    ▼                                         │
│   ┌─────────────────────────────────────────────────────────────────────┐   │
│   │                        AFTER YOU RECORD                              │   │
│   │                                                                      │   │
│   │   Recording → Transcript → Chapters → Recap → Promises               │   │
│   │                                                                      │   │
│   │   📦 recording-pipeline                                              │   │
│   │      Automated post-production: 1 recording → 5 outputs              │   │
│   └─────────────────────────────────────────────────────────────────────┘   │
│                                                                             │
│   ┌─────────────────────────────────────────────────────────────────────┐   │
│   │                     PHILOSOPHY & GOVERNANCE                          │   │
│   │                                                                      │   │
│   │   📄 teaching-at-scale (this repo)                                   │   │
│   │      Why this approach works. Lessons from 50+ modules delivered.    │   │
│   └─────────────────────────────────────────────────────────────────────┘   │
│                                                                             │
└─────────────────────────────────────────────────────────────────────────────┘
```

---

## The Core Insight

**Manual curriculum development doesn't scale.**

When you're running multiple cohorts, producing 50+ modules, and recording 60+ hours of live instruction, you need infrastructure. You need:

- **Repeatable workflows** — So every module hits the same quality bar
- **Templates that encode decisions** — So you're not reinventing structure each time
- **Automation for mechanical work** — So human effort goes to teaching, not transcription
- **Documentation that transfers** — So someone else can pick up where you left off

This repo and its siblings document that infrastructure.

---

## Implementation Repos

| Repo | What It Does | Status |
|------|--------------|--------|
| [curriculum-dev-kit](https://github.com/{your-username}/curriculum-dev-kit) | 4-phase workflow for building course modules: Content Audit → Research → Brief → Production. Templates for topic outlines, presentation briefs, speaker notes, and HTML slides. | Complete |
| [recording-pipeline](https://github.com/{your-username}/recording-pipeline) | Automated post-production: one recording becomes transcript + clean text + YouTube chapters + LMS recap + promise extraction. GPU-accelerated, Discord-notified. | Complete |
| ai-memory-stack | Multi-AI coordination with persistent memory via Qdrant. Council reviews, session handoffs, inter-AI protocols. | Planned |

---

## The Workflow (Overview)

Every module goes through four phases:

```
Phase 1: Content Audit   → What needs to be taught?
Phase 2: Research        → What does the evidence say? (optional for rework)
Phase 3: Brief           → What are we committing to build?
Phase 4: Production      → Build slides, notes, record, publish
```

**For the full workflow with templates:** See [curriculum-dev-kit](https://github.com/{your-username}/curriculum-dev-kit)

**For post-recording automation:** See [recording-pipeline](https://github.com/{your-username}/recording-pipeline)

---

## What's In This Repo

This hub repo contains the **philosophy and governance** that connects the implementation repos.

```
teaching-at-scale/
├── README.md                           # You are here (the hub)
├── project-management/
│   ├── CONVERSATION-CONTEXT.md         # Origin story and key decisions
│   └── LESSONS-LEARNED.md              # What actually works in practice
└── methodology/
    └── 4-phase-workflow.md             # Workflow overview (detailed version in curriculum-dev-kit)
```

### Start Here

| Document | What It Covers |
|----------|----------------|
| [Conversation Context](project-management/CONVERSATION-CONTEXT.md) | Why this methodology exists. The decisions that shaped it. How it evolved from "just teaching" to "teaching at scale." |
| [Lessons Learned](project-management/LESSONS-LEARNED.md) | What works and what doesn't — from 50+ modules of real delivery to adult learners in workforce development. |

---

## Proof Points

| Metric | Value |
|--------|-------|
| Active teaching programs | 5 |
| Course modules developed | 50+ |
| Class recordings processed | 100+ |
| Python automation scripts | 50+ |
| Concurrent cohorts managed | 2 |

---

## Background

This methodology was developed by educators working in higher education and professional development.

**Current work includes:**
- Project management certification programs
- AI fundamentals training
- AI in manufacturing contexts
- Power BI data analytics, dashboards, and DAX (beginner to intermediate)

The throughline: taking complex, repeatable processes and building systems around them.

---

## How to Navigate

**If you're an instructional designer:**
Start with [curriculum-dev-kit](https://github.com/{your-username}/curriculum-dev-kit) — the templates and workflow.

**If you're technical:**
Start with [recording-pipeline](https://github.com/{your-username}/recording-pipeline) — the automation scripts.

**If you're curious about the thinking:**
Start with [Conversation Context](project-management/CONVERSATION-CONTEXT.md) — why this exists and how it evolved.

**If you're curious about outcomes:**
Start with [Lessons Learned](project-management/LESSONS-LEARNED.md) — what actually works in practice.

---

## Related

| Related Repo | What It Covers |
|--------------|----------------|
| [recording-pipeline](https://github.com/{your-username}/recording-pipeline) | Post-recording automation (after you record) |
| [curriculum-dev-kit](https://github.com/{your-username}/curriculum-dev-kit) | Pre-recording content development (before you record) |
| teaching-at-scale | Philosophy, governance, and lessons learned (this repo) |

---

*This is the hub. The implementations are in the repos. The lessons are in the docs.*
