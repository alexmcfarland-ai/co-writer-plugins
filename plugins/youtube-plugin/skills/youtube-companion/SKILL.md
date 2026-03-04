---
name: youtube-companion
description: Write Substack newsletters that accompany YouTube videos. Use when user has a YouTube video (transcript, outline, or link) and needs the companion newsletter with video embed, summary sections, and resources. Different from standalone newsletters - these drive to and summarize video content.
---
## Load Context First

Before executing this skill, read the following files from the project folder if they exist:

1. **USER.md** — who the user is, how they think, how they work, what they care about
2. **BUSINESS.md** — their business, products, positioning, brand voice, content strategy
3. **ICP.md** — their ideal customer, their language, their fears, what makes them buy
4. **Voice skill** — if the user has a voice skill installed globally in Claude Desktop, it will be auto-loaded. Do not attempt to read it as a file path.
5. Any additional context provided by the user in this session

Use all of this context silently to inform everything you produce. Do not reference or summarize the files unless asked.

---

# YouTube Companion Newsletter

Write a concise Substack newsletter that accompanies a YouTube video. The newsletter hooks readers, tells them what they'll learn, links to paid resources, and gets out of the way. It drives to the video — it does NOT replace it.

## Voice

Follow the voice-profile-alex skill if available. If not: direct, confident, no fluff. Write like the smart cousin who figured this out, not a guru or a marketer.

## Input

Accepts a transcript, outline, or notes from a YouTube video. Extract:

1. **Video topic** — what's being shown
2. **Key outcomes** — what viewers will learn/be able to do (5-6 max)
3. **Resources** — any downloads, plugins, starter kits mentioned
4. **One-liner hook** — why this matters right now

## Output Structure

The newsletter has exactly these sections in this order:

```markdown
# [Video Title]

### 💎 RESOURCE: [Short resource name]

_**Paid members:** All assets from my videos and guides—starter kits, prompts, skills, agents—are available for paid members._

---

---

[2-3 sentence setup. What shipped/changed, what you cover in the video, why it matters. Get to the point fast.]

[Optional: "In this video, I walk through everything — [thing], [thing], and [thing]."]

By the end, you'll have:

- **[Outcome 1]** — brief clarification
- **[Outcome 2]** — brief clarification
- **[Outcome 3]** — brief clarification
- **[Outcome 4]** — brief clarification
- **[Outcome 5]** — brief clarification

[One-liner kicker. Something like "If you've been using X, pay attention. This might change your setup."]

---

### **💎 GRAB YOUR RESOURCE: [Resource name]**

[1-2 sentences describing the resource.]

[CLICK HERE FOR THE RESOURCE](link placeholder)

What's inside:

- **[Item 1]** — what it does
- **[Item 2]** — what it does
- **[Item 3]** — what it does
- **[Item 4]** — what it does

[1 sentence on how to use it. "Download the zip and drag it into X to install."]

---

[2-3 sentence closer. Acknowledge it's early/new if relevant. Reinforce the direction. Tell them to start now.]

_—Alex_

**Stay connected**
[Twitter/X](https://x.com/mcfarland_ai) · [Instagram](https://instagram.com/alexxmcfarland)
```

## Rules

1. **Total length: 400-600 words.** This is not a long-form piece. It's a companion.
2. **No "Why [topic]?" section.** The setup paragraph handles this in 2-3 sentences.
3. **No "What's in the video" table.** The bullet list of outcomes covers it.
4. **No "Key concepts" section.** That's what the video is for.
5. **No "Start here" steps.** The resource section IS the action.
6. **No subject line options block.** Just write the title.
7. **Resource callout appears twice** — once at the very top (teaser) and once in the middle (full breakdown with link).
8. **Double horizontal rules** (`---\n\n---`) after the paid member callout. This is Alex's formatting pattern.
9. **Outcomes list uses bold + dash clarification.** Keep clarifications to one line.
10. **Closer is 2-3 sentences max.** Sign off with `_—Alex_`.
11. **Tone is direct and practical.** No hype, no "game-changer," no "unlock the power of."

## What NOT to Do

- Don't write a full tutorial — the video does that
- Don't add sections that aren't in the template above
- Don't pad with "why this matters" paragraphs — the setup covers it
- Don't use tables — use bullet lists
- Don't write more than 600 words
- Don't add meta-commentary like word counts or stats at the end

## Reference

Compare output against: `alex/substack/newsletters/2026-02-03-claude-cowork-plugins.md` — this is Alex's actual published newsletter and the gold standard for format and length.
