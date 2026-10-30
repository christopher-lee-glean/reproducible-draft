# reproducible-draft

A skill that packages one workflow: draft fast with AI, improve it with human feedback, and finish with a prompt anyone can paste into their own agent to reproduce the result.

A skill is just a folder of plain-text instructions in the open Agent Skills format. No product or account is required.

## How to use it

- **Agents that support Agent Skills** (for example, Claude Code): copy the `reproducible-draft` folder into the agent's skills directory, such as `~/.claude/skills/`. The agent picks it up when you start a drafting task.
- **Claude apps:** upload the zip as a custom skill in Settings, if skills are enabled for your account.
- **Any other AI chat:** paste the contents of `SKILL.md` at the start of a conversation, then describe what you want to draft.

## What's inside

- `SKILL.md`: the workflow the agent follows.
- `templates/reproduction-prompt.md`: the shape of the final, shareable prompt.
- `templates/feedback-log.md`: turns reviewer comments into reusable rules.
- `examples/how-this-was-made-tab.md`: a fictional example of the finished "How this was made" tab.

Edit any of it. If you improve it, version it and share it back.
