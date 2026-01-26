# 4-Phase Curriculum Development Workflow

> The systematic process for transforming source content into deliverable course modules.

---

## Overview

Every module goes through four phases:

```
Phase 1: Content Audit     → What needs to be taught?
Phase 2: Presentation Dev  → How will it be shown?
Phase 3: Speaker Notes     → How will it be taught?
Phase 4: Production        → How will it be delivered and captured?
```

Each phase has defined inputs, outputs, and quality gates. A module doesn't advance until the current phase is complete.

---

## Phase 1: Content Audit

### Purpose
Understand the source material and identify gaps against learning objectives.

### Inputs
- Source content (Coursera modules, existing presentations, reference materials)
- Learning objectives (what learners should be able to do)
- Time constraints (module duration, session format)

### Process

1. **Source Review**
   - Watch/read all source materials
   - Take structured notes: key concepts, examples, activities
   - Flag confusing or incomplete sections

2. **Learning Objective Alignment**
   - Map source content to learning objectives
   - Identify gaps (objectives without content)
   - Identify surplus (content without objectives)

3. **Topic Outline Creation**
   - List major topics (3-5 per module)
   - Subtopics under each major topic
   - Estimated time per section
   - Proposed activities or checkpoints

4. **Gap Analysis**
   - What's missing from source that learners need?
   - What examples need to be updated or localized?
   - What activities need to be created?

### Outputs
- Topic outline document (approved)
- Gap analysis notes
- Time budget

### Quality Gate
Topic outline reviewed and approved before Phase 2 begins. Changes to outline after Phase 2 require rework.

---

## Phase 2: Presentation Development

### Purpose
Create the visual materials for instruction.

### Inputs
- Approved topic outline from Phase 1
- Institutional branding guidelines (colors, logos, fonts)
- Slide structure standards

### Process

1. **Slide Structure Planning**
   - Title slide
   - Agenda/roadmap slide
   - Content slides (1 concept per slide)
   - Activity/discussion slides
   - Summary/review slide

2. **Content Development**
   - One key point per slide
   - Supporting visuals (diagrams, screenshots, examples)
   - Consistent formatting (headings, bullets, spacing)

3. **Visual Design**
   - Institutional colors (SCSU: Navy #003366, Gold #FFD700)
   - Readable fonts (min 24pt for content)
   - Clean layouts (no clutter)

4. **AI-Assisted Drafting** (optional)
   - Provide outline + context to AI
   - Generate slide content drafts
   - Human review and revision required

### Outputs
- Complete slide deck (HTML or PPTX)
- 40-60 slides typical
- All visuals embedded or linked

### Quality Gate
Slides reviewed for:
- Alignment with topic outline
- Visual consistency
- Readability
- Accessibility (alt text, color contrast)

---

## Phase 3: Speaker Notes

### Purpose
Create the teaching script that accompanies each slide.

### Inputs
- Completed slides from Phase 2
- Topic outline from Phase 1
- Target session duration

### Process

1. **Note Structure** (per slide)
   ```
   INTRO (1-2 sentences)
   - What this slide covers
   - Why it matters

   KEY POINTS (3-5 bullets)
   - Main teaching content
   - Examples to mention
   - Common misconceptions to address

   TRANSITION (1 sentence)
   - Connection to next slide

   TIMING: X minutes
   ```

2. **Content Depth**
   - 200-300 words per slide
   - Enough detail to teach from, not read from
   - Include questions to ask learners

3. **Discussion Questions**
   - At least 1 per major section
   - Open-ended, not yes/no
   - Relevant to learner context (workforce, certification)

4. **Timing Estimates**
   - Per-slide timing
   - Section subtotals
   - Total session duration
   - Buffer for questions (10-15%)

### Outputs
- Complete speaker notes document
- Aligned 1:1 with slides
- Total timing calculated

### Quality Gate
Notes reviewed for:
- Completeness (every slide has notes)
- Teachability (could someone else use these?)
- Timing (fits session duration)

---

## Phase 4: Production

### Purpose
Deliver the content and create all derivative assets.

### Inputs
- Slides from Phase 2
- Speaker notes from Phase 3
- Recording setup (OBS, YouTube, camera, mic)

### Process

1. **Pre-Recording**
   - Test all equipment
   - Open slides, notes, and any demos
   - Start recording software
   - Verify YouTube stream (if live)

2. **Live Delivery**
   - Follow speaker notes structure
   - Engage with chat/questions
   - Verbally announce module/session info (for auto-classification)

3. **Post-Recording** (automated via recording pipeline)
   - Whisper transcription → SRT file
   - Clean text conversion → readable transcript
   - Chapter generation → YouTube chapters
   - Recap generation → Blackboard announcement
   - Promise extraction → follow-up items

4. **Publishing**
   - Video to YouTube (if live, already there)
   - Transcript to content archive
   - Announcement to Blackboard
   - Module marked complete in tracking

### Outputs
- Video recording (MKV or MP4)
- Timestamped transcript (SRT)
- Clean text transcript
- YouTube chapters
- Blackboard announcement
- Any extracted follow-up items

### Quality Gate
Module marked PUBLISHED only when:
- Video is accessible
- Transcript is accurate (spot-checked)
- Announcement posted to LMS
- Tracking updated

---

## Phase Transitions

```
┌─────────────────┐
│   Phase 1       │
│ Content Audit   │
│                 │
│ Output: Outline │
└────────┬────────┘
         │ Outline approved?
         ▼
┌─────────────────┐
│   Phase 2       │
│ Presentation    │
│                 │
│ Output: Slides  │
└────────┬────────┘
         │ Slides reviewed?
         ▼
┌─────────────────┐
│   Phase 3       │
│ Speaker Notes   │
│                 │
│ Output: Notes   │
└────────┬────────┘
         │ Notes complete?
         ▼
┌─────────────────┐
│   Phase 4       │
│ Production      │
│                 │
│ Output: Assets  │
└─────────────────┘
```

**Key rule:** Don't skip phases. Rushing to recording without solid notes creates inconsistent delivery. Rushing to slides without outline approval creates rework.

---

## Tooling

### Phase 1
- Obsidian (note-taking, outline creation)
- Source materials (Coursera, PDFs, videos)

### Phase 2
- HTML editor (VS Code) or PowerPoint
- Figma/Canva for custom graphics
- AI assistance (outline → draft content)

### Phase 3
- Obsidian or Word (notes authoring)
- Slide deck for reference
- AI assistance (slides → draft notes)

### Phase 4
- OBS Studio (recording)
- YouTube Live (streaming)
- Recording pipeline scripts (post-production)
- Blackboard (LMS publishing)

---

## Common Failure Modes

| Failure | Symptom | Fix |
|---------|---------|-----|
| Skipping Phase 1 | Slides don't cover objectives | Enforce outline approval |
| Rushing Phase 2 | Visual inconsistency | Use templates |
| Thin Phase 3 | Unprepared delivery, dead air | Min word counts |
| Manual Phase 4 | Post-production backlog | Automate pipeline |

---

## Adapting the Workflow

This workflow is designed for professional certificate courses delivered live. Adjustments for other contexts:

**Asynchronous delivery:** Phase 4 changes—no live stream, pre-recorded with editing.

**Shorter modules:** Phases 2-3 can compress if content is simple.

**Team development:** Add review gates between phases with assigned reviewers.

**Existing content adaptation:** Phase 1 becomes more about audit than creation.

---

*This workflow is the foundation. See `/automation/` for tools that accelerate each phase.*
