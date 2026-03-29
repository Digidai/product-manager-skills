# TODOS

## Coaching Protocol

### Role Switching System
**Priority:** P2
**What:** Add role switching (mentor/challenger/ceo/user_voice/eng_lead) to coaching mode
**Why:** Strongest differentiation feature. Makes coaching feel like multiple experts, not one mentor.
**Cons:** Relies on model self-discipline in pure Markdown. Cross-platform fidelity not guaranteed.
**Depends on:** v0.4 coaching rules validated as working cross-platform
**Context:** Codex outside voice flagged that pure-Markdown role switching is aspirational. Validate v0.4 interaction rules first, then add role switching if the base coaching protocol proves reliable.

### Default Coaching Behavior Decision
**Priority:** P1
**What:** Decide if v0.5 default should be coaching (always push back) with "quick mode" for fast output, instead of current standard-first approach
**Why:** Current README promises "push back / strong PM peer" but coaching is opt-in, hiding the differentiation. Codex flagged this contradiction.
**Depends on:** v0.4 user feedback. Do users actively use "coach me" prompts, or do they prefer fast output?
**Context:** This is a design decision, not engineering work. Collect feedback from v0.4 users before deciding.

### Scenario Triggers Experiment
**Priority:** P3
**What:** Design a safe "proactive PM suggestion" mechanism for when AI detects PM-relevant patterns during code work
**Why:** Shifts product form from request-response to ambient coaching. High potential, high risk of annoyance.
**Cons:** Markdown can't do real event monitoring. Risk of being disruptive.
**Depends on:** v0.4 coaching validation + default behavior decision
**Context:** Codex flagged this as a product form shift, not a content extension. Needs careful design including frequency limits and opt-out.

## Completed
