# On The Rails

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
