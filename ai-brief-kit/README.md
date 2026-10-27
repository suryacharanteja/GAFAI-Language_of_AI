# The Language of AI: Workshop Kit

Three things from the workshop: how to talk **about** AI (a 4-sentence brief), how to talk **to** AI (a 5-part prompt), and **where to draw the line**. Nothing to install: everything is on this page.

- **Printable card (two-sided A4):** [ai-brief-card.pdf](ai-brief-card.pdf)
- **Blank worksheet:** [worksheet.md](worksheet.md)
- **The workshop case:** [case-brief.md](case-brief.md)
- **License:** [CC BY 4.0](LICENSE.md), so you can reuse and adapt it with credit

---

## 1. Talking about AI: the 4-sentence brief

Explain any AI project to someone who doesn't work in tech, in under 30 seconds.

| # | Sentence | Template |
|---|---|---|
| 1 | **What it does** | This **[tool]** takes **[input]** and gives **[output]**, so **[who]** can **[spend time on what]**. |
| 2 | **The honest promise** | It **[does what well]**, but it can **[go wrong how]**, so **[what we do about it]**. |
| 3 | **Who holds the wheel** | For **[type of task]**, **[named role]** **[checks / decides]** before **[action]**. |
| 4 | **The ask** | I need **[decision]** from **[who]** by **[date]**. |

Use the same project for all four sentences.

### Sentence 1: Name the task, not the technology

| Instead of | Say what it does |
|---|---|
| "RAG assistant" | Answers staff questions from our procedures |
| "Computer vision model" | Spots damaged items in photos |
| "Predictive maintenance model" | Flags which equipment is likely to fail next month |

### Sentence 2: What you can honestly promise

| If it… | You can promise |
|---|---|
| **Follows fixed rules** (often no AI needed) | "It does exactly what we set, every time, and nothing else." |
| **Predicts** | "It gives a likelihood, not a certainty. Here's how often it misses." |
| **Drafts or answers** (generative AI) | "It's fast and usually right (here's how often), but it can be wrong and sound sure. A person checks what matters." |
| **Acts on its own** (an agent) | "It acts only within limits we set in advance, and a named person reviews what it does." |

A good sentence 2 has both halves: **how often it goes wrong**, and **what you do about it**. "95% accurate" and "about 1 in 20 answers are wrong, so we check" are the same fact. Only the second tells people what to do.

### Sentence 3: Three levels of control

| Level | What it means | When to use it |
|---|---|---|
| **1. A person decides** | It informs. A named person makes the call. | Safety, big money, people's rights, anything you can't undo |
| **2. A person checks** | It drafts or answers. A person reviews before anyone relies on it. | Policy, customers, anything that leaves the team |
| **3. It runs alone** | No review before it acts. | Low stakes, easy to spot, easy to undo |

**The test:** if it's wrong, who gets hurt, and can we undo it? Name a role, such as "the shift supervisor", not "a human".

### Sentence 4: Ask for one decision

Every brief ends with a decision, an owner and a date. Not "thoughts?" and not "let's discuss": one thing they can say yes or no to.

### Same brief, different room

Keep all four sentences. Change the order for the person in front of you.

| Room | Order | Start with |
|---|---|---|
| Executive or sponsor | 4 → 1 → 2 → 3 | The decision you need |
| Staff who will use it | 1 → 3 → 2 → 4 | What changes in their day. Sentence 4 becomes what you need them to do. |
| Risk, legal or regulator | 3 → 2 → 1 → 4 | Who holds the wheel |

Every room hears sentence 2. Never drop the limit.

### Worked example: the procedures assistant

1. **What it does:** This assistant answers staff questions from our own procedures, with a link to the exact page, so supervisors spend less time answering the same questions.
2. **The honest promise:** It answers in seconds and shows where the answer came from, but in testing about [1 in X] answers had a mistake that sounded confident, so staff check the linked page before acting on anything important.
3. **Who holds the wheel:** For safety-critical tasks, it only points to the official procedure, and the shift supervisor confirms before anyone acts.
4. **The ask:** I need approval for an 8-week pilot in one department, and a safety lead to sign off the safety rules, by [date].

### Practice: fix this brief

A tool that predicts which customers will cancel. Every sentence below is weak. Try fixing each one before you look at the answers.

1. "We've built a churn-propensity model using gradient boosting."
2. "It will tell us exactly which customers are leaving."
3. "The system will handle retention automatically."
4. "Happy to discuss."

<details>
<summary>One way to fix it (the figures are examples)</summary>

1. This tool looks at customer history and flags who's likely to cancel next month, so the retention team can call them first.
2. It gives a likelihood, not a certainty: in testing, about 7 in 10 of the customers it flagged did cancel, so we treat it as a call list, not a verdict.
3. A retention team member decides whether and how to contact each flagged customer. Nothing goes out automatically.
4. I need approval to trial it with one retention team for six weeks, starting [date].

</details>

---

## 2. Talking to AI: the 5-part prompt

A vague prompt gets a vague answer. Give the AI all five parts.

| Part | What it covers | Example |
|---|---|---|
| **1. Role** | Who the AI should act as | "Act as a communications advisor." |
| **2. Task** | What you want done | "Rewrite this project update as a 4-sentence brief." |
| **3. Context** | The background, and who it's for | "It's for a non-technical director who must approve a pilot." |
| **4. Format** | Length, style and structure | "Plain words, under 100 words." |
| **5. Check** | What it should flag for you | "Then list anything you assumed or aren't sure about." |

### A prompt you can copy

This one turns any project description into a 4-sentence brief. Works in any AI assistant. Never include confidential details.

```
Act as a communications advisor. Rewrite the project below as a 4-sentence brief for a non-technical director: (1) what it does, in plain words; (2) what it does well, how often it goes wrong, and what we do about it; (3) who checks or decides before anything important happens; (4) the one decision I need, from whom, by when. Plain words, under 100 words. Then list anything you assumed or aren't sure about. Project: [2-3 lines, no confidential details]
```

### Before you use anything AI wrote

- **Is every fact true?** It can be wrong and sound sure.
- **Did it add anything you didn't give it?** Numbers, names and promises are the usual suspects.
- **Would you sign your name to it?** If not, it isn't finished.

---

## 3. Where to draw the line

### Seven questions before you use or buy an AI tool

| | Ask |
|---|---|
| **Fairness** | Does it work equally well for everyone it affects? |
| **Accountability** | Who answers for it when it's wrong? |
| **Transparency** | Do people know AI is involved, and can we explain its answers? |
| **Ethics** | Should we do this at all, even if we can? |
| **Safety** | What's the worst that happens if it fails, and who notices? |
| **Security** | Where does our data go, and who can see it? |
| **Sovereignty** | Where is our data stored and processed, and under whose laws? |

### Security: attackers use AI too

- Never paste confidential information into an AI tool.
- Use the AI tools your organization has approved.
- Treat urgent messages, links and voice notes with extra suspicion.

Background: in October 2026, security researchers nicknamed a wave of AI-linked security incidents "Black October". Reporting is still developing, and experts disagree on how much AI drove the attacks. Further reading:
- [CNBC, 23 Oct 2026](https://www.cnbc.com/2026/10/23/php-vulnerabilities-ai-cybersecurity.html)
- [Wikipedia, Black October (information security)](https://en.wikipedia.org/wiki/Black_October_(information_security))
- [SecurityToday, 22 Oct 2026: many attacks had been running for months](https://www.securitytoday.de/en/2026/10/22/black-october-many-attacks-had-been-running-for-months/)

### Sustainability: use AI where it earns its place

Every request uses electricity and water in data centres, and leaning on AI for everything weakens your own judgment.

- Use it where it saves real effort.
- Ask once, well, instead of five times. The 5-part prompt helps.
- Keep your own judgment for what matters most.

---

## Before your next AI conversation

- [ ] Read your four sentences out loud. Do they take under 30 seconds?
- [ ] Could your listener repeat sentence 1 to someone else?
- [ ] Have you removed every technology name your listener wouldn't use?
- [ ] Does sentence 2 say how often it goes wrong, and what you do about it?
- [ ] Does sentence 3 name a role, not "a human"?
- [ ] Does sentence 4 have one decision, an owner and a date?
- [ ] If AI helped you write it, have you checked every fact?
