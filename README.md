# claude-skills

A collection of [Claude Code](https://claude.ai/claude-code) skills.

## Skills

### `/renovate`

Handles Renovate bot dependency update branches end-to-end.

Renovate bumps versions but can't adapt code to breaking changes. This skill picks up where Renovate left off: identify what changed, research breaking changes, fix the code, and verify builds and tests pass.

**Supported ecosystems:** Go, Maven/Java, npm/Node.js, Python, Rust/Cargo, Ruby/Bundler

**Usage:**
```
/renovate
/renovate renovate/some-branch-name
```

## Installation

### Add as a marketplace

```
/plugin marketplace add d-rk/claude-skills
```

### Install the renovate skill

```
/plugin install renovate@claude-skills
```

## Manual installation

Copy `skills/renovate/SKILL.md` into `~/.claude/skills/renovate/SKILL.md`.
