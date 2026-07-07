# 90-Day Plan

> A phased schedule from zero to hireable proof of capability. Follow the phases in order; each phase assumes completion of the previous one.

---

## Phase 1: Foundations
**Days 1–30**

| Week | Focus | Deliverable |
|------|-------|-------------|
| 1 | Python fundamentals: functions, classes, data structures, venv | 3 small scripts exercising core patterns |
| 2 | Python async + SQL: asyncio/httpx, SELECT, JOIN, GROUP BY | Working async script that queries a DB |
| 3 | Git, CLI, Linux: git workflow, bash, curl, jq | Git-tracked project with meaningful commits |
| 4 | First LLM API calls: OpenAI/Anthropic, streaming, error handling | Script that calls an LLM, streams response, handles errors |

**Day 1 rule**: The smallest thing you can build today — even if it's just "print the response from GPT-4o-mini" — is infinitely better than waiting until you feel ready.

**Publish**: Write one thread on X about what you built and what you learned. The audience is yourself from 2 weeks ago.

---

## Phase 2: Build the Proof
**Days 31–60**

| Week | Focus | Deliverable |
|------|-------|-------------|
| 5 | Embeddings + vector search | Semantic search on a small document set |
| 6 | RAG pipeline end-to-end (chunk → embed → retrieve → generate → cite) | **Project 1:** Working RAG Q&A on your data |
| 7 | Agent frameworks: function calling, tool definition, planning, error recovery | Agent with 2+ tools, shown in a notebook |
| 8 | Multi-step agents + memory + agent safety | **Project 2:** Agent that uses 3+ tools with state |

**Publish**: Write technical threads for each project. Show your architecture diagram, the hardest bug you fixed, and what you'd do differently.

---

## Phase 3: Ship & Scale
**Days 61–90**

| Week | Focus | Deliverable |
|------|-------|-------------|
| 9 | Docker, Docker Compose, secrets management | Containerised your RAG app |
| 10 | Cloud deploy (Railway/Render/Fly.io) + monitoring | **Project 3:** Deployed public URL with basic monitoring |
| 11 | Open source contributions + cold outreach | One merged PR and 5 cold outreach emails with demo |
| 12 | Specialise + portfolio polish | Portfolio README, demo video, focused practice |

**Publish**: Long-form breakdown of Project 3 — architecture, trade-offs, deployment lessons. This is your strongest signal.

---

## Trap Checklist

| Trap | Why It's Dangerous | How to Avoid |
|------|--------------------|-------------|
| Tutorial hell | Infinite consumption without building | Ship something on Day 1, no matter how small |
| Waiting to "feel ready" | Readiness is a feeling, not a state | Start before you're ready. Fix as you go. |
| Wrong order | Learning deployment before APIs | Follow the stack order strictly |
| Private repos | Zero proof signal | Make everything public by default |
| Copying code you can't explain | You'll fail any technical interview | For LLM-generated code, always ask "explain line by line" |
| Scope creep on projects | Nothing ships | Cut scope ruthlessly. MVP first, polish later. |
| Isolation | Slow progress, no accountability | Build with friends, post in public, join a cohort |

---

## Success Criteria

By day 90, you should have:

- [ ] **9 stack skills** exercised in real projects
- [ ] **3 public GitHub repos** with working AI projects
- [ ] **10+ public posts** explaining your builds and architecture decisions
- [ ] **1 deployed product** at a public URL
- [ ] **1 open source contribution** (merged or meaningful PR)
- [ ] **5+ cold outreach emails** sent to companies/teams you want to join
- [ ] A clear answer to: "What do you specialise in?" (RAG, agents, or AI product engineering)
