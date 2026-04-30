# On The Rails

**Production is not a playground.**

A hardened Standard Operating Procedure (SOP) for running high-stakes AI coding agents in real production environments.

### Philosophy

This SOP treats AI coding agents as trusted but **strictly governed** collaborators — not casual assistants.  
It is designed for situations where real users, real data, and real money are at stake.

### Key Features

- Strong ownership bias (“our code/config is the problem until proven otherwise”)
- Mandatory structured hypothesis before every fix
- Hard anti-augering rule (max 2 attempts per approach, then forced strategy change)
- Autonomous mode **OFF by default**
- Explicit approval required for all destructive and privileged actions

### Enforcement Model

What makes this SOP effective is its **layered enforcement**:

- **Pre-action hooks** in the Claude CLI enforce command hygiene, path restrictions, destructive action gates, and other operational constraints.
- **Git pre-commit hooks** ensure commits are tied to accepted tasks and protect sensitive files.
- The combination of strict rules + mechanical guardrails dramatically reduces loops, scope creep, and silent failures.

### Contents

- **[SOP.md](SOP.md)** — Full detailed Standard Operating Procedure
- **[AGENTS.md](AGENTS.md)** — Concise rules optimized for the AI agent to follow directly
- **[tj.sh.CLI.md](tj.sh.CLI.md)** — Task CLI reference (for implementing similar workflow tooling)

### How to Use

1. Read **[SOP.md](SOP.md)** for the complete rule set.
2. Use **[AGENTS.md](AGENTS.md)** as the core instruction set when configuring your AI coding agent.
3. Adapt the principles and especially the **pre-action hooks + git hook** approach to your own environment.

Best suited for production dev consulting, internal platform work, or any team that wants AI agents to operate with high reliability and low risk.

---

**Feedback welcome**  
If you're running AI agents in serious production settings, I'd love to hear what enforcement mechanisms you consider essential.

Made with rigor.
