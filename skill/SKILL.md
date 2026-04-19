---
name: adhd-boss-briefing
description: >
  Use this skill when drafting any legal or compliance update for a non-lawyer executive
  who has ADHD or ADHD-like working style — including managers with short attention spans,
  strong preference for bottom-line-up-front communication, and low tolerance for legal
  jargon. Triggers include: "write up this legal update for my boss", "draft the briefing
  doc on [X] for management", "help me write the IM/chat message summarizing [X]",
  "how do I explain this compliance issue to a non-lawyer", "draft the executive summary
  for [legal matter]", or any situation where complex legal or regulatory analysis needs
  to be communicated to a senior decision-maker who is not a lawyer. Produces two output
  formats: a short IM/chat cover message (8–15 lines) and a full briefing document (1–3
  pages). Always use this skill when the reader is a non-lawyer executive — do not default
  to legal memo format.
---

# ADHD Boss Briefing Skill

This skill produces legal and compliance updates for non-lawyer executives who have ADHD
or an ADHD-compatible working style. It governs two output formats: a short **IM cover
message** (sent via WeChat, Slack, Teams, Lark, or any chat tool) and a **full briefing
document** (attached file, 1–3 pages).

The fundamental insight behind this skill: **the biggest failure mode in legal-to-executive
communication is not getting the law wrong — it is writing for a lawyer when the reader
is not one.**

---

## Step 1: Know Your Reader

Before drafting, internalize this reader profile. Every drafting decision flows from it.

| Trait | What It Means for Your Draft |
|---|---|
| **Not a lawyer** | Legal terms need plain-English translation in parentheses, or should be replaced entirely. If a sentence requires a law degree to parse, rewrite it. |
| **ADHD** | Conclusion comes first, always. Long preamble = lost reader. Bullet points over prose. Clear headings. No walls of text. |
| **Finance / business background** | Respects logical structure and numbers. Responds to commercial framing ("this affects revenue / timeline / liability") over legal framing ("this engages Article X"). Will notice a gap in logic. |
| **Poor working memory** | Every document must be self-contained. Explicitly recall prior context — never assume they remember a previous briefing. |
| **Wants to know what to do** | Ambiguous conclusions are unacceptable. Every briefing must end with a clear recommended action or decision. "It depends" without a recommendation is a failure. |

---

## Step 2: Choose the Output Format

Ask the user (or infer from context) which format is needed:

| Format | When to Use | Length |
|---|---|---|
| **Format A — IM Cover Message** | Sending a document via chat; need the executive to read it before a meeting; standalone update on a fast-moving issue | 8–15 lines |
| **Format B — Full Briefing Document** | Attached to the IM message as the complete analysis; standalone read for a scheduled briefing | 1–3 pages |

In most cases, both formats are produced together: the IM message is what the executive
reads first; the document is what they refer to if they want detail. If the user only
asks for one, produce only that one.

---

## Format A: IM Cover Message

### Structure

```
[Topic name + status signal — one line]
e.g., "[Matter Name] Update:" or "Compliance Strategy — Key Decisions Needed:"

[Issue 1]
Conclusion: [one sentence, plain language, with a clear direction]
• [supporting point — 1 line]
• [supporting point — 1 line]
• [supporting point — 1 line, max]

[Issue 2]
Conclusion: [one sentence]
• [supporting point]
• [supporting point]

[Issue 3 — if applicable, same structure]

[Closing line]
e.g., "Full analysis attached. Recommend reviewing Section X before [meeting/call]."
Or: "Need your go-ahead on [specific action] by [date]."
```

### Rules

- **8–15 lines total.** If longer, it has become a document. Move content to Format B.
- **Every issue has a conclusion.** No issue should end without a direction.
  If genuinely uncertain: "No conclusion yet — expect to confirm by [date]."
- **Bullets only.** No continuous prose. The reader is likely on mobile.
- **No legal jargon.** If you must use a term, explain it inline:
  "RPM (price-fixing risk)" or "Art. 102 (EU antitrust law for dominant companies)"
- **Flag decisions explicitly.** If the executive needs to approve something:
  "Recommend: [action] — please confirm if you agree."
- **One topic per bullet.** Do not combine two different issues in one bullet point.

### Example (structure reference — not content)

```
[Matter] Compliance Update:

1. [Risk Area A]
Conclusion: We can maintain current practice — risk is limited.
• Data shows mechanism has minimal impact on actual outcomes
• Competitors operate similar systems without enforcement action
• No immediate regulator action expected on this point

2. [Risk Area B]
Conclusion: Need to make a targeted fix; working on it.
• Regulator has flagged this specifically (confirmed via [source])
• Proposed fix: [plain-language description] — details in attachment
• Timeline: draft ready by [date], need your sign-off before [date]

3. [Workstream C]
Status: Pending external input, no action needed from you now.

Full analysis in attachment. Recommend 5-min read of Section 2 before our call.
```

---

## Format B: Full Briefing Document

### Structure

```
[Title — specific, date-stamped]
e.g., "[Matter Name] — Strategy Update | [Date] | Internal Only"

─────────────────────────────────────────
CONCLUSION
─────────────────────────────────────────
[2–4 sentences maximum. State every key conclusion with a clear direction.
Do not use "it depends" without immediately resolving it.
Example: "We recommend [X]. The main reason is [Y]. We need a decision on [Z] by [date]."]

─────────────────────────────────────────
I. [Issue 1 — plain-language title]
─────────────────────────────────────────
Bottom line: [one sentence — the conclusion for this issue]

[Supporting analysis — 3–5 bullet points]
• [Fact or finding — plain language]
• [Fact or finding]
• [Implication or risk — framed commercially where possible]
• [What this means for us specifically]

[Context recall if needed:]
"Note: In our [previous briefing on date], we flagged [X]. This update changes/confirms that."

─────────────────────────────────────────
II. [Issue 2]
─────────────────────────────────────────
[Same structure]

─────────────────────────────────────────
NEXT STEPS
─────────────────────────────────────────
1. [Owner] — [Specific action] — [by when]
2. [Owner] — [Specific action] — [by when]
3. [Owner, if executive] — [Decision needed] — [by when]
```

### Language rules

**Replace legal language with commercial language:**

| Instead of... | Write... |
|---|---|
| "This engages Article 101 TFEU" | "This is the EU's main antitrust rule — it applies here" |
| "RPM (resale price maintenance)" | "price-fixing risk — Temu/the company controls seller prices in a way that may be illegal" |
| "By object restriction" | "the regulator can treat this as illegal without needing to prove it caused harm" |
| "Preliminary assessment" | "the regulator's initial findings (the formal document before a final decision)" |
| "We are conducting further diligence" | "we are still gathering facts — expect an update by [date]" |
| "The matter remains under review" | "no conclusion yet; we expect to know by [date]" |

**Numbers over adjectives:**
- ❌ "A significant proportion of sellers reject the recommended price"
- ✅ "60% of sellers reject the recommended price"

**Active over passive:**
- ❌ "It has been determined that further analysis is required"
- ✅ "We need to run more analysis before deciding — expect results by [date]"

**Explicit call-backs:**
Every briefing document must recall the relevant prior context explicitly.
Do not write "as previously discussed." Write:
"In our [March 26] update, we flagged [X] as a risk. Since then: [update]."

### Length

1–3 pages. If it runs longer:
- Check whether every section is truly necessary for this executive's decision
- Move detailed supporting data to an appendix
- Consider whether two separate briefings would serve better

### What to put in the Conclusion section vs. the Next Steps section

**Conclusion** = what is true / what we know / what we recommend (analytical outputs)
**Next Steps** = what happens next / who does what / what decision is needed (action outputs)

Do not mix these. A conclusion that says "we will do X" belongs in Next Steps.
A next step that says "the risk is Y" belongs in the Conclusion.

---

## Step 3: Common Failure Modes to Avoid

**Failure 1: Burying the conclusion**
The executive reads the first paragraph and the last paragraph. If the conclusion is in
paragraph 4, it will not be read until after patience has run out.
Fix: Open every section with its conclusion. Open the document with the overall conclusion.

**Failure 2: Explaining the law instead of explaining the risk**
The executive does not need to understand how Article 102 works. They need to understand
what happens to the company if the risk materializes.
Fix: Frame every legal issue as a business consequence. "If the regulator finds against us
on this point, the likely outcome is [fine / required operational change / public decision]."

**Failure 3: Leaving the executive with nothing to decide**
A briefing that ends with "we are monitoring the situation" gives the executive no reason
to have read the document.
Fix: Every briefing must have a Next Steps section with at least one item that requires
the executive's input, decision, or sign-off.

**Failure 4: Assuming prior context**
The executive has not re-read the previous briefing before opening this one.
Fix: Any reference to prior work must include a one-line recall.
"The [pricing mechanism] we flagged in January — the one where [plain-language description]
— has now [update]."

**Failure 5: Using precision as a proxy for clarity**
Legal precision is valuable in a court document. In an executive briefing, precision that
makes a sentence hard to parse is a cost, not a benefit.
Fix: When in doubt, use the simpler word. Use the shorter sentence. Accuracy can be
preserved in an appendix or footnote; the main text should be navigable at speed.

---

## Quick Reference Card

```
FORMAT A (IM message):    8–15 lines | bullets only | conclusion per issue | no jargon
FORMAT B (document):      1–3 pages | conclusion first | plain language | explicit call-backs
BOTH FORMATS:             Bottom line up front | numbers > adjectives | always end with action
NEVER:                    "It depends" without resolution | legal terms without translation
                          | assume prior context | passive voice for conclusions
```
Done
上面就是完整内容，全选复制后粘贴到GitHub的编辑器里。

操作步骤再说一遍：

点页面右上角 "+" → "Create new file"
文件名输入框里输入 skill/SKILL.md（输入斜杠时会自动变成目录）
把上面输出的全部内容粘贴进大文本框
页面底部 Commit message 填 Add skill/SKILL.md，点 "Commit changes"
完成后repo就齐了，给我看一下最终截图确认一下。



