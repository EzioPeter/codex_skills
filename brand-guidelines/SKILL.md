---
name: brand-guidelines
description: Applies Anthropic's official brand colors and typography to any sort of artifact that may benefit from having Anthropic's look-and-feel. Use it when brand colors or style guidelines, visual formatting, or company design standards apply.
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

# Anthropic Brand Styling

## Overview

To access Anthropic's official brand identity and style resources, use this skill.

**Keywords**: branding, corporate identity, visual identity, post-processing, styling, brand colors, typography, Anthropic brand, visual formatting, visual design

## Brand Guidelines

### Colors

**Main Colors:**

- Dark: `#141413` - Primary text and dark backgrounds
- Light: `#faf9f5` - Light backgrounds and text on dark
- Mid Gray: `#b0aea5` - Secondary elements
- Light Gray: `#e8e6dc` - Subtle backgrounds

**Accent Colors:**

- Orange: `#d97757` - Primary accent
- Blue: `#6a9bcc` - Secondary accent
- Green: `#788c5d` - Tertiary accent

### Typography

- **Headings**: Poppins (with Arial fallback)
- **Body Text**: Lora (with Georgia fallback)
- **Note**: Fonts should be pre-installed in your environment for best results

## Features

### Smart Font Application

- Applies Poppins font to headings (24pt and larger)
- Applies Lora font to body text
- Automatically falls back to Arial/Georgia if custom fonts unavailable
- Preserves readability across all systems

### Text Styling

- Headings (24pt+): Poppins font
- Body text: Lora font
- Smart color selection based on background
- Preserves text hierarchy and formatting

### Shape and Accent Colors

- Non-text shapes use accent colors
- Cycles through orange, blue, and green accents
- Maintains visual interest while staying on-brand

## Technical Details

### Font Management

- Uses system-installed Poppins and Lora fonts when available
- Provides automatic fallback to Arial (headings) and Georgia (body)
- No font installation required - works with existing system fonts
- For best results, pre-install Poppins and Lora fonts in your environment

### Color Application

- Uses RGB color values for precise brand matching
- Applied via python-pptx's RGBColor class
- Maintains color fidelity across different systems
