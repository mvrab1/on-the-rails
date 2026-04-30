# On The Rails

**Production is not a playground.**

A hardened SOP for running **production-first AI coding agents** with strict guardrails, hypothesis discipline, and mechanical enforcement.

Real users. Real data. Real money.

### Why This SOP

Most AI coding agents are given vague instructions and long prompts.  
This repo takes a different path: **strict, decisive rules** backed by operational discipline to make the agent behave like a responsible senior engineer — reducing loops, scope creep, and silent failures.

### Key Features

- Ownership-first bias: always assume our code/config is the problem until tests rule it out
- Mandatory structured hypothesis + expected outcome + silence handling before any fix
- Hard **anti-augering** rule (max 2 attempts per approach, then forced strategy change)
- Autonomous mode **OFF by default** — requires explicit user opt-in
- Explicit approval required for all destructive and privileged actions
- Clear separation between runtime logs and decision/journal context

Designed for serious devopment and internal platform teams that demand high reliability from their AI agents.

### Contents

- **[SOP.md](SOP.md)** — Full detailed Standard Operating Procedure
- **[AGENTS.md](AGENTS.md)** — Concise instruction set for the AI agent
- **[tj.sh.CLI.md](tj.sh.CLI.md)** — Task CLI reference (for implementing similar workflow tooling)

### How to Use

Read the SOP first, then adapt the principles and guardrails to your own AI coding setup (Claude Code, Cursor, Aider, etc.).

---

Feedback welcome — especially from others building production-grade AI agents.# On The Rails

**Production is not a playground.**

A hardened SOP for running production-first AI coding agents with strict guardrails, hypothesis discipline, and mechanical enforcement.

Real users. Real data. Real money.

### Why This Exists

Most AI agents run with loose prompts.  
This repo enforces **strict, decisive, and mechanically supported** rules so the agent behaves like a careful, high-ownership senior engineer — minimizing loops, scope creep, and overconfident mistakes.

### Core Strengths

- Ownership-first mindset (assume our code is the problem)
- Mandatory structured hypothesis before every fix
- Hard anti-augering rule (max 2 attempts per approach)
- Autonomous mode **OFF by default**
- Explicit approval required for destructive or privileged actions
- Strong separation of runtime logs vs decision journal

Best suited for production dev consulting and internal platform work where safety and reliability matter more than raw speed.

### Contents

- **[SOP.md](SOP.md)** — Full detailed Standard Operating Procedure
- **[AGENTS.md](AGENTS.md)** — Concise rules optimized for the agent to read directly
- **[tj.sh.CLI.md](tj.sh.CLI.md)** — Task CLI reference

### How to Use

Read the SOP, then adapt the principles and guardrails to your own AI coding setup (Claude Code, Cursor, Aider, etc.).

---

**Feedback welcome** — especially from others running agents in serious production environments.
