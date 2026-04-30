# On The Rails

**Production is not a playground.**

A hardened Standard Operating Procedure (SOP) for running high-stakes AI coding agents in real production environments.

### Philosophy

This SOP treats AI coding agents as trusted but strictly governed engineers — not casual assistants.

It enforces discipline around:
- Ownership and root-cause bias
- Hypothesis-driven fixes
- Anti-augering (no repeated failed attempts)
- Strict scope control
- Mechanical safety guardrails

### Core Highlights

- **Own It First**: Always assume the problem is in our code/config until proven otherwise.
- **Hypothesis Discipline**: Every fix requires explicit hypothesis, expected outcome, failure criteria, and silence handling.
- **Anti-Augering Rule**: Hard cap of 2 attempts per approach — then forced strategy change.
- **Autonomous Mode OFF by default** — explicit opt-in only.
- **Destructive Actions** require explicit user approval.
- Strong preference for evidence over speculation.

Designed for production-first dev consulting and internal platform work where reliability matters more than speed.

### Files

- **[SOP.md](SOP.md)** — Full detailed Standard Operating Procedure
- **[AGENTS.md](AGENTS.md)** — Concise rules for direct agent consumption
- **[tj.sh.CLI.md](tj.sh.CLI.md)** — Task CLI reference

### Who Should Use This

Teams and individuals running AI agents (Claude Code, Cursor, Aider, etc.) on real systems with real consequences.

---

**Feedback welcome.**  
If you're building or running production AI agents, I'd love to hear what rules you consider non-negotiable.
