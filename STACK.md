# Learning Stack

> Follow this order strictly. Each layer is prerequisite to the next.

| # | Skill | Why It Matters | Suggested Depth |
|---|-------|----------------|-----------------|
| 1 | **Python** | Lingua franca of AI. Functions, classes, async — critical for API-heavy work | Build one working project |
| 2 | **SQL + Data Handling** | Every AI system touches data. Queries, joins, indexing, ETL basics | Be fluent; can query any database |
| 3 | **Git, CLI, Linux Basics** | You'll live in the terminal. Git workflow, bash, file system, processes | Daily comfort; not expert |
| 4 | **REST APIs + LLM Integration** | The core skill. Calling models, rate limits, error handling, streaming | Build one multi-API integration |
| 5 | **Embeddings + Vector Search** | Foundation of retrieval. Understand embeddings conceptually, use pgvector / Pinecone | Implement a semantic search |
| 6 | **RAG (Retrieval Augmented Generation)** | End-to-end grounded generation. Chunking, retrieval, prompt construction, hallucination prevention | Build a full RAG pipeline on your data |
| 7 | **Agent Frameworks + Tool Use** | Agents plan, reason, and call tools. Tool definition, function calling, error recovery, multi-step plans | Build an agent that uses 3+ tools |
| 8 | **Deployment + Basic MLOps** | "Works on my machine" doesn't count. Docker, cloud deploy, monitoring, eval | Deploy one thing publicly |
| 9 | **AI Dev Tools** | Master the tools that do the job. Claude Code, Cursor, Copilot, workflow automation | Daily professional use |

---

## Layer-by-Layer Details

### 1. Python
- Functions, classes, decorators, context managers
- `asyncio` and `aiohttp` / `httpx` for async API calls
- Environment management (venv, uv, pip)
- Data structures: dicts, lists, sets, comprehensions
- **Pitfall**: Shallow understanding of async will break production code.

### 2. SQL + Data Handling
- SELECT, JOIN, GROUP BY, subqueries, window functions
- Basic data cleaning and transformation (pandas or polars)
- File formats: JSON, CSV, Parquet
- **Pitfall**: Thinking ORMs replace knowing SQL. They don't.

### 3. Git, CLI, Linux
- `git add/commit/push/pull/merge/rebase`
- `curl`, `jq`, `grep`, `awk`, pipes
- File permissions, environment variables, process management
- `tmux` or `screen` for long-running processes
- **Pitfall**: Avoid GUI Git clients early — learn the CLI first.

### 4. REST APIs + LLM Integration
- HTTP methods, status codes, headers, rate limiting
- Calling OpenAI / Anthropic APIs with proper error handling
- Streaming responses, tokens, context windows
- Retry logic, exponential backoff
- **Pitfall**: Hardcoding API keys, ignoring rate limits, no retry logic.

### 5. Embeddings + Vector Search
- What embeddings are (semantic vectors, not magic)
- pgvector, Pinecone, Chroma, or Qdrant
- Similarity search: cosine similarity, dot product
- Index types and trade-offs
- **Pitfall**: Assuming vector search replaces keyword search. Use both (hybrid).

### 6. RAG (Retrieval Augmented Generation)
- Chunking strategies (fixed-size, semantic, recursive)
- Embedding + storing documents
- Retrieval + prompt construction
- Evaluating retrieval quality and generation quality
- **Pitfall**: Chunking naively (too small = lost context, too large = noise).

### 7. Agent Frameworks + Tool Use
- Function/tool calling (OpenAI tool use, Anthropic tool use)
- Planning and decomposition of tasks
- Error recovery and re-prompting
- Frameworks: LangGraph, CrewAI, or raw function calls
- **Pitfall**: Letting agents loop infinitely — always set max steps and timeouts.

### 8. Deployment + Basic MLOps
- Docker, Docker Compose
- Deploy to Railway / Render / Fly.io / Vercel
- Environment variables, secrets management
- Monitoring: logging, error tracking, basic eval
- **Pitfall**: Deploying without observability. You'll debug blind.

### 9. AI Dev Tools
- Claude Code, Cursor, Copilot, Continue.dev
- Prompt engineering for coding assistants
- Workflow automation with AI
- **Pitfall**: Letting the AI write code you don't understand. Always review and learn from the output.
