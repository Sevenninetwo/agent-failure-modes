# AI Agent Deployment — Field Notes

**Francis Foo** · [LinkedIn](https://www.linkedin.com/in/franciscfoo) · [GitHub](https://github.com/Sevenninetwo)

---

This repo documents what I've learned building and deploying AI agents — not in theory, but in production. The failures, the fixes, and the architectural decisions that came out of both.

I'm not an engineer by training. I come from GTM and commercial strategy — Meta, Airbnb, Reddit. What I bring is a decade and a half of watching systems interact with real users at scale, combined with hands-on work building agentic systems as AI became central to how revenue teams operate.

These notes are written for practitioners: people who are past the "what is an agent" stage and are now asking why their agent stopped behaving correctly at week four.

---

## Writing

### [What Actually Breaks Production AI Agents](./agent-failure-modes.html)

Seven failure modes I've encountered deploying agentic systems — planner loops, non-idempotent retries, silent infrastructure failures, memory poisoning, hallucination under weak retrieval, prompt injection, and observability. Each section is built around a specific incident rather than a category. No toy code snippets. No tidy conclusions.

The article went through four rounds of review by a senior AI systems practitioner before publication. The feedback at each stage is part of how I work: write, pressure-test, revise, repeat.

---

## Projects

| Project | What it does | Stack |
|---|---|---|
| [AI Calendar Agent](https://github.com/Sevenninetwo/ai-calendar-agent) | Telegram bot that manages Google Calendar via natural language | Node.js · Google Calendar API · Claude API · Railway |
| [AI Expense Agent](https://github.com/Sevenninetwo/ai-expense-agent) | Telegram bot that logs expenses to Google Sheets | Node.js · Google Sheets API · Claude API · Railway |
| [AI Transformation Playbook](https://github.com/Sevenninetwo/AI_Transformation) | Structured framework for enterprise AI adoption across five pillars | Markdown · ADKAR · Kotter's 8-Step |

---

## Background

I co-founded [Qrigami Labs](https://qrigami.com), a commercial strategy consultancy focused on revenue architecture for growth-stage companies. Before that: growth and monetisation roles at Meta, Airbnb, Reddit, NIQ, and SPH Media across Southeast Asia.

The AI work here isn't a pivot. It's what happens when someone who has spent 16 years thinking about how commercial systems break starts applying that lens to AI systems.

---

*Open to conversations about AI deployment, GTM strategy, and what actually happens when agents meet production infrastructure.*
