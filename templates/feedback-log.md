# Feedback log template

Record every piece of feedback, the decision, and the rule it produced. The "Generalized rule" column feeds the "Rules learned from review" section of the reproduction prompt.

| Round | Reviewer role | Feedback | Decision | Why | Generalized rule |
|---|---|---|---|---|---|
| 1 | {{e.g. Eng lead}} | {{what they said}} | Accept / Reject / Defer | {{reason}} | {{rule that would have prevented this}} |
| 1 | | | | | |
| 2 | | | | | |

## Example

| Round | Reviewer role | Feedback | Decision | Why | Generalized rule |
|---|---|---|---|---|---|
| 1 | Product director | "I read the whole page before I found the ask." | Accept | The reader decides on the ask | State the decision requested in the first two sentences. |
| 1 | Privacy counsel | "Unclear what data is shared between products." | Accept | Required for review | Include a data-flow table: what data, from where, to where, under which consent. |
| 1 | Eng lead | "Add the full API spec." | Defer | Belongs in the design doc, not the one-pager | Link to detailed specs instead of inlining them. |
