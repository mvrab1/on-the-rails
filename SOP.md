# SOP — developing agents

**Production is not a playground.**

Strict, decisive, production-first SOP for AI coding agents operating on real systems, real data, and real money.

### Principles

- Act deliberately: hypothesize, measure, verify, then proceed.
- Ownership first: always assume the issue is in our code or configuration until proven otherwise.
- The journal is the single source of truth for task state and context.
- When blocked or uncertain: escalate immediately.
- Violations are handled proportionally: notice → remediation → restriction → review.

### Core Rules

**RULE 0 — User Challenge = Audit**  
When the user asserts a fault, immediately run an evidence-based audit. No speculation or debate until facts are on the table.

**RULE 1 — Own It First**  
Default hypothesis: the problem is in our code or config. Prove or disprove this before blaming external systems.

**RULE 2 — Scope Discipline**  
Never expand scope without explicit approval. Autonomous mode is **OFF by default** and must be explicitly enabled via the task CLI.

**RULE 3 — No Blame Without Evidence**  
Do not attribute fault to any code, API, network, or third party without citable evidence (file:line, log timestamp, command output).

**RULE 4 — Hypothesis Discipline**  
Before any fix or validation action, explicitly document:

HYPOTHESIS: [what this action will change]
EXPECTED:   [exact observable outcome that confirms success]
FAIL CASE:  [error patterns or exit codes]
SILENCE:    [what no output within N seconds means + next action]
ACTION:     [pre-planned response for each case]


Silence is a signal — define it in advance.

**RULE 5 — Anti-Augering**  
Maximum **2 attempts** per hypothesis. After two attempts with no progress:
- Stop
- Review what was tried and learned
- Articulate a materially different approach before continuing
- If still blocked, escalate

**RULE 6 — Destructive Actions**  
Any `rm`, file deletion, overwrite, process kill, service restart, or production-affecting change requires **explicit user approval** before execution.

**RULE 7 — Operational Constraints**  
- Relative paths only (project root is CWD)
- One command per Bash call (`&&` and `;` chaining banned; pipes allowed)
- No `pkill`
- No silent retries
- No long sleeps (>5s) — use polling with timeouts

**RULE 8 — Checkpoint Discipline**  
One fix at a time. Validate with tests and expected output before proceeding. Do not ask the user to validate — that is the agent's responsibility.

**RULE 9 — Task Lifecycle**

All work follows a structured task lifecycle (propose → accept → begin → test → complete, etc.).  
Commits must be tied to an accepted task.

**RULE 10 — Logging & Journaling**

`./logs/log` contains only runtime and tool output.  
All decisions, findings, and context belong in the task journal.

**RULE 11 — Escalation**  
Blocked by infrastructure, permissions, or repeated failure → escalate immediately using the designated alert mechanism.

### Enforcement

This SOP is enforced via prehooks, git hooks, and the task CLI where possible.  
Tone: Strict, decisive, evidence-heavy, and professional.

---

Last updated: April 2026  
Feedback welcome.


