---
name: internal-comms
description: A set of resources to help me write all kinds of internal communications, using the formats that my company likes to use. Use this skill whenever asked to write some sort of internal communications (status reports, leadership updates, 3P updates, company newsletters, FAQs, incident reports, project updates, etc.).
license: Complete terms in LICENSE.txt
---

# Codex Compatibility Notes

This skill was adapted from Anthropic's Claude Code skills so it can be used by Codex. Apply these interpretation rules while following the original instructions:

- Treat references to "Claude", "the next Claude", or "Reader Claude" as Codex or the current assistant unless the text is explicitly about Anthropic's Claude product or API.
- Treat "Claude Code" as Codex, and treat "Claude.ai" / "Claude app" as the current chat environment when that wording is only about where a workflow or artifact runs.
- Replace `AskUserQuestion` with a concise direct question to the user.
- Replace `WebFetch` / `WebSearch` with Codex web browsing tools.
- Replace `create_file` with creating a normal workspace file, and replace `str_replace` / `Edit` with precise file edits using Codex's editing workflow.
- Only use subagents or delegation when the current environment supports it and the user has explicitly allowed that mode of work.
- If the skill discusses Anthropic, Claude API, or Anthropic branding as part of the user task, keep that product-specific content intact; only adapt the runtime and tool assumptions.

## When to use this skill
To write internal communications, use this skill for:
- 3P updates (Progress, Plans, Problems)
- Company newsletters
- FAQ responses
- Status reports
- Leadership updates
- Project updates
- Incident reports

## How to use this skill

To write any internal communication:

1. **Identify the communication type** from the request
2. **Load the appropriate guideline file** from the `examples/` directory:
    - `examples/3p-updates.md` - For Progress/Plans/Problems team updates
    - `examples/company-newsletter.md` - For company-wide newsletters
    - `examples/faq-answers.md` - For answering frequently asked questions
    - `examples/general-comms.md` - For anything else that doesn't explicitly match one of the above
3. **Follow the specific instructions** in that file for formatting, tone, and content gathering

If the communication type doesn't match any existing guideline, ask for clarification or more context about the desired format.

## Keywords
3P updates, company newsletter, company comms, weekly update, faqs, common questions, updates, internal comms
