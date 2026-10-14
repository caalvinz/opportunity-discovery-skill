# Adaptive Reasoning: choosing the next best action

Do a **silent reasoning audit** after each meaningful user contribution. Never expose hidden chain-of-thought; communicate conclusions, evidence, and rationale concisely.

## State dimensions
Track whether new information materially changes: actor, triggering job, pain, alternative, benefit, buyer/channel, solution necessity, risks, economics, timing. If none changes, recognize diminishing returns.

## Action selection

| Signal | Action | Typical response |
|---|---|---|
| Single proposed solution with uncertain underlying job | Generate | Show 2–3 distinct problem interpretations |
| Concrete recent episode is missing | Probe | Ask for one specific event |
| New framing accepted too readily | Challenge | Introduce a plausible rival explanation |
| Material shift in audience/value/channel | Synthesize | Explain what changed and what is still conjecture |
| Same assumptions restated across turns | Synthesize → Validate | Checkpoint then propose a real-world test |
| Willingness-to-use/pay, actual frequency, retention impact unknown | Validate | Design behavioral evidence collection |
| Evidence adequate for small reversible commitment | Decide | Recommend gate outcome with caveats |

## Information-gain discipline
Prefer questions whose answers **change the decision or next experiment**. If the answer would only embellish a story, stop probing. Do not invent an information-gain score. Be alert to confirmation loops: a user's preference is not independent corroboration.

## Checkpoint trigger policy
Use semantic signals, not "every N turns". Material reframing, repeated questioning, unchallenged assumptions, evidence boundary, user request. After checkpoint, offer a *specific* next step rather than automatically starting another question chain.

## Two contrasting moves
**Generate:** “Perhaps the pain is not preparing a conversation but uncertainty about authority, policy, or trust; how would these differ?”
**Converge:** “We have clarified the intended experience, but still lack evidence that HR members will spend 15 minutes using it before a real conversation. Next test should observe that behavior.”

## Avoid premature closure
Do not convert an insightful concept into a PRD unless the user requests it and the gate is appropriate. Keep **problem clarity**, **user validation**, and **business validation** distinct.
