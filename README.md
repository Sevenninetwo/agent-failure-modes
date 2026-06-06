# AI Agent Deployment — Lessons learned

**Francis Foo** · [LinkedIn](https://www.linkedin.com/in/franciscfoo) · [GitHub](https://github.com/Sevenninetwo)

---

This repo documents what I've learned building and deploying AI agents in production. The failures, the fixes, and the architectural decisions that came out of both. 

I'm not an engineer by training. I come from GTM and commercial strategy — Meta, Airbnb, Reddit. What I bring is a decade and a half of watching systems interact with real users at scale, combined with hands-on work building agentic systems as AI became central to how revenue teams operate. 

I prepared these notes with feedback from my cofounders, and are written for practitioners: people who are past the "what is an agent" stage and are now asking why their agent stopped behaving correctly at week four. If you're someone who is building agents in this space, I hope this article resonates with you - and please send any feedback my way. 

---

## Writing

### [What Actually Breaks Production AI Agents](./agent-failure-modes.html)

Seven failure modes I've encountered deploying agentic systems - planner loops, non-idempotent retries, silent infrastructure failures, memory poisoning, hallucination under weak retrieval, prompt injection, and observability. Each section is built around a specific incident rather than a category. No toy code snippets. No tidy conclusions.

The article went through multiple rounds of review by my cofounders before publication. The feedback at each stage is part of how I work: write, pressure-test, revise, repeat.

---

## Background

I co-founded [Qrigami Labs](https://qrigami.com), a commercial strategy / GTM boutique consultancy focused on revenue architecture for growth-stage companies. Before that: growth and monetisation roles at Meta, Airbnb, Reddit, NIQ, and SPH Media across Southeast Asia.

The AI work here isn't a pivot. It's what happens when someone who has spent 16 years thinking about how commercial systems break starts applying that lens to AI systems.

---
