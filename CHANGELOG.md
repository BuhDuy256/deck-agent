# Changelog

All notable changes to this project are recorded here.

## [Unreleased]

### Added

- Build workflow for a five-person team (`WORKFLOW.md`): version planning, phases 1–6, version close, test tiers (CI, eval, manual), full and light builds, an as-built layer.
- Agent instructions (`AGENTS.md`, `CLAUDE.md`) and skills in `.agents/skills/`, mirrored to `.claude/skills/` and `.codex/skills/`.
- Public docs in `docs/` and internal docs in `dev/`: target spec templates and criteria, version layout, plan and as-built templates, research style, meeting notes.
- GitHub issue templates, PR template and CODEOWNERS for the protected paths.
- "No agent attribution" rule in `AGENTS.md` and `CLAUDE.md`, and a project setting that turns off Claude Code commit and PR attribution.

### Changed

- The `commit` and `commit-push` skills no longer add a `Co-Authored-By` trailer for an AI agent.
