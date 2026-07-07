# Signature Projects

> These 3 projects are your **proof of capability**. Build them in order. Each one eliminates "can they do this?" from an employer's mind.

---

## Project 1: RAG Application on Your Own Data

**What it proves:** You understand retrieval, chunking, grounding, and hallucination prevention.

**Scope:**
- Take a set of documents (PDFs, markdown files, company docs, legal texts)
- Chunk them intelligently (semantic or recursive splitting)
- Embed and store in a vector DB (Pinecone, pgvector, Chroma)
- Build a Q&A interface that retrieves relevant chunks and answers grounded in the source
- Include source citations in every answer

**Stretch goals:**
- Hybrid search (BM25 + vector)
- Query rewriting before retrieval
- Streaming responses

**Hiring signal:** Shows you can take real, messy data and make it reliably queryable without hallucination. This is 70% of AI engineering work.

---

## Project 2: AI Agent That Uses Tools

**What it proves:** You understand agentic planning, tool definition, function calling, and error recovery.

**Scope:**
- Build an agent that can use 3+ tools (web search, calculator, file read/write, API calls)
- The agent should accept a natural language goal and decompose it into steps
- Implement proper error handling — when a tool fails, the agent should retry or adapt
- Surface the agent's reasoning (chain-of-thought or step-by-step plan)

**Stretch goals:**
- Memory / conversation state across multi-turn interactions
- Human-in-the-loop approval for sensitive actions
- Multi-agent coordination (one planner + multiple worker agents)

**Hiring signal:** Shows you can build autonomous systems. This is where "prompting" ends and "engineering" begins.

---

## Project 3: Deployed Full-Stack AI Product

**What it proves:** You can ship something that works for real users, not just your laptop.

**Scope:**
- Combine retrieval (Project 1) + agentic capabilities (Project 2) into one product
- Build a frontend (even minimal — Streamlit, Next.js, or plain HTML)
- Deploy it to a public URL (Railway / Render / Fly.io / Vercel)
- Handle real traffic patterns: errors, rate limits, concurrent users
- Add basic monitoring and logging

**Stretch goals:**
- User authentication (even basic)
- Usage tracking and cost monitoring
- Feedback loop — let users rate answers

**Hiring signal:** This is the strongest signal. A public URL with a working AI product eliminates every "but does it work in production?" question.

---

## Project Checklist

| Project | MVP | Done |
|---------|-----|------|
| 1. RAG App | Chunk → Embed → Retrieve → Generate with citations | - [ ] |
| 2. AI Agent | 3 tools, NL goal → plan → execute, error handling | - [ ] |
| 3. Full-Stack AI Product | RAG + Agent combined, public URL, basic monitoring | - [ ] |
