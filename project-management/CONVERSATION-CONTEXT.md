# Conversation Context

> This document records the development history and rationale behind this methodology. It's the "why" behind the "what."

---

## Origin Story

### The Starting Point (Late 2024)

I started teaching professional certificate courses at a state university workforce development office in late 2024. The role was straightforward: take existing course content, adapt it for live delivery, and teach adult learners preparing for workforce certifications.

The first few modules were manual:
- Review source videos, take notes
- Build slides in PowerPoint
- Write speaker notes in a separate doc
- Record live sessions
- Manually create announcements
- Upload to the LMS

This worked for one course. Then I got a second course. Then grant-funded technical training. Then discussions about additional certificate programs.

**The manual approach was going to break.**

### The Scale Problem

By early 2025, I was looking at:
- 30 modules for project management (6 courses × 5 modules average)
- 20 modules for AI fundamentals (5 courses × 4 modules)
- Week-based curriculum for industry-specific AI training
- Additional certificate programs in development

That's 50+ unique modules, each requiring:
- Topic outline
- 40-60 slides
- 200-300 words of speaker notes per slide
- 1-2 hour recording
- Post-production assets

Multiply by multiple cohorts running simultaneously, and the workload becomes impossible without systems.

---

## Key Decisions

### Decision 1: Structure Over Improvisation

**The problem:** Early modules had inconsistent quality. Some had detailed speaker notes, others had bullet points. Recording quality varied.

**The solution:** Create a repeatable structure:
- Standardized module scaffold (same folders, same files, same naming)
- Defined speaker notes format (intro → key points → transitions → discussion)
- HTML presentations instead of PowerPoint (version control, consistent rendering)

**The outcome:** Quality became consistent. New modules start from a known-good template.

### Decision 2: Automate Post-Production

**The problem:** After each recording, I was spending 30-60 minutes on:
- Cleaning up transcripts
- Writing chapter markers
- Creating LMS announcements
- Extracting key points

Multiply by 100+ recordings.

**The solution:** Build a recording pipeline that automatically:
1. Transcribes via Whisper (local, GPU-accelerated)
2. Converts SRT to clean text (filler words removed)
3. Generates YouTube chapters from content
4. Creates recap announcements
5. Extracts "promises" made during class

**The outcome:** Post-production dropped from 30-60 minutes to ~5 minutes of review.

### Decision 3: AI as Collaborator, Not Replacement

**The problem:** AI tools could generate content, but raw output was often generic or missed context.

**The solution:** Use AI for specific, constrained tasks:
- Outline expansion (human-approved outline → detailed content)
- Speaker note drafts (from approved slides)
- Recap generation (from approved transcripts)
- NOT for pedagogical decisions or learning objective design

**The outcome:** AI accelerates execution but doesn't make design choices.

### Decision 4: Local-First Infrastructure

**The problem:** Dependence on cloud APIs means:
- Cost scales with usage
- Privacy concerns with student content
- Outages affect teaching

**The solution:** Build local infrastructure:
- Ollama for local LLM inference
- Qdrant for vector storage (semantic search across content)
- Docker containers for tool orchestration

**The outcome:** Core operations work offline. Cloud is optional enhancement.

### Decision 5: Document the Methodology, Not Just the Content

**The problem:** If I got hit by a bus, no one could continue my work. The process was in my head.

**The solution:** This repository. Document:
- The workflow (what to do)
- The rationale (why to do it)
- The lessons learned (what actually works)
- The automation (how to do it faster)

**The outcome:** Handoff becomes possible. Others can adopt or adapt.

---

## Evolution Timeline

| Date | Milestone |
|------|-----------|
| Late 2024 | Started teaching professional certificates |
| Late 2024 | First recording pipeline script (manual trigger) |
| Early 2025 | Added second course |
| Early 2025 | Standardized module scaffold template |
| Early 2025 | Council review system for multi-AI document review |
| 2025 | Whisper transcription automated |
| 2025 | Grant-funded technical training added |
| 2025 | Chapter generation automated |
| 2025 | LMS recap generation automated |
| 2026 | This methodology documentation created |

---

## What's Still Evolving

### Active Development
- Promise extraction (tracking commitments made in class)
- Semantic search across all published content
- Inter-AI memory protocol (continuity across sessions)

### Under Consideration
- Student-facing documentation (not just instructor-facing)
- Video highlight extraction (key moments from recordings)
- Cohort analytics (completion patterns, engagement)

### Decided Against
- Fully automated slide generation (quality too inconsistent)
- AI-generated learning objectives (too important to delegate)
- Real-time AI assistance during live teaching (too distracting)

---

## Influences

This methodology didn't emerge in isolation:

**Structured course development** from colleagues demonstrated that curriculum development could be treated like software development—with project management, version control, and documentation.

**Professional certificate programs** showed how to structure learning paths with clear progressions.

**Enterprise marketing automation** (previous career) taught that any repeatable process can be systematized.

---

## Current State

As of early 2026:
- **5 active programs** across project management, AI, and data analytics
- **50+ modules** in various stages of development
- **50+ Python scripts** supporting automation
- **2 concurrent cohorts** running simultaneously
- **100+ recordings** processed through the pipeline

The methodology works. This documentation makes it shareable.

---

*Last updated: January 2026*
