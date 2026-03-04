---
description: Write a Substack companion newsletter for a YouTube video, including embed, summary sections, and resources.
argument-hint: [video transcript or topic]
allowed-tools: Read
---

First, read the following context files from the project folder if they exist:
- USER.md
- BUSINESS.md
- ICP.md

Then read and follow the instructions in @${CLAUDE_PLUGIN_ROOT}/skills/youtube-companion/SKILL.md.

Write a companion newsletter for: $ARGUMENTS

If no transcript or topic is provided, ask the user before starting.
