# TODOS

## Coaching Protocol

### ~~Default Coaching Behavior Decision~~ (RESOLVED in v0.5.2)
**Decision:** Hybrid. Added a "framing gate" that always runs (not coaching). Serious framing issues (solution smuggling, zero metrics, scope mixing 3+ features) get one turn of pushback before output. Minor issues get inline `[flag: ...]` tags. Full coaching remains opt-in for interactive follow-up, verdicts, and conversation anti-patterns. This resolves the README contradiction without breaking activation-first.

### Role Switching System
**Priority:** P2 | **Effort:** M
**What:** Add role switching (mentor/challenger/ceo/user_voice/eng_lead) to coaching mode.
**Why:** Strongest differentiation feature. Makes coaching feel like multiple experts, not one mentor.
**Cons:** Relies on model self-discipline in pure Markdown. Cross-platform fidelity not guaranteed.
**Depends on:** v0.4 coaching rules validated as working cross-platform.
**Context:** Codex outside voice flagged that pure-Markdown role switching is aspirational. Validate v0.4 interaction rules first, then add role switching if the base coaching protocol proves reliable.

### Scenario Triggers Experiment
**Priority:** P3 | **Effort:** L
**What:** Design a safe "proactive PM suggestion" mechanism for when AI detects PM-relevant patterns during code work.
**Why:** Shifts product form from request-response to ambient coaching. High potential, high risk of annoyance.
**Cons:** Markdown can't do real event monitoring. Risk of being disruptive.
**Depends on:** v0.4 coaching validation + default behavior decision.
**Context:** Codex flagged this as a product form shift, not a content extension. Needs careful design including frequency limits and opt-out.

## Infrastructure

### Template Generation System
**Priority:** P3 | **Effort:** L
**What:** Move SKILL.md to a template-based generation system (SKILL.md.tmpl + gen script) where placeholders like `{{ROUTING_TABLE}}` and `{{QUALITY_GATES}}` are filled from source metadata.
**Why:** As knowledge modules and routing rules grow, hand-maintaining SKILL.md will drift from actual content. gstack uses this pattern with `gen-skill-docs.ts` to keep docs in sync.
**Depends on:** Project reaching 10+ knowledge modules or frequent routing table drift.
**Context:** At current scale (7 knowledge modules, ~330-line SKILL.md), hand maintenance still works, but drift is now real enough to justify a lightweight release consistency check. Revisit generation when the skill grows to 8+ domains or when template count exceeds 15.

### Multi-Platform Host Config
**Priority:** P3 | **Effort:** M
**What:** Add a `hosts/` directory with typed configs for each supported AI coding agent (Claude Code, Codex, Cursor, Windsurf, OpenClaw), enabling platform-specific behavior.
**Why:** gstack supports 8 hosts from one codebase. As AI coding tools diverge in capabilities (AskUserQuestion, file access, browser control), platform-specific adaptation becomes necessary.
**Depends on:** Identifying at least 2 concrete platform-specific behaviors worth adapting.
**Context:** Pure Markdown skills are inherently cross-platform. This becomes relevant only when adding interactive features (guided mode with AskUserQuestion) that work differently across platforms.

## Completed

### v0.5.0 (2026-04-11)
- [x] CHANGELOG.md with full version history
- [x] ETHOS.md with core philosophy
- [x] Voice guidelines and AI slop blacklist
- [x] Completion status protocol (DONE / DONE_WITH_CONCERNS / BLOCKED / NEEDS_CONTEXT)
- [x] Session memory protocol for cross-session user context
- [x] PM Sprint workflow for end-to-end feature development

### v0.4.0 (2026-03-29)
- [x] Coaching protocol with 5 behaviors
- [x] Domain-specific coaching rules (6 domains)
- [x] Coaching gold transcript example
- [x] Starter prompts for coaching mode
