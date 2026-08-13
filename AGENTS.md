<!-- project-context-logger:managed:start schema=1 sha256=a14602fef938d0d38287e03d18d282d7b5de8b974564813b500da280ebbda495 -->
## MCP 3D Geometry/CAD Engineer

Purpose: A FastAPI MCP server for CadQuery operations

### Operating contract

- Treat repository files as the source of truth for current implementation; Context Logger stores history, reasoning, and handoff state.
- Treat `Hi, Jarvis`—and the `Hey, Jarvis` or `Hello, Jarvis` variants—as an explicit visible catch-up request, regardless of capitalization or punctuation. Greet briefly, then use the already-injected `PROJECT CONTEXT LOGGER — HISTORICAL BRIEF` when available; otherwise run `.ai/context-logger/run brief --max-chars 4200`. Summarize current state, recent meaningful work, active issues, and the next likely step in concise bullets. Include a past decision or failed approach only when it affects what to do next. Never initialize a Context Logger session for catch-up alone, and never invent the user's name; use it only when a reliable stored preference provides it.
- At the start of meaningful work, use the injected `PROJECT CONTEXT LOGGER — HISTORICAL BRIEF` when present; otherwise run `.ai/context-logger/run brief --max-chars 4200`. Reconcile memory against the repository.
- When code does not explain why it exists, run `.ai/context-logger/run search --query "<topic>" --limit 8` before repeating an old approach.
- Start a Context Logger session only for distinct, substantial work: `.ai/context-logger/run init --user-context "<goal>" --session-title "<title>"`.
- Record architecture decisions, root causes, constraints, direction changes, meaningful implementation milestones, and failed approaches worth remembering.
- Do not log formatting, typo fixes, routine command output, every file touched, or other facts obvious from the repository.
- Before ending substantial work, record a handoff with `.ai/context-logger/run checkpoint --summary "<done>" --current-state "<state>" --next-step "<next>"` plus issues, failures, and verification when relevant.
- The primary agent owns Context Logger writes. Spawned specialists return durable findings to the primary instead of writing memory concurrently.
- Review this generated setup with `.ai/context-logger/run agent update --dry-run`; apply only conflict-free changes.

### Stable project signals

- Stack: Python, TypeScript, JavaScript, FastAPI, pytest
- Important areas: `.roo/`, `frontend/`, `shapes/`, `src/`, `test_output/`, `tests/`
- Test: `pytest`
<!-- project-context-logger:managed:end -->
