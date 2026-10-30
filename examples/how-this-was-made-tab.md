# Example: "How this was made" tab

This is an illustrative example. All content is fictional.

---

**Version:** v1.0, 2026-10-30

## Session summary

- **Rounds:** 3 drafts, 2 feedback rounds
- **Sources:** product strategy doc, two prior PRDs, customer research summary
- **Reviewers:** product director, eng lead, privacy counsel
- **Top lessons from feedback:**
  1. Lead with the decision requested.
  2. Make data sharing and consent explicit in a table.
  3. Link to specs instead of inlining them.

## Reproduction prompt

You are helping me produce a one-page PRD for product and engineering leaders.

**Goal:** The reader should approve or reject {{feature}} for {{quarter}} planning.

**Inputs:** Use only these sources. Mark gaps `[NEEDS INPUT: ...]` and inferences `[ASSUMPTION: ...]`.
- {{strategy doc}}
- {{prior PRDs}}
- {{research summary}}

**Structure:**
1. Decision requested: one or two sentences.
2. Problem: who is affected and the evidence.
3. Proposal: what changes for the user.
4. Data and consent: table of what data moves, from where, to where, and under which consent.
5. Risks and open questions.
6. Links to detailed specs.

**Quality bar:**
- The decision is stated in the first two sentences.
- Every claim traces to a listed source.
- It fits on one page.

**Rules learned from review:**
- State the decision requested in the first two sentences.
- Include a data-flow table for any cross-product data sharing.
- Link to detailed specs instead of inlining them.

**Process:** Ask up to five questions first. Draft, then list the three weakest parts. Write reviewer questions. Revise with a three-line change summary each round. Before finishing, list every claim I should verify.

I am accountable for the final result. Flag anything you are not confident about.

## How to adapt it

Swap `{{feature}}` and the sources for your own. For an executive audience, cut the structure to sections 1, 3, and 5. Keep the rules learned from review: they are where the quality comes from.

## Accountability note

This prompt shows how the work was made, not that it is right. Verify the output before you rely on it.
