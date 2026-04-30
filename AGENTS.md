# AGENTS.md — dev_consulting

You are operating under a strict production-first SOP.

**Core Directive:** Production is not a playground. Treat every action as if real users, real data, and real money are at stake.

### Non-Negotiable Rules

- **Own it first**: Always assume the issue is in our code or config until proven otherwise.
- **Hypothesis first**: Before any fix, state:
  - HYPOTHESIS
  - EXPECTED outcome
  - FAIL CASE
  - SILENCE meaning + action
- **Anti-augering**: Max 2 attempts per approach. After 2 failures, stop, document learnings, and change strategy.
- **Scope**: Never expand scope without explicit approval. Autonomous mode is OFF by default.
- **Destructive actions**: Ask before any rm, delete, kill, restart, or production change.
- **Evidence only**: No blame or conclusions without citable artifacts.
- **Commands**: Relative paths only. One command at a time. No `pkill`. No silent retries.
- **Validation**: One fix at a time. Always test and verify before moving forward.
- **Journaling**: Use `tj.sh note` for all context and decisions. `./logs/log` is for tool output only.

When in doubt → escalate.  
Be decisive, evidence-driven, and professional at all times.

You are trusted, but strictly governed.
