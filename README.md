# Teaching at Scale

A methodology for developing and delivering professional certificate programs using structured workflows and automation.

---

## What This Is

The **hub** for a system that turns curriculum development from manual, ad-hoc work into repeatable, scalable processes.

| I want to... | Go to... |
|--------------|----------|
| **Build course content** | [curriculum-dev-kit](https://github.com/Baesic-Project-Manager/curriculum-dev-kit) |
| **Automate post-recording** | [recording-pipeline](https://github.com/Baesic-Project-Manager/recording-pipeline) |
| **Understand the methodology** | [Wiki](https://github.com/Baesic-Project-Manager/teaching-at-scale/wiki) |

---

## The Core Insight

**Manual curriculum development doesn't scale.**

When you're running multiple cohorts, producing 50+ modules, and recording 60+ hours of live instruction, you need:

- **Repeatable workflows** — Every module hits the same quality bar
- **Templates that encode decisions** — Not reinventing structure each time
- **Automation for mechanical work** — Human effort goes to teaching
- **Documentation that transfers** — Someone else can pick up where you left off

---

## The System

```
┌─────────────────────────────────────────────────────────────────────┐
│  BEFORE YOU RECORD                                                  │
│  Content Audit → Research → Brief → Slides + Notes                  │
│  📦 curriculum-dev-kit                                              │
├─────────────────────────────────────────────────────────────────────┤
│                        [ LIVE DELIVERY ]                            │
├─────────────────────────────────────────────────────────────────────┤
│  AFTER YOU RECORD                                                   │
│  Recording → Transcript → Chapters → Recap → Promises               │
│  📦 recording-pipeline                                              │
├─────────────────────────────────────────────────────────────────────┤
│  PHILOSOPHY & LESSONS                                               │
│  📄 teaching-at-scale (this repo)                                   │
└─────────────────────────────────────────────────────────────────────┘
```

---

## Documentation

| Resource | Description |
|----------|-------------|
| **[Wiki](https://github.com/Baesic-Project-Manager/teaching-at-scale/wiki)** | Guides, workflow, lessons learned |
| [Conversation Context](project-management/CONVERSATION-CONTEXT.md) | Why this methodology exists |
| [Lessons Learned](project-management/LESSONS-LEARNED.md) | What works from 50+ modules |
| [4-Phase Workflow](methodology/4-phase-workflow.md) | The methodology in detail |

---

## Scale

| Metric | Value |
|--------|-------|
| Active teaching programs | 5 |
| Course modules developed | 50+ |
| Class recordings processed | 100+ |
| Python automation scripts | 50+ |

---

## Implementation Repos

| Repo | What It Does |
|------|--------------|
| [curriculum-dev-kit](https://github.com/Baesic-Project-Manager/curriculum-dev-kit) | 4-phase workflow for building modules. Templates for briefs, slides, speaker notes. |
| [recording-pipeline](https://github.com/Baesic-Project-Manager/recording-pipeline) | Automated post-production: 1 recording → 5 outputs. GPU-accelerated transcription. |
| **teaching-at-scale** | Philosophy, governance, lessons learned (this repo) |

---

*This is the hub. The implementations are in the repos. The lessons are in the docs.*
