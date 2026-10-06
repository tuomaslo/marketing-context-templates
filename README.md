# Marketing Context Templates

**Stop re-explaining your brand to AI.**

Every marketer has done it: opened ChatGPT, typed "write a LinkedIn post about our new feature", got something generic back, spent 20 minutes editing it into something that actually sounds like you and then repeated the whole process tomorrow.

To fix this, we've built brand knowledge systems for 20+ brands. After hundreds of iterations we've ended up with a base context file structure that's shared here.

15 short Markdown templates for your brand, audience, products, and marketing channels. Fill the files you need, then give them to your AI when you work.

Built by [Tuomas Lounamaa](https://github.com/tuomaslo). I help tech companies with **agent discovery** — so their products get found and used by AI agents — and **GTM strategy**, including ICP targeting and finding practical ways to reach the right customers.

**[Read more about my work →](https://share.carryo.io/tuomas)**

## Start with five files

Download this repo using **Code → Download ZIP**, or clone it. Start by filling these files for your own brand:

1. [Brand core](identity/brand-core.md) — what you do and why it matters.
2. [Voice guide](identity/voice-guide.md) — how you sound, with examples.
3. [Audience profile](identity/audience-profile.md) — who you serve and what they need.
4. [Guardrails](guardrails/guardrails.md) — what to avoid and what to check.
5. One [channel template](channel/) — wherever you are writing next.

See the [completed Linear example](examples/linear/README.md) before filling your own. Add the other templates when a task needs them.

## Fill the files with AI

Give your AI the selected templates, your website, product documentation, and a few approved examples. In a file-based agent, open the downloaded folder and ask it to read this README. In a chat, attach or paste the files.

```text
Fill the selected marketing context templates for [BRAND].
Use these sources: [WEBSITE, PRODUCT DOCS, APPROVED EXAMPLES].

Keep each file brief and specific. Use these labels where needed:
- Confirmed: supported by a source or approved by the brand owner.
- Proposed: suggested wording, interpretation, or a decision to review.
- Unknown: important information the sources do not establish.

Link important factual claims to their sources. Give changing facts,
such as pricing, a checked date. Keep product facts and customer proof
in proof/product-and-proof.md; reference them elsewhere.
Mark examples Published or Draft. Only describe performance if measured.
Do not invent customer quotes, metrics, capabilities, or strategy.

Return the filled files and a short list of decisions or missing facts
for me to review. Use the Linear example as a format reference only.
```

Review the result. Replace placeholders with useful content or **Unknown**, and remove sections that do not help. Save the filled files in your own working copy. Keep examples you want the AI to learn from.

## Which files should the AI read?

For writing, read the three identity files, guardrails, and the chosen channel. Then add only what the task needs:

| Task | Extra context |
|---|---|
| Product, pricing, or customer claims | [Product and proof](proof/product-and-proof.md) |
| Comparison or sales copy | [Positioning](proof/positioning.md), relevant [competitor research](intelligence/competitive-landscape.md) |
| Campaign planning | [Strategy](strategy/strategy.md), relevant [trends](intelligence/industry-trends.md) |
| Visual brief | [Visual brand](visual/visual-brand.md) |

In a chat or project, supply these files using the tool's supported attachments or knowledge setup. A folder of Markdown files does not load itself into every prompt.

**Resolve conflicts:** follow the latest owner-approved direction and current product facts. Older published copy and draft examples must not override them. Flag unresolved contradictions. Leave out unknown claims, or ask when they are essential to the task.

## The full library

| Category | Templates |
|---|---|
| Identity | [Brand core](identity/brand-core.md), [Voice](identity/voice-guide.md), [Audience](identity/audience-profile.md) |
| Proof | [Product and proof](proof/product-and-proof.md), [Positioning](proof/positioning.md) |
| Channel | [LinkedIn](channel/linkedin.md), [X](channel/twitter.md), [Instagram](channel/instagram.md), [Email](channel/email.md), [Website](channel/website.md) |
| Guardrails | [Guardrails](guardrails/guardrails.md) |
| Visual | [Visual brand](visual/visual-brand.md) |
| Strategy | [Strategy](strategy/strategy.md) |
| Intelligence | [Competitors](intelligence/competitive-landscape.md), [Trends](intelligence/industry-trends.md) |

Keep these files focused. Update a rule when you repeatedly correct the AI. Refresh product facts when the product changes. Use source links inside the relevant files; no separate source register is required.

## Updating an older copy

If you already filled the previous templates, move your content into the merged files before removing your old copies:

| Previous files | New home |
|---|---|
| `proof/achievements.md` + `proof/product-updates.md` | `proof/product-and-proof.md` |
| `guardrails/dont-list.md` + `guardrails/quality-checklist.md` | `guardrails/guardrails.md` |
| `channel/website.md` + `channel/website-reference.md` | `channel/website.md` |
| `visual/visual-brand.md` + `visual/visual-examples.md` | `visual/visual-brand.md` |

## Contributing and license

Ideas, issues, and pull requests are welcome. [MIT licensed](LICENSE): copy, adapt, and use the templates.
