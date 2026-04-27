# Sajjad Khan

Researcher and engineer working on agentic AI, multi-agent LLM systems, and
distributed systems infrastructure. I am especially interested in optimistic
concurrency control for shared LLM state, formal verification of multi-agent
coordination protocols, and the engineering of reliable autonomous AI
infrastructure.

## Current research

**S-Bus: Automatic Read-Set Reconstruction for Multi-Agent LLM State
Coordination.** A Rust transactional middleware that uses a server-side
DeliveryLog to automatically reconstruct each agent's read-set from observed
HTTP traffic, enabling optimistic concurrency control over shared LLM state
without agent-side SDK changes. Empirical safety parity demonstrated against
PostgreSQL 17 SERIALIZABLE and Redis 7 WATCH/MULTI across 884,110 commit
attempts on three independent backends. Mechanised in TLAPS, TLC, and Dafny.

- **System:** [`sbus`](https://github.com/sajjadanwar0/sbus) — Rust workspace
  (server, baselines, proxy)
- **Mechanised proofs:** [`sbus-formals`](https://github.com/sajjadanwar0/sbus-formals) — TLA+, TLAPS, Dafny
- **Experiments:** [`sbus-experiments`](https://github.com/sajjadanwar0/sbus-experiments) — Python harness reproducing every paper measurement

Preprint: 2026 (arXiv link — TBA).

## Background

Eight years of software-engineering experience across distributed backends,
production AI systems (RAG over compliance content, and full-stack
applications, in addition to the research above.
