# Opportunity Discovery Skill

**Evidence-driven commercial judgment for end-to-end system builders.**

An open Agent Skill for evaluating whether an idea, product opportunity, AI workflow, or internal transformation is *worth doing* before investing in specification and engineering.

**Version:** 0.2.0 · **License:** MIT · **Status:** experimental

## Two complementary reasoning engines

- **Generative Reasoning:** challenge solution-first framing, find overlooked actors, problems, opportunities, and alternatives.
- **Critical Convergence:** test competing explanations, distinguish evidence from assumptions, detect diminishing information gain, and move to real-world validation.

Rather than asking endless questions, the skill adaptively chooses **Generate → Probe → Challenge → Synthesize → Validate → Decide**, including an **Opportunity Checkpoint** when appropriate.

## Installation

### Quick install (recommended)

Using the [Skills CLI](https://github.com/vercel-labs/skills):

```bash
npx skills@latest add caalvinz/opportunity-discovery-skill
```

When prompted, select **Codex** as the target agent and **Global** as the installation scope to make the skill available across projects. You can also inspect supported options with `npx skills@latest add --help`. This command uses the third-party Skills CLI; it does **not** require the standalone `codex` executable.

### Manual install

For Codex Desktop installations that discover user-level skills from `~/.agents/skills/`:

```bash
git clone https://github.com/caalvinz/opportunity-discovery-skill.git
mkdir -p ~/.agents/skills/opportunity-discovery
cp -R opportunity-discovery-skill/SKILL.md opportunity-discovery-skill/references opportunity-discovery-skill/assets ~/.agents/skills/opportunity-discovery/
```

If your Codex version uses a different Skills directory, follow its configured path instead.

### Verify installation

Restart or refresh Codex Desktop. In a new conversation, ask:

> Use the opportunity-discovery skill in Explore mode to challenge a new product idea. First confirm you can find the skill.

### Update

For a Skills CLI installation, use the CLI's update workflow if supported by your installed version (check `npx skills@latest --help`).

For manual installations, pull the latest repository changes and copy the updated `SKILL.md`, `references/`, and `assets/` into your existing skill directory.

Installing this repository does not install a ChatGPT Plugin.

## Try it

> Use opportunity-discovery in Explore mode. I have an idea for an HR conversation-preparation partner. Challenge the underlying problem rather than designing features.

> Give me an Opportunity Checkpoint: what changed, what remains assumed, the strongest competing hypothesis, and what real-world evidence would change our decision?

> Switch to Critical Convergence and propose the cheapest discriminating experiment. Do not start coding.

## Modes

| Mode | Outcome |
| --- | --- |
| Explore | Discover and reframe opportunities through conversation |
| Assess | Inspect value, adoption, alternatives, feasibility, economics and strategic fit |
| Validate | Plan falsifiable experiments with explicit decision consequences |
| Decide | Recommend Pursue, Experiment, Park or Reject, with evidence and counterarguments |

## Files

- [SKILL.md](SKILL.md) — operating contract, routing, checkpoint behavior, SDLC handoff.
- [references/](references/) — methods for adaptive reasoning, evidence, commercial judgment and an illustrative HRP case.
- [assets/](assets/) — templates for checkpoint, evidence ledger, opportunity assessment, experiment brief, decision record and downstream problem brief.
- [CHANGELOG.md](CHANGELOG.md) — version history.

## Boundaries

The skill **does not** establish market demand from a convincing conversation, turn every idea into an AI agent, substitute for HR/legal/professional judgment, or automatically generate a PRD. The human owns investment decisions. The skill is currently a design/prototype; real-world quality is not yet benchmarked.

## Origin and acknowledgements

Inspired by iterative questioning and evidence-driven, human-governed product and engineering workflows. This is an independent skill, not affiliated with Matt Pocock or OpenAI.

MIT licensed. See [LICENSE](LICENSE).
