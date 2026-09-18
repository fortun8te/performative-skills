---
name: next-feature
description: Recommend concrete product features and short implementation plans, grounded in the current product. Use for what to build next, feature ideas, or evaluating proposed features. Planning only unless the user also requests implementation.
---

# Next feature

Recommend a capability someone can actually use, with enough detail to decide whether to build it.

## Understand the request

- Follow the requested count and scope. Default to one recommendation; add at most two one-line alternatives only when they represent meaningful tradeoffs.
- For a proposed feature, evaluate and sharpen that feature. For a supplied list, compare those items; respect a request to rank all of them.
- Use the user's objective, constraints and stage of product. A prototype can justify an exploratory feature without existing customers or usage data.

## Ground the recommendation

Reuse relevant context already provided. Otherwise inspect a small amount of available evidence: the product overview, relevant UI or command flow, implementation, and issues or feedback. Start with at most five targeted reads or searches; avoid whole-repository dumps. Stop once you understand current behavior, the gap, and a plausible delivery path. Expand only to resolve a specific uncertainty that could change the recommendation, or when asked for deeper research.

Check that the capability is not already present. Code demonstrates implementation, not adoption or demand. Distinguish observed facts, user-reported needs and your hypotheses; never invent users, requests, metrics or conversion gains. Cite the one or two strongest available sources beside the reasoning.

When access or context is missing, state the limitation. Ask one focused question if it determines the product or recommendation; otherwise give a clearly provisional proposal. Research competitors only if requested or needed for the decision. Delegation is optional, not a required stage.

## Choose a real feature

Describe it as **when [situation], the user can [action], producing [visible result]**. “Improve engagement” is a goal; “save a filtered search and reopen it with the same filters” is a capability.

Prefer the strongest combination of user value, evidence, fit and delivery effort. Consider important infrequent tasks, accessibility and reliability alongside frequent workflows. An existing workaround can demonstrate friction; it is not grounds for rejection. Avoid arbitrary improvement multipliers or usage-frequency gates.

Keep the smallest useful version intact. Name its entry point, essential behavior and a meaningful failure or empty case when applicable. A roadmap theme, refactor or research task alone is not a feature; label such work honestly if it is the better next investment. Recommend validation instead of a build when the central assumption is too weak, with a concrete check.

## Deliver a short decision

Default to **220 words or fewer**. For a requested list, give each item a compact capability/example and rationale; expand the plan for the recommended item unless plans for every item were requested. Detailed requests override the default length.

- **Feature:** Plain name and one concrete before/after example.
- **Why this next:** Product-specific evidence, expected benefit and the main uncertainty or tradeoff.
- **Plan:** Two or three actionable steps tied to the actual flow or verified components. Separate verified locations from proposed ones. Avoid filler such as “build, test, deploy.”
- **Done when:** An observable user outcome, including the important edge case. Use an outcome to monitor only when it can realistically be measured; do not invent numerical targets.

Omit preamble, repeated summaries and speculative schedules. This is a recommendation and plan; modify code or create tickets only when the user requests execution.
