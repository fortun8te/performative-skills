# Performative Skills

Three compact agent skills for better creative reviews and better product decisions.

## Critic

Five relevant perspectives: four main voices and one wildcard. The cast favors Jony Ive, Jonathan Anderson and Rick Rubin when useful, with Theo Von as a frequent wildcard. James Baldwin adds a lens on truth, language and human particularity. All 33 perspectives remain selectable.

Only selected voice cards load. Reviews default to 180–260 words: verdict, five distinct observations, what to keep, and up to three concrete next steps. Real tradeoffs matter; numerical scores, forced fights and invented user reactions do not.

These are editorial interpretations inspired by public work, not authentic statements or endorsements. Source anchors and limitations are included in the cards. Some cards have primary-source links; others name the work that grounds the lens. They are not biographies or a claim that every attribution has been independently verified.

Examples:

- `critic: review this ad for its intended audience`
- `critic cast: Jony Ive, Jonathan Anderson, Rick Rubin, James Baldwin, Theo Von`
- `critic rick: I keep polishing this and can't decide what to remove`

The old standalone [Rick skill](https://github.com/fortun8te/rick) is superseded by Critic's mirror mode.

## Next Feature

Recommend a concrete capability grounded in the actual product, not an abstract roadmap slogan. Default: one feature, a before/after example, why it matters, two or three build steps and an observable completion check, in 180 words or fewer. Explicit requests for more ideas or detail take precedence.

Evidence lookup starts small. Existing workarounds and infrequent tasks can justify a feature. No invented usage data, arbitrary improvement multiplier or blanket ban on exports, notifications or accessibility work.

Examples:

- `next-feature: what is the next useful capability for this app?`
- `next-feature: compare these four proposals and recommend one`
- `next-feature: give me five distinct ideas, then a short plan for the best`

## Nichemaxx

Find the precise reference you would not quite have reached alone. Start from the current piece or feeling, connect it to a specific work, and explain the useful detail. Default: one strong pull in 60–140 words; up to three under 180 words when comparison helps.

No fixed aesthetic, mandatory obscurity or “always slow cuts” formula. Saved items are clues, not identity or vetoes. Verify the detail that supports the recommendation, not just the title. Listening and reading recommendations can be for enjoyment, without a forced production exercise.

Examples:

- `nichemaxx: one photographic reference for bright sunlight that feels slightly artificial`
- `nichemaxx: this track is close, but I want something less obvious with the same tension`
- `nichemaxx: keep my concept, find one adjacent reference that could loosen it up`

Personal archives are optional and stay local. When context is needed, the skill can read a private index at `~/.config/performative-skills/context.md` (or under `$XDG_CONFIG_HOME`). No personal archive or profile is included in this repository.

## Install

Copy any of `skills/critic`, `skills/next-feature` and `skills/nichemaxx` into the skill directory your agent reads, such as `~/.codex/skills/` or `~/.claude/skills/`. Include each folder's supporting files. Use the agent's skill selector or name the skill in your prompt; slash-command behavior depends on the agent.

Replace an existing copy rather than installing a second named variant. The skills have no runtime dependencies or required subagents. Mirror mode loads only its short guide; panel mode loads the cast index and selected cards.

## Why three skills?

Nichemaxx discovers and connects. Critic evaluates existing work. Next Feature proposes usable product capabilities. They can work together without turning every request into a three-stage process.

## Validation and scope

Skill metadata and local reference links are checked. See [evaluation cases](tests/scenarios.md) for behavioral checks and limitations. Word-count reductions measure instruction size, not benchmarked model token use or proven output quality.

MIT licensed. No client files, private research, credentials or local conversation history are included.
