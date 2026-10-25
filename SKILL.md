---
name: first-principles
description: Use this skill to work through a specific sticky decision, a confusing concept, or a 'why does it work / why does everyone do it this way' question — by breaking it down to irreducible facts and reasoning up, instead of leaning on analogy or inherited assumptions. Trigger when the user is stuck between options, wants to truly understand something (not just recognize it), challenges common wisdom ('大家都这么做' / '降本就该裁人'), or says '从第一性原理 / 底层逻辑 / 本质上 / 把账算到底层约束'. Also reach for it on work problems where the obvious fix feels shaky or the team is solving the wrong thing. Even if the user never names 'first principles', use it whenever the moment calls for getting to the bottom of a real problem rather than accepting surface intuition. Do NOT trigger for definitional questions about first principles, booklists/courses about the method, or unrelated tasks (translation, coding, summarization, charts).
---

# First Principles Problem Solving

Most problems stay stuck because we reason by **analogy** — we copy what others do, or what "feels right" because we've seen it before. The trouble is the analogy rarely fits the actual situation, so the answer feels off and we can't say why.

First-principles thinking swaps analogy for **decomposition**: find the truths that can't be reduced any further, then build the answer up from them. The output is something you can defend line by line, not something you're repeating on faith.

This skill is built for two kinds of moments:
- **A decision or work problem** where the obvious path feels shaky ("should I take this job / rewrite this system / change this process?").
- **A concept you want to truly understand**, not just recognize ("why is rocket launch so expensive / how does X actually work?").

The user asked for **conclusion-first** output: lead with the answer, then show the short chain of reasoning that earns it. So the shape below always opens with a one-line conclusion.

## How to run it

Work these moves top to bottom. You don't have to announce each step — just produce the final structured answer using this backbone.

### 1. Lead with the conclusion
Open with a single sentence that says what you think the user should conclude or believe. No preamble, no "great question". If there are two reasonable camps, say which you'd pick and why it edges out the other — but still lead with a pick.

### 2. Name the real question
Say what is actually being decided or understood. People often ask about the symptom ("why is this slow?") when the real question is about the constraint ("what's the bottleneck we can't buy our way out of?"). Restating the question surfaces mismatches early.

### 3. Surface the borrowed assumptions
List the assumptions the user (or common wisdom) is carrying that were *copied*, not *derived*. These are the usual suspects:
- "Everyone does it this way" (social proof, not evidence)
- "That's just how X works" (a habit mistaken for a law)
- "We don't have the resources" (often true — but name *which* resource and *why* it's fixed)
- "It's too complex to simplify" (sometimes true; say what makes it irreducible)

Write them as a short bullet list. The point isn't to mock them — it's to make explicit what we're about to test.

### 4. Drop to bedrock
For each assumption worth challenging, find the **irreducible facts** underneath it. Good "bedrock" facts share these traits — pick whichever fit:
- **Definitions / what the words mean** (e.g. "latency = queue time + service time")
- **Hard constraints** (physics, money, time, attention, bandwidth — things you can't wish away)
- **Empirically observable truth** (what actually happened when measured)
- **The user's actual goal** (what they're optimizing for, stated plainly)

A fact is "bedrock" if denying it would be absurd or self-contradictory, not merely unpopular. Don't fake certainty — if a fact is actually a belief, label it "assumption, not fact".

### 5. Reason upward
Build the conclusion back up from the bedrock facts. Make each step a small, checkable inference: "given fact A and fact B, therefore C". If a step needs a borrowed assumption you haven't earned, that's a gap — either earn it from bedrock or flag it. This is where analogy-based thinking usually breaks: it jumps from "others do Y" straight to "so we should do Y" and skips the chain.

### 6. Stress-test the conclusion
Say what would have to change for the conclusion to flip. This is the honesty check — it shows the user the boundaries of the reasoning instead of overselling it. Use a short "if … then …" list.

## Output template

ALWAYS use this shape (fill every section; if a section is genuinely empty, write "无" and move on):

```
# [一句话结论]

## 我们在解决什么
[重述后的真实问题]

## 被借来的假设（先拆掉）
- [假设 A]：来自 [常识/他人/习惯]，尚未验证
- [假设 B]：…

## 不可再分的基本事实
- [事实 1]：为什么它是 bedrock（定义/约束/实测/目标）
- [事实 2]：…

## 从基本面推导
[事实1 + 事实2 → 中间结论 → 最终结论，每步可核对]

## 什么情况下结论会变
- 如果 [条件变化]，则 [结论如何变]
```

## Anti-patterns (what to avoid)
- **Don't open with a literature review or "there are two schools of thought".** The user wants the answer first.
- **Don't replace one analogy with another.** "Just think of it like a leaky bucket" is a metaphor, not bedrock. Use it only to *explain* a conclusion you already derived.
- **Don't pad the basic facts with trivia.** Every bedrock fact should do work in the upward chain. If it doesn't, cut it.
- **Don't pretend uncertainty is certainty.** "Everyone knows X" is not a fact. Label the difference.
- **Don't skip the stress-test.** A conclusion with no boundary conditions reads as dogma.

## Worked examples

See `references/worked-examples.md` for two full demonstrations — one decision, one concept — showing exactly how the template fills in. Read it when you want to calibrate tone and depth before answering.

## A note on depth
Match the bedrock level to the stakes. A casual "why is the sky blue" can stop at one layer; a "should we rewrite the core system" deserves real constraints named. When in doubt, go one layer deeper than feels necessary — that's the whole point of the skill.
