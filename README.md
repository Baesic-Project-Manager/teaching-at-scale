# Teaching at Scale

A methodology for developing and delivering multiple concurrent curriculum programs using structured workflows and automation.

---

## What This Is

This repository documents how I manage 5+ active teaching programs across community colleges, state workforce agencies, and K-12 systems—simultaneously. It's not a course repository; it's a **system for creating courses**.

The core insight: manual curriculum development doesn't scale. When you're running multiple cohorts, producing 50+ modules, and recording 60+ hours of live instruction, you need infrastructure. This repo documents that infrastructure.

---

## Who I Am

**Matt Behar** | Instructional Designer & Course Facilitator

Currently at SCSU OWLL (Office of Workforce and Lifelong Learning), teaching:
- Google Project Management Professional Certificate (6 courses, 30 modules)
- AI Fundamentals (5 courses, 20 modules)
- AI in Manufacturing (CT Tech Talent Accelerator grant, $30,000)

Previously: Digital marketing automation at enterprise scale (Eloqua, Monday.com).

The throughline: taking complex, repeatable processes and building systems around them.

---

## What's Here

### `/project-management/`
Active development tracking using a structured workflow:
- **CONVERSATION-CONTEXT.md** — Why this methodology exists and how it evolved
- **TODO.md** — Current priorities
- **DONE.md** — Completed milestones
- **ISSUES.md** — Unresolved design questions
- **LESSONS-LEARNED.md** — What I've discovered from actual classroom delivery

### `/methodology/`
The core framework for curriculum development:
- **4-phase-workflow.md** — Content Audit → Presentation → Speaker Notes → Production
- **speaker-notes-format.md** — Structured format for teaching scripts
- **scaffolding-framework.md** — How content sequences across modules
- **ai-integration.md** — Where AI tools fit (and don't)

### `/automation/`
Scripts and workflows that make scale possible:
- **recording-pipeline/** — How 1 class recording becomes 5 deliverables
- **content-indexing/** — Semantic search across all published content
- **publishing-workflow/** — OneDrive → Git → LMS automation

### `/templates/`
Reusable scaffolding:
- Module structure templates
- Presentation format specs
- Speaker notes format

### `/examples/`
Sanitized samples from real courses (structure shown, proprietary content removed).

### `/projects/`
Brief descriptions of active programs and their status.

---

## The Core Methodology

### The Problem
Each course module requires:
- Topic research and outline
- Visual presentation (40-60 slides)
- Speaker notes (200-300 words per slide)
- Live recording and delivery
- Post-production (transcripts, chapters, announcements)
- LMS publishing

Multiply by 50+ modules across multiple courses. Manual approaches break down.

### The Solution: 4-Phase Workflow

```
Phase 1: Content Audit
├── Review source materials
├── Gap analysis vs. learning objectives
└── Topic outline approval

Phase 2: Presentation Development
├── Visual design (institutional branding)
├── Slide structure standards
└── AI-assisted content generation

Phase 3: Speaker Notes
├── Structured format (intro → points → transitions)
├── Timing estimates
└── Discussion questions

Phase 4: Production
├── Live recording (YouTube + OBS)
├── Auto-transcription (Whisper)
├── Chapter generation
├── Announcement creation
└── LMS publishing
```

### The Automation Layer

One recording produces:
1. **Timestamped transcript** (SRT) — auto-generated via Whisper
2. **Clean text** — filler words removed, readable format
3. **YouTube chapters** — auto-generated from content analysis
4. **Blackboard announcement** — recap for learners
5. **Promise extraction** — commitments made during class for follow-up

This happens automatically. The scripts are in `/automation/recording-pipeline/`.

---

## Proof Points

| Metric | Value |
|--------|-------|
| Active teaching programs | 5 |
| Course modules developed | 50+ |
| Class recordings | 69 |
| Python automation scripts | 54 |
| Grant funding secured | $30,000 |
| Concurrent cohorts managed | 2 |

---

## How to Navigate

**If you're an instructional designer:**
Start with `/methodology/4-phase-workflow.md` — the core framework.

**If you're technical:**
Start with `/automation/recording-pipeline/` — the scripts that make it work.

**If you're hiring:**
Start with `/project-management/CONVERSATION-CONTEXT.md` — why this exists and how I think.

**If you're curious about outcomes:**
Start with `/project-management/LESSONS-LEARNED.md` — what actually works in practice.

---

## Related Work

This methodology was influenced by:
- [Mike Behar's AI-in-Business-Course-Development](https://github.com/mikeBehar/AI-in-Business-Course-Development) — structured project management for course design
- [PPTX_Creation_utilities](https://github.com/mikeBehar/PPTX_Creation_utilities) — programmatic presentation generation

---

## Contact

- **LinkedIn:** [link]
- **Email:** [email]
- **Current role:** Instructional Designer / Course Facilitator at SCSU OWLL

---

*This methodology is actively evolving. Check CONVERSATION-CONTEXT.md for the latest development rationale.*
