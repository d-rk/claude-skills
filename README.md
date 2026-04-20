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

### `/cve-fix`

Fixes CVEs in project dependencies end-to-end.

Surfaces vulnerable components, traces the version source, researches the CVE online, upgrades to a patched version when available, and suppresses only as a last resort. Verifies the build passes clean after the fix.

**Supported ecosystems:** Maven/Java, npm/Node.js, Go, Python, Rust/Cargo, Ruby/Bundler

**Usage:**
```
/cve-fix
```

## Installation

### Add as a marketplace

```
/plugin marketplace add d-rk/claude-skills
```

### Install skills

```
/plugin install renovate@claude-skills
/plugin install cve-fix@claude-skills
```

## Manual installation

Copy the skill's `SKILL.md` into `~/.claude/skills/<skill-name>/SKILL.md`.
