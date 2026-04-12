# Product Manager Skills v0.5: Growth Domain, Sprint Workflow, and Update Notifications

**TL;DR:** v0.5 adds a 7th knowledge domain (Growth & PLG), a 6-phase PM Sprint workflow, always-on framing quality gates, voice discipline, session memory, and an auto-update notification system. 40+ frameworks across 7 domains.

---

## What Changed

### New: Growth & PLG Knowledge Domain

The biggest content addition since launch. A full knowledge module covering:

- **PLG Readiness Assessment:** PLG vs SLG decision framework, maturity levels (0-3), hybrid model guidance
- **Activation & Onboarding:** How to find your activation metric, onboarding design principles, diagnostic funnel for drop-off analysis
- **Viral & Network Effects:** Viral loop design (4 components), K-factor calculation, 5 types of virality, network effects assessment
- **Freemium & Conversion:** 4 freemium model types, conversion benchmarks, common conversion failures and fixes
- **Growth Experimentation:** 5-part experiment framework, ICE prioritization, experimentation anti-patterns
- **Growth Metrics Dashboard:** 6 weekly metrics for PLG products with formulas

Plus domain-specific quality gates (7 PLG anti-patterns, 5 experiment anti-patterns) and coaching rules.

**Try it:**
```
We're considering adding a free tier to our B2B analytics tool. Assess our PLG readiness and recommend a freemium model.
```

### New: PM Sprint Workflow

Say "take this from idea to PRD" and the skill runs 6 phases end-to-end:

1. **Discover** - Frame the problem, validate it's real
2. **Position** - Market fit, competitive context
3. **Prioritize** - Score alternatives, name tradeoffs
4. **Specify** - PRD, user stories, acceptance criteria
5. **Validate** - Experiment design, kill criteria
6. **Measure** - Metrics dashboard, feature ROI

Each phase feeds output to the next. Skip, reorder, or stop at any phase. The skill labels where you are: `[Sprint: Phase 2/6 - Position]`.

### New: Framing Gate (Always On)

This resolves a contradiction: the README promised "pushback" but coaching was opt-in. Now, serious framing issues get challenged automatically:

- Solution smuggling in problem statements
- Zero success metrics
- Scope mixing 3+ unrelated features

One turn of pushback, not an interrogation. If you say "I know, just write it," the skill proceeds immediately. Minor issues get inline `[flag: ...]` tags without blocking output.

Full coaching mode (interactive follow-up, verdicts, conversation anti-patterns) remains opt-in via "coach me."

### New: Update Notifications

A 45-line bash script checks your installed version against GitHub at session start. Cached for 60 minutes, 5-second timeout, zero telemetry. If a new version is available:

```
product-manager-skills v0.5.2 is available (you have v0.4.0).
Update: clawhub update product-manager-skills
```

### New: Voice Guidelines

12 banned AI slop words (delve, crucial, robust, comprehensive, leverage, utilize, facilitate, streamline, synergy, holistic, paradigm, ecosystem). No em dashes. No filler openings ("Great question!") or closings ("Hope this helps!"). Sharper output.

### New: Completion Status Protocol

Every output now reports a status:
- `STATUS: DONE` - request fulfilled
- `STATUS: DONE_WITH_CONCERNS` - delivered, but something is risky
- `STATUS: BLOCKED` - cannot proceed without input
- `STATUS: NEEDS_CONTEXT` - partial output, more context would help

### New: Session Memory

The skill remembers your product stage, team structure, metrics baseline, and framework preferences within a session. Labels recalled context as `[from earlier: user is Series A, 15-person team, $80k MRR]`.

### New: ETHOS.md

Core philosophy extracted as a standalone document:
1. **Thinking Before Templating** - judgment over completeness
2. **Opinions With Tradeoffs** - positions, not hedges
3. **Compression Over Completeness** - 3 bullets, not 3 paragraphs

---

## By the Numbers

| Metric | v0.4 | v0.5 |
|--------|------|------|
| Knowledge domains | 6 | 7 |
| Frameworks | 30+ | 40+ |
| Templates | 12 | 12 |
| Routing intents | ~45 | ~55 |
| Quality gate anti-patterns | ~50 | ~62 |
| Coaching triggers | ~30 | ~36 |
| Starter prompts | ~20 | ~26 |

---

## Install / Update

```bash
# Claude Code / OpenClaw
clawhub install product-manager-skills

# Codex / Cursor / Windsurf
npx skills add Digidai/product-manager-skills
```

Full changelog: [CHANGELOG.md](../CHANGELOG.md)

---

Built by [Gene Dai](https://genedai.me/). Feedback: [GitHub Issues](https://github.com/Digidai/product-manager-skills/issues).
