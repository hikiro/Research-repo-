# Animation Intelligence & Production Research

A versioned, searchable knowledge base for animation research, character acting, visual storytelling, rigging adaptation, production methods, and quality assurance for **The Curiosity Archive** and related animation work.

This repository is the research and decision record. It is separate from the executable animation-engine repository:

- Production code: the local `stopmo-studio` source repository (its remote URL has not yet been verified).
- Research and reusable knowledge: this repository.

## Working principles

1. **Recover before rebuilding.** Inspect existing research, decisions, assets, and working implementations before proposing replacements.
2. **Evidence before rules.** Record source links, publication details, observations, tests, and limitations. Do not present hypotheses as established facts.
3. **Context matters.** Animation, acting, rigging, timing, and staging rules must state the character, action, environment, shot, scale, and intended effect to which they apply.
4. **Reusable, not universal by default.** A useful pattern is a candidate rule until its scope and exceptions are understood.
5. **Record failures as well as successes.** Preserve root causes, failed attempts, fixes, and measurable quality checks.
6. **Keep research connected to production.** Each transferable finding should explain how it can inform a rig, animation, shot, tool, or QA test.

## Evidence labels

- **VERIFIED** — directly demonstrated by a reproducible test or inspected project artifact.
- **SOURCE-SUPPORTED** — supported by a traceable, credible external source.
- **OBSERVED** — directly seen in supplied footage, frames, images, or project output; interpretation may still be uncertain.
- **HYPOTHESIS** — plausible explanation or proposed rule that needs validation.
- **PENDING** — not yet investigated or not enough evidence to decide.

## Repository map

- [INDEX.md](INDEX.md) — navigation and current research status.
- [RESEARCH_DOMAINS.md](RESEARCH_DOMAINS.md) — approved research domains and scope.
- [LEARNING_LOG.md](LEARNING_LOG.md) — chronological decisions, findings, failures, and fixes.
- [RULEBOOK.md](RULEBOOK.md) — evidence-aware principles and production rules.
- [DO_AND_DONT.md](DO_AND_DONT.md) — practical working guidance and anti-patterns.
- [ACTIVE_ENGINEERING_STATUS.md](ACTIVE_ENGINEERING_STATUS.md) — snapshot of the linked production-engine investigation.
- [templates/RESEARCH_ENTRY_TEMPLATE.md](templates/RESEARCH_ENTRY_TEMPLATE.md) — template for new research.
- [templates/SCENARIO_PRESET_TEMPLATE.md](templates/SCENARIO_PRESET_TEMPLATE.md) — template for context-specific animation and rigging presets.

## Update policy

Update the relevant index and learning log whenever a meaningful decision, source-backed finding, production test, defect, or rule changes. Include dates, exact references, evidence labels, scope, and unresolved questions. Do not silently replace an older conclusion: record what changed and why.
