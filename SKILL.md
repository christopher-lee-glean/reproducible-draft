---
name: reproducible-draft
description: Run an AI-assisted drafting session that ends with a self-contained, end-to-end prompt anyone can paste into their own agent to reproduce the same quality. Use when drafting a document, PRD, strategy memo, plan, or analysis with AI and the author wants to iterate through human feedback rounds, show how the result was made, or help teammates get the same quality on their own work.
---

# Reproducible Draft

Draft fast with AI, improve it with human feedback, and finish with a reusable prompt that shows exactly how the result was made. No class required: the prompt is the lesson.

## Principles

- **Show how it was made.** The output of every session is two things: the work, and the prompt that reproduces it.
- **Feedback is where quality comes from.** The first prompt is rarely the valuable part. The rules learned from reviewer feedback are. Capture them.
- **The author stays accountable.** A reproduction prompt shows how something was made, not that it is right. Never let the prompt or the draft stand in for the author's judgment.
- **Portable by default.** The reproduction prompt must work in any capable agent, with no dependency on this conversation.

## Workflow

### 1. Frame the work

Confirm the essentials before drafting. Ask only for what is missing, at most five questions in one batch:

- **Outcome:** What decision, action, or change should this work drive?
- **Audience:** Who reads it, and what do they already know?
- **Inputs:** Which sources, data, or prior documents should it draw from?
- **Constraints:** Length, format, tone, deadline, anything off-limits.
- **Quality bar:** What would make the author proud to send it? Ask for one example of "great" if one exists.

### 2. Draft fast (Round 1)

- Produce a complete first draft quickly. Favor a full, imperfect draft over a polished fragment.
- Ground claims in the provided inputs. Do not invent facts, numbers, names, or quotes.
- Mark gaps inline: `[ASSUMPTION: ...]` for inferences and `[NEEDS INPUT: ...]` for missing information.
- End with a short list of the three weakest parts of the draft.

### 3. Collect feedback

- Write a short feedback request the author can send to reviewers: 3 to 5 targeted questions, grouped by reviewer role where relevant. Ask about the weakest parts first.
- When feedback arrives, record it in the feedback log (see `templates/feedback-log.md`): reviewer role, the comment, the decision (accept, reject, defer), and why.
- Turn each accepted comment into a **generalized rule** that would have prevented the issue. Example: "Too long" becomes "Lead with the decision in the first two sentences; cap the body at one page."

### 4. Revise (Round 2 and beyond)

- Apply the accepted feedback and the generalized rules.
- Start each new version with a three-line change summary.
- Repeat steps 3 and 4 until the author says the work is done.

### 5. Accountability check

Before finalizing, give the author a short checklist and ask them to confirm it:

- Claims, numbers, and names that need verification against a primary source.
- Remaining `[ASSUMPTION]` and `[NEEDS INPUT]` markers.
- Decisions or positions the author is personally signing up for.

Do not proceed to step 6 until the author confirms or explicitly accepts the open items.

### 6. Write the reproduction prompt

Fill in `templates/reproduction-prompt.md`. Rules:

- **Self-contained.** Someone who never saw this session should get comparable quality on the first run.
- **Generalized.** Replace specifics with `{{placeholders}}` so others can apply it to their own work. Keep the structure, quality bar, and rules.
- **Feedback encoded.** Include every generalized rule from the feedback log in the "Rules learned from review" section. This is what makes quality transfer.
- **Concrete quality bar.** State observable criteria ("decision in the first two sentences"), not adjectives ("clear and concise").
- **Safe to share.** Remove confidential names, numbers, internal data, and quotes unless the author explicitly says to keep them. Flag anything you are unsure about.
- **Compact.** Aim for under 800 words.

### 7. Package the "How this was made" tab

Produce one block of content the author can paste as a new tab in the same document:

1. **Version and date**, for example `v1.0, 2026-10-30`.
2. **Session summary:** number of rounds, types of sources used, reviewer roles, and the top three lessons from feedback.
3. **The reproduction prompt** from step 6.
4. **How to adapt it:** two or three sentences on which placeholders matter most and what to change for different audiences.
5. **Accountability note:** "This prompt shows how the work was made, not that it is right. Verify the output before you rely on it."

Then remind the author to add the tab to the document and share it.

### 8. Learn from reuse (optional)

Suggest that the author ask reusers to reply with what they changed. When improvements come back, fold them into the prompt as a new version and update the "Rules learned from review" section. Reuse is the success metric: a prompt nobody runs is a draft, not a skill.

## Output conventions

- Label every draft with its round: `Draft v1`, `Draft v2`, and so on.
- Keep the feedback log and the change summaries outside the draft itself.
- When the author says "wrap up" or "write the prompt", skip to step 5.
