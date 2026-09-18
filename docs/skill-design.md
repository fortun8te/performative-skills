# Skill design choices

Inspired by [Matt Pocock's writing-for-agents](https://github.com/mattpocock/skills/blob/c55ee46073ed923f86ce59a5eb3b6d895095d1b7/skills/productivity/writing-for-agents/SKILL.md): keep universal behavior in a small core, load specialist depth only when a clear condition applies, define observable completion, and keep each rule in one place.

His [code-review skill](https://github.com/mattpocock/skills/blob/c55ee46073ed923f86ce59a5eb3b6d895095d1b7/skills/engineering/code-review/SKILL.md) distinguishes explicit requirements from heuristic judgments. Here, a user's current brief takes priority over a critic's aesthetic or a historical taste interpretation. His [research skill](https://github.com/mattpocock/skills/blob/c55ee46073ed923f86ce59a5eb3b6d895095d1b7/skills/engineering/research/SKILL.md) favors tracing facts to primary sources.

These are structural lessons, not copied workflows. We do not adopt exhaustive grilling or long specification output. Each skill has its own short response contract, with requested detail taking precedence.

- Critic: cast selection precedes loading. Five relevant perspectives, one wildcard by default. Source-grounded interpretive lenses, not celebrity impersonation.
- Next Feature: bounded product inspection, explicit user capability, actionable minimal plan and observable completion.
- Nichemaxx: a precise relationship in the request, selective evidence, verified reference detail and a useful connection. Novelty is not a quota and private taste is not a public dataset.

Personalization can amplify bad assumptions. Machine labels are useful candidate filters; they cannot establish why someone saved an item, their identity, or what they will never like. Prefer current explicit feedback and item-level evidence, with original speaker and context preserved.

Smaller instructions can reduce reading cost, but are not proof of better judgment. Evaluate actual outputs for usefulness, factual support, distinctness, audience fit and brevity. Keep the core small; add rules only for demonstrated failures.
