# Marketing Context Templates

**Stop re-explaining your brand to AI every single time.**

Every marketer has done it: opened ChatGPT, typed "write a LinkedIn post about our new feature", got something generic back, spent 20 minutes editing it into something that actually sounds like you and then repeated the whole process tomorrow.

To fix this, we've built brand knowledge systems for 20+ brands. After hundreds of iterations we've ended up with a base context file structure that's shared here. 

Take these templates, fill with your brand and get AI to work for you at a completely new level.

## What Is This

A set of **19 structured markdown templates** organized into 7 categories. Designed to capture everything an AI needs to pland and create in your voice, for your audience, in your channels:

| Category | Files | What it captures |
|----------|-------|-----------------|
| `identity/` | brand-core, voice-guide, audience-profile | Who you are, how you sound, who you're talking to |
| `proof/` | achievements, positioning, product-updates | What you've done, how you compete, what you've shipped |
| `channel/` | linkedin, twitter, instagram, email, website, website-reference | Per-channel specs, best performers, and formats |
| `guardrails/` | dont-list, quality-checklist | What to never say, and what good looks like |
| `visual/` | visual-brand, visual-examples | Brand look and feel, image assets |
| `strategy/` | strategy | How you market — channels, cadence, campaigns |
| `intelligence/` | competitive-landscape, industry-trends | What's happening in your market |

Each file has clear instructions, concrete examples, and `[PLACEHOLDER]`-style prompts. Fill them in once, update them as you grow, and use them everywhere.

## Why This Works

AI tools hallucinate generic content because they're given generic prompts. When you give them structured, specific context about your brand, the output quality jumps dramatically.

Teams using a properly filled context library report:

- **Fewer revision rounds** — output that sounds like you from draft one
- **Consistent brand voice** across every channel and every team member
- **Less hallucination** — specific brand facts replace made-up claims
- **Faster production** — skip the "re-explain the brand" step every time
- **Better onboarding** — new team members or agencies get up to speed faster

**The big shift is moving away from editing the output and working on the system that generates the output. Context engineering is what enables scale and consistent quality.**

The context library doesn't just make AI better. It forces you to articulate things about your brand that often live only in someone's head. That clarity pays dividends beyond AI usage.

## How to Use These Templates

### Option 1 — Fork, fill, and load into an AI project (Claude, ChatGPT, Gemini)

1. Fork this repo and fill in the templates with your brand details
2. Download the filled files (or just the identity + guardrails files to start)
3. In Claude, ChatGPT, or Gemini, create a new **Project**
4. Upload the downloaded files as context/knowledge files to the project
5. Every conversation in that project now has your full brand context automatically loaded — no pasting required

### Option 2 — Use with Claude Code or Cursor

After forking the repo, clone it to your computer and open the folder in Claude Code or Cursor. The AI reads all your context files directly — no copy-pasting needed.

- **Clone your fork:** go to your forked repo on GitHub, click the green **Code** button, copy the URL, then run `git clone [that URL]` in your terminal
- **Open in Claude Code:** navigate into the folder in your terminal and type `claude` to start
- **Open in Cursor:** open Cursor and use File → Open Folder to open the cloned folder
- Ask the AI to help fill in templates, create content, or update your context files — it has access to all files at once
- Save changes to keep your context library current over time

### Option 3 — Use as a system prompt

In Claude, ChatGPT, or any tool that supports custom instructions or system prompts:

1. Combine your key files (brand-core + voice-guide + audience-profile + dont-list) into one block
2. Set it as your default system prompt or custom instructions
3. Every conversation starts with your brand context already loaded

**Claude custom instructions example:**
```
You are a marketing assistant for [YOUR BRAND]. Always refer to the following brand context when planning marketing or writing any content:

[paste your combined context files here]

Always follow the voice guide and never use the banned phrases in the don't list.
```

### Option 4 — Paste into any AI chat (Claude, ChatGPT, Gemini)

> This system is designed to get you away from copy-pasting context every time — but pasting is a perfectly good way to get started and feel the difference before setting up a project or integration.

1. Fork this repo and fill in the templates with your brand details
2. When starting a content task, paste the relevant files as context:

```
Here is my brand context:

[paste brand-core.md]
[paste voice-guide.md]
[paste audience-profile.md]
[paste linkedin.md — if writing LinkedIn content]
[paste dont-list.md]

Now write a LinkedIn post announcing our new [feature]. The post should...
```

Which files to include depends on the task:
- **Writing content:** identity files + relevant channel file + guardrails
- **Planning a campaign:** identity + strategy + intelligence
- **Writing about a product update:** identity + proof/product-updates + channel files
- **Competitive content:** identity + proof/positioning + intelligence

## Getting Started

### 1. Fork or Download this repo

Click **Fork** at the top right. This becomes your private brand context library. Alternatively, click the Code dropdown and download this as a Zip file.

### 2. Fill the templates — the easy way

The fastest way to fill these templates is to let an AI do the first pass for you:

1. Open a new conversation in Claude or ChatGPT
2. Paste the template file(s) you want to fill
3. Give it everything it needs to work from:
   - Files you have (old brand docs, a deck, past content)
   - Memory the AI already has about you (if you've used a Claude Project or ChatGPT memory extensively, it may already know things aboyt your brand)
   - Your website URL as additional reference
4. Give it this instruction: **"Fill in these templates using only what you can find in the materials I've given you. Do not invent or assume anything. If you don't have enough information to fill a field, leave it blank or flag it. No hallucinations — I will review everything before use."**
5. Review every field manually before committing. The AI will get most things right but will occasionally fill in something plausible-sounding that isn't quite true. That's your job to catch.

This gets you a solid 80% fill in minutes rather than hours. The remaining 20% — the specific examples, exact numbers, and nuanced takes — you fill in yourself.

### 3. Start with Identity (highest ROI)

Fill in these three files first — they're included in every prompt and have the most impact:

1. **`identity/brand-core.md`** — 15 minutes. Your mission, what you do, who you serve.
2. **`identity/voice-guide.md`** — 30 minutes. How you sound. Include real examples.
3. **`identity/audience-profile.md`** — 20 minutes. Who you're talking to and what they care about.

With just these three files filled in, your AI output will be noticeably better.

### 4. Add Guardrails

4. **`guardrails/dont-list.md`** — 20 minutes. Every phrase that makes you wince, written down.
5. **`guardrails/quality-checklist.md`** — 10 minutes. Customize the checklist for your brand.

### 5. Fill in your active channels

Add your actual top-performing posts and channel specs to the channel files you use. The examples section of each playbook is where the real quality improvement comes from — the AI learns your pattern from real examples.

### 6. Fill in Proof and Strategy when you need deeper outputs

The proof and strategy files make a big difference for planning content and writing anything competitive or credibility-focused.

## File Naming & Structure

```
marketing-context-templates/
├── identity/
│   ├── brand-core.md          # Mission, vision, values, what you do
│   ├── voice-guide.md         # How you sound, forbidden phrases, tone by context
│   └── audience-profile.md    # Who you're talking to, their goals and pain points
│
├── proof/
│   ├── achievements.md        # Stats, case studies, testimonials, milestones
│   ├── positioning.md         # Competitive positioning, unique advantages
│   └── product-updates.md     # Changelog for content use (connect to Linear)
│
├── channel/
│   ├── linkedin.md            # Specs, top performers, hooks, formats
│   ├── twitter.md             # Specs, tweet formats, top performers
│   ├── email.md               # Program overview, subject patterns, top emails
│   ├── website.md             # Blog + landing page playbook, top content
│   └── website-reference.md   # Your actual website copy (paste or scrape)
│
├── guardrails/
│   ├── dont-list.md           # Banned phrases, tone mistakes, claim rules
│   └── quality-checklist.md   # Pre-publish checklist, AI output quality signals
│
├── visual/
│   ├── visual-brand.md        # Colors, fonts, visual mood, image style
│   └── visual-examples.md     # Actual image URLs and when to use them
│
├── strategy/
│   └── strategy.md            # Active channels, cadence, sequences, tool stack
│
└── intelligence/
    ├── competitive-landscape.md   # Competitor tracking, positioning gaps
    └── industry-trends.md         # Market forces, emerging topics, audience shifts
```

## Tips for Getting the Most Out of This

**Be specific, not aspirational.** The voice guide works because of the specific "never say X, say Y instead" entries — not the abstract "we sound professional" descriptions. Specificity is what separates useful context from generic filler.

**Use real examples.** Wherever you feel the template and example structures don't quite work for you, just copypaste example for that category of knowledge. Especially when you go closer to the channel playbook files, these have a "top performing posts" section. Filling those in with your actual best content is the single highest-ROI thing you can do. AI loves to use patterns from real examples.

**Update it when the AI gets it wrong.** Every time you edit AI output and think "it should never do that again" — add it to `dont-list.md`. The file compounds over time.

**No need to fill it all in at once.** Start with Identity and Guardrails. Add channels as you use them. 

Fill out Strategy and Intelligence files when you want to do strategic planning with AI. These are also highest maintenance and we recomend setting scheduled, regular updates.

**Keep the files focused.** Longer isn't better. A focused 300-word voice guide beats a sprawling 2,000-word one that dilutes the signal with filler. This also makes it harder for you and your colleagues to update. Filling these files with a lot of AI slop is what you want to stricly avoid.

## Contributing

Found a template structure that works better? Have a file type that should be in here? Ideas, PRs and issues welcome.

## License

Fork it, adapt it, use it however you want.

*Built by [tuomaslo](https://github.com/tuomaslo) 
