# On The Rails

A battle-tested Standard Operating Procedure (SOP) for running high-stakes AI coding agents in production environments.

**"Production is not a playground."**

Real users. Real data. Real money.

### Why This SOP Exists

Most AI coding agents are given loose instructions and a long prompt.  
This repo takes a different approach: **strict, decisive, and mechanically enforced** rules designed to make AI agents behave like a careful, high-ownership senior engineer — while dramatically reducing common failure modes like augering, scope creep, and overconfident mistakes.

### Core Principles

- Default to **ownership**: Always assume the issue is in our code or config until proven otherwise.
- **Hypothesis discipline**: Every fix must be preceded by a clear hypothesis, expected outcome, failure criteria, and silence handling.
- **Anti-augering**: Hard limit of 2 attempts per approach — then a forced change in strategy.
- **Scope control**: No scope changes without explicit approval. Autonomous mode is **off by default**.
- **Safety first**: Destructive actions, privileged commands, and production-affecting changes require explicit user approval.
- Strong mechanical guardrails via prehooks, git hooks, and protected file handling.

### Key Features of This SOP

- Structured hypothesis → action → verification workflow
- One fix at a time with mandatory checkpoints
- Clear escalation paths for blockers
- Strict separation between runtime logs and decision/journal context
- Proportional enforcement for SOP violations

This SOP is particularly suited for **production-first dev consulting**, internal platform work, or any environment where reliability and caution matter more than speed.

### Repository Structure

- `SOP.md` — The full Standard Operating Procedure (the heart of the repo)
- `AGENTS.md` — (optional) Lightweight version for direct agent consumption
- `examples/` — Hypothesis templates, escalation examples, etc.

### How to Use

1. Read the full SOP in [`SOP.md`](SOP.md)
2. Adapt the rules to your environment
3. Use the principles and guardrails when configuring your AI coding agent (Claude Code, Cursor, Aider, etc.)

### Who This Is For

- Engineers and teams running AI agents on real production systems
- Anyone tired of agents looping, hallucinating fixes, or quietly breaking things
- Developers who want to treat AI agents as **trusted but strictly governed** collaborators

---

**Feedback and contributions welcome.**

If you're running AI agents in serious environments, I'd love to hear what rules you consider non-negotiable.

---

Made with rigor.    
