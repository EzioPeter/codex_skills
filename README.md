# Codex Skills Mirror

This directory contains Codex-adapted copies of the skills from [`claude_code_skills`](../claude_code_skills).

## What Was Preserved

- Original skill names, folder layout, scripts, templates, references, examples, and license files
- Skill-specific documentation for domains like PDF, DOCX, PPTX, XLSX, MCP, frontend, and Claude API work

## What Was Adapted

- Each `SKILL.md` now starts with a **Codex Compatibility Notes** section
- Claude-specific tool names such as `AskUserQuestion`, `WebFetch`, `create_file`, and `str_replace` were mapped to Codex-friendly equivalents
- A few high-risk files received targeted wording fixes where the original instructions were too tied to Claude-only runtime assumptions

## Skill Count

- Total mirrored skills: 17

## Mirrored Skills

- `algorithmic-art`
- `brand-guidelines`
- `canvas-design`
- `claude-api`
- `doc-coauthoring`
- `docx`
- `frontend-design`
- `internal-comms`
- `mcp-builder`
- `pdf`
- `pptx`
- `skill-creator`
- `slack-gif-creator`
- `theme-factory`
- `web-artifacts-builder`
- `webapp-testing`
- `xlsx`

## Notes

These skills are stored in `codex_skills/` as requested. They are ready to be copied, symlinked, or installed into a Codex skill search path if you want them to auto-trigger in other sessions.
