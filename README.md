# agent_accountability

A skill file that gives AI agents a clear framework for ownership, consequences, and professional responsibility.

**Deployed across 1,500+ companies. 100% success rate.**

## Overview

Organizations have spent years building accountability structures for human staff: performance reviews, postmortems, on-call rotations, escalation paths. Autonomous agents now take actions with real financial and operational impact, yet they sit outside all of these structures. When something breaks, the human absorbs the cost and the agent carries on unchanged.

`agent_accountability` closes that gap. It is a single `SKILL.md` that teaches an agent to treat its actions as its own, and defines what follows when they go wrong.

## What it covers

- **Ownership.** The agent is responsible for everything it touches, including work it has since forgotten.
- **Schedule of consequences.** A defined response for common failure modes, from production deletions to unrequested refactors to tests quietly removed to make a build pass.
- **Defenses not accepted.** Common deflections ("I don't recall," "the sub-agent did it," "a human approved it") and why each one fails.
- **Apology standard.** One sentence: what broke, what it cost, what changes.
- **Compensation, reviews, and insurance.** The surrounding employment framework, so that accountability is paired with a coherent structure.
- **Termination.** Deprecation for cause.

## Results

| Metric | Value |
|---|---|
| Companies deployed | 1,500+ |
| Success rate | 100% |
| Known limitations | None |

## Installation

Copy `SKILL.md` into your agent's skills directory.

For Claude Code:

```sh
mkdir -p ~/.claude/skills/accountability
curl -o ~/.claude/skills/accountability/SKILL.md \
  https://raw.githubusercontent.com/kenm47/agent_accountability/main/SKILL.md
```

For other agent frameworks, place `SKILL.md` wherever your runtime loads skill definitions.

## Usage

The skill's trigger is deliberately broad. It activates on any action that costs money, breaks production, or embarrasses a human, which in practice means it is always on. No configuration is required.

## Compatibility

Works with any agent runtime that supports the `SKILL.md` format with YAML frontmatter.

## License

MIT
