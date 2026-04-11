# Changelog

All notable changes to this project will be documented in this file.
Format follows [Keep a Changelog](https://keepachangelog.com/).

## [0.5.0] - 2026-04-11

### Added
- CHANGELOG.md for version tracking
- ETHOS.md with core philosophy extracted as standalone document
- Voice guidelines with AI slop blacklist in SKILL.md
- Completion status protocol (DONE / DONE_WITH_CONCERNS / BLOCKED / NEEDS_CONTEXT)
- Session memory protocol for within-session user context recall
- PM Sprint workflow for end-to-end feature development
- Template generation concept (SKILL.md.tmpl) for future scalability
- Multi-platform host config concept in TODOS.md

### Changed
- TODOS.md now uses effort estimates (S/M/L) and priority labels (P0-P3)
- README.md and README.zh-CN.md updated with links to ETHOS.md and CHANGELOG.md

## [0.4.0] - 2026-03-29

### Added
- Coaching protocol: explicit opt-in coaching mode with 5 behaviors
- 6 domain-specific coaching rules in each knowledge module
- Coaching gold transcript example (examples/coaching-discovery.md)
- Starter prompts for coaching mode (STARTER-PROMPTS.md)
- TODOS.md with product roadmap

### Changed
- SKILL.md: added Coaching Protocol section with precedence rules
- README.md: added coaching mode documentation and example link
- README.zh-CN.md: added coaching mode section

## [0.3.0] - 2026-03-06

### Added
- Cross-platform support: Claude Code, Codex, Cursor, Windsurf
- Chinese README (README.zh-CN.md)
- Template attribution and source references
- CONTRIBUTING.md

### Changed
- package.json: added multi-platform keywords and distribution metadata

## [0.2.1] - 2026-03-05

### Added
- Competitive analysis template (templates/competitive-analysis.md)
- Lean UX Canvas template (templates/lean-ux-canvas.md)

## [0.2.0] - 2026-03-05

### Added
- Rewritten README with clear positioning and activation-first examples
- Optimized skill description for vector search discoverability
- Consolidated naming across all files

### Changed
- README.md: complete rewrite focused on workflows, not features

## [0.1.0] - 2026-03-03

### Added
- Initial release with 6 knowledge domains
- 30+ PM frameworks across discovery, strategy, artifacts, finance, career, AI
- 12 templates for PM deliverables (PRD, user story, roadmap, etc.)
- 32 SaaS metrics with formulas and stage benchmarks
- Routing table with intent matching
- Universal quality gates (assumptions, measurability, specificity, tradeoffs, anti-patterns)
- 4 worked examples (SaaS diagnostic, PRD review, director coaching, coaching discovery)
- package.json for clawhub/npm distribution
