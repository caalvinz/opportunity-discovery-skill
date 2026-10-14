# Opportunity Discovery Skill

**Evidence-driven commercial judgment for end-to-end system builders.**

An open Agent Skill for evaluating whether an idea, product opportunity, AI workflow, or internal transformation is *worth doing* before investing in specification and engineering.

**Version:** 0.2.0 · **License:** MIT · **Status:** experimental

## Two complementary reasoning engines

- **Generative Reasoning:** challenge solution-first framing, find overlooked actors, problems, opportunities, and alternatives.
- **Critical Convergence:** test competing explanations, distinguish evidence from assumptions, detect diminishing information gain, and move to real-world validation.

Rather than asking endless questions, the skill adaptively chooses **Generate → Probe → Challenge → Synthesize → Validate → Decide**, including an **Opportunity Checkpoint** when appropriate.

## Install

Use an Agent Skills-compatible host. For Codex Desktop with a user-level Skills directory:

```bash
git clone https://github.com/caalvinz/opportunity-discovery-skill.git
mkdir -p ~/.agents/skills/opportunity-discovery
cp -R opportunity-discovery-skill/SKILL.md opportunity-discovery-skill/references opportunity-discovery-skill/assets ~/.agents/skills/opportunity-discovery/
```

Restart or refresh your agent and verify it discovers `opportunity-discovery`. Actual Skills discovery locations may depend on your Codex version. Installing the GitHub repository does not install a ChatGPT Plugin.

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
