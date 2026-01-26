# Conversation Context

> This document records the development history and rationale behind this methodology. It's the "why" behind the "what."

---

## Origin Story

### The Starting Point (Late 2024)

I started teaching Google Project Management Certificate courses at SCSU OWLL in late 2024. The role was straightforward: take Coursera content, adapt it for live delivery, and teach adult learners preparing for workforce certifications.

The first few modules were manual:
- Watch Coursera videos, take notes
- Build slides in PowerPoint
- Write speaker notes in a separate doc
- Record live sessions
- Manually create announcements
- Upload to Blackboard

This worked for one course. Then I got a second course (AI Fundamentals). Then the $30,000 grant for AI in Manufacturing. Then discussions about taking over NCC's AI Certificate program.

**The manual approach was going to break.**

### The Scale Problem

By early 2025, I was looking at:
- 30 modules for Google PM (6 courses × 5 modules average)
- 20 modules for AI Fundamentals (5 courses × 4 modules)
- Week-based curriculum for AI in Manufacturing
- 4 courses for NCC AI Certificate (potential)

That's 50+ unique modules, each requiring:
- Topic outline
- 40-60 slides
- 200-300 words of speaker notes per slide
- 1-2 hour recording
- Post-production assets

Multiply by multiple cohorts running simultaneously (I had 2 GPM cohorts at once), and the workload becomes impossible without systems.

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
- Creating Blackboard announcements
- Extracting key points

Multiply by 69 recordings.

**The solution:** Build a recording pipeline that automatically:
1. Transcribes via Whisper (local, GPU-accelerated)
2. Converts SRT to clean text (filler words removed)
3. Generates YouTube chapters from content
4. Creates Blackboard recap announcements
5. Extracts "promises" made during class

**The outcome:** Post-production dropped from 30-60 minutes to ~5 minutes of review.

### Decision 3: AI as Collaborator, Not Replacement

**The problem:** AI tools (ChatGPT, Claude) could generate content, but raw output was often generic or missed context.

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
- Ollama for local LLM inference (llama3.1:8b, nomic-embed-text)
- Qdrant for vector storage (semantic search across content)
- Docker MCP gateway for tool orchestration

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
| Nov 2024 | Started teaching GPM at SCSU OWLL |
| Dec 2024 | First recording pipeline script (manual trigger) |
| Jan 2025 | Added AI Fundamentals course |
| Jan 2025 | Standardized module scaffold template |
| Jan 2025 | Council review system for multi-AI document review |
| Feb 2025 | Whisper transcription automated |
| Feb 2025 | $30k AI in Manufacturing grant secured |
| 2025 | Chapter generation automated |
| 2025 | Blackboard recap generation automated |
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

**Mike Behar's work** at CT State Norwalk showed me that curriculum development could be structured like software development—with project management, version control, and documentation.

**Coursera's instructional design** demonstrated how to structure professional certificate programs with clear learning paths.

**Enterprise marketing automation** (my previous career) taught me that any repeatable process can be systematized.

---

## Current State

As of January 2026:
- **5 active programs** (GPM, AI Fundamentals, AI Manufacturing, NCC prep, Power BI)
- **50+ modules** in various stages of development
- **54 Python scripts** supporting automation
- **2 concurrent cohorts** running simultaneously
- **69 recordings** processed through the pipeline

The methodology works. This documentation makes it shareable.

---

*Last updated: January 2026*
