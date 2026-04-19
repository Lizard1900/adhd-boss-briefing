# adhd-boss-briefing

A Claude skill for legal and compliance professionals who need to brief a non-lawyer executive with ADHD — or anyone who prefers bottom-line-up-front, jargon-free communication.

## The problem this solves

Legal teams produce rigorous analysis. Executives need clear decisions. The gap between them is not a knowledge problem — it is a communication format problem.

When your boss:
- Has ADHD or an ADHD-compatible attention style
- Comes from a business or finance background (not legal)
- Reads on mobile, between meetings, at speed
- Will not re-read your previous briefing before opening this one
- Needs to know **what to decide**, not just **what the law says**

...standard legal memo format will fail. This skill fixes that.

## What it does

This skill produces two output formats for any legal or compliance update:

| Format | Length | Use case |
|--------|--------|----------|
| **IM Cover Message** | 8–15 lines | Send via Slack, Teams, WeChat, Lark — the message the exec reads *before* opening the attachment |
| **Full Briefing Document** | 1–3 pages | The attached document with complete analysis |

Both formats follow the same core principle: **conclusion first, plain language throughout, always end with a specific action or decision**.

## Who it's for

- In-house legal and compliance professionals
- Regulatory affairs teams
- Anyone who briefs a non-lawyer decision-maker on complex legal matters
- Works for any legal domain: competition law, employment, data privacy, financial regulation, etc.

## Installation

### Option 1: Install the `.skill` file directly

1. Download [`adhd-boss-briefing.skill`](./adhd-boss-briefing.skill)
2. Go to [claude.ai](https://claude.ai) → Settings → Skills
3. Upload the `.skill` file
4. The skill will now be available in your conversations

### Option 2: Copy the SKILL.md manually

1. Copy the contents of [`skill/SKILL.md`](./skill/SKILL.md)
2. Create a new skill in Claude and paste the content

## Usage

Once installed, Claude will automatically apply this skill when you ask for executive briefings. You can also trigger it explicitly:

```
"Write up this compliance update for my boss — IM message format"
"Draft the briefing doc on our GDPR investigation for management"
"Help me explain this antitrust risk to a non-lawyer exec"
"Write a Slack message summarizing where we are on the [X] matter"
```

## Example output

**IM Cover Message:**
```
[Matter] Compliance Update:

1. Pricing mechanism risk
Conclusion: We can maintain current practice — risk is lower than initially assessed.
• 60% of sellers reject our recommended price, showing they have real bargaining power
• Competitors run similar systems without enforcement action in the past 3 years
• No immediate regulatory action expected; we will monitor

2. Transparency obligations
Conclusion: We need to make a targeted fix to our seller communications.
• Regulator has flagged this point specifically (confirmed last week)
• Proposed fix: add plain-language explanation of how prices are set to seller dashboard
• Timeline: draft ready by Friday; need your go-ahead before we send to product team

Full analysis attached. Recommend reading Section 2 before Thursday's call.
```

## Customization

The skill works out of the box, but you can improve results by telling Claude:

- **Your boss's specific background**: "My boss has a banking background" or "My boss is an engineer"
- **The communication platform**: "This is for a Slack message" or "This is for a Teams post"
- **The language**: The skill defaults to the language of your input — write in Chinese and it will output in Chinese
- **Which format you need**: "Just the IM message" or "Just the briefing doc" or "Both"

## What makes a good executive briefing

The skill is built around five principles derived from working with ADHD executives:

1. **Conclusion first** — Every section opens with its bottom line. The executive reads the first sentence of each section; make it count.
2. **Plain language** — Legal terms get plain-English translations. If a sentence requires a law degree to parse, it gets rewritten.
3. **Numbers over adjectives** — "60% of sellers" beats "a significant proportion of sellers" every time.
4. **Explicit call-backs** — Never assume the executive remembers the previous briefing. Every reference to prior context includes a one-line recap.
5. **Always end with an action** — Every briefing ends with numbered next steps, at least one of which requires the executive's input or decision.

## Contributing

Improvements welcome. If you work with a different type of non-lawyer decision-maker (e.g., a technical founder, a finance CFO, a board member) and have learned what works, open a PR with your additions.

## License

MIT — use freely, attribution appreciated but not required.
