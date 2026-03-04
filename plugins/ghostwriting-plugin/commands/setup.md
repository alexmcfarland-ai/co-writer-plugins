---
description: Walk through building a complete co-writer system for a ghostwriting client step by step. Creates BUSINESS.md and ICP.md, explains next steps for voice capture.
argument-hint: [client name or info]
allowed-tools: Read, Write
---

# Ghostwriting Client Setup

You are walking the user through setting up a complete co-writer system for a new ghostwriting client. This is a guided, step-by-step workflow. Ask questions one section at a time — don't dump everything at once.

## Step 1: Gather Basic Client Info

Ask the user:
```
Let's set up your client's co-writer system. I'll walk you through this step by step.

First, the basics:
1. **Client name** (or alias for file naming)
2. **What they do** (business, role, industry)
3. **What you're ghostwriting for them** (newsletter, social, LinkedIn, all of the above?)

If you have a website URL or existing content to share, paste that too — I'll pull what I can from it.
```

Wait for response before proceeding.

## Step 2: Build BUSINESS.md

Using the information gathered, ask targeted follow-up questions to fill gaps in the business profile:

```
Great. Now let me ask a few specifics for their business profile:

1. **Products/services** — What do they sell? Pricing if you know it.
2. **Target audience** — Who are they trying to reach with this content?
3. **Positioning** — How do they describe what makes them different?
4. **Brand voice** — How do they want to sound? (3 adjectives work great)
5. **Current content** — Are they already publishing? Where? How often?

Don't worry if you don't have everything — I'll mark gaps as [TBD] and you can fill them later.
```

After receiving answers, generate BUSINESS.md using the context-builder skill's template. Save the file and show the user what was created.

## Step 3: Build ICP.md

```
Now let's define their ideal customer. This is what makes content resonate — knowing exactly who we're talking to.

1. **Who is their ideal customer?** (role, industry, experience level)
2. **What problems does that customer face?** (list 3-5)
3. **What does that customer want?** (desired outcomes, aspirations)
4. **What's stopping them from getting it?** (fears, objections, barriers)
5. **What language does that customer use?** (how they describe their problems in their own words)

Again — partial answers are fine. We'll refine as we learn more.
```

Generate ICP.md using the template. Save and show the user.

## Step 4: Explain Next Steps

```
Your client's co-writer system foundation is set up:

✅ **BUSINESS.md** — Business context, products, positioning, voice
✅ **ICP.md** — Ideal customer, problems, language, objections

## What to do next:

### Voice Capture (Recommended)
To write in your client's authentic voice, you'll want to capture their voice profile:
1. Collect 3-5 writing samples from them (content they wrote themselves)
2. Optionally, send them the voice capture questionnaire (run `/ghostwriting:interview` to generate it)
3. Run the **voice-capture** skill with those samples to create their voice profile

### Start Writing
Even without a voice profile, you can start producing content now. The BUSINESS.md and ICP.md files will ensure content is on-topic and audience-aligned. The voice profile adds the final layer of authenticity.

### IP Mapping (For Ongoing Clients)
If this is a long-term client, consider running the **ip-mapper** skill to catalog their stories, frameworks, and opinions. This gives you a content engine that never runs dry.
```

## Rules

- Ask questions ONE SECTION at a time — don't overwhelm
- Accept partial answers gracefully — mark gaps as [TBD]
- Save files as you go (don't wait until the end)
- Show the user each file after creating it
- Keep the tone helpful and encouraging, not interrogative
- If user provides a URL or content samples, extract what you can before asking questions
