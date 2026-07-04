# Paper Health Check Example

## User Prompt

```text
Use $paper-mentor in Paper Health Check mode.

Field: AI for education
Target venue or reader: applied AI conference
Artifact type: abstract
Claimed contribution: a lightweight feedback model for short student answers
My biggest concern: novelty and experimental strength

Text:
[paste abstract here]
```

## Expected Response Shape

```text
One-line diagnosis:
The idea is potentially useful, but the contribution must be narrowed and tied to evidence that the model is both lightweight and pedagogically useful.

Traffic light:
Yellow

Scorecard:
- Problem importance: 4/5
- Gap clarity: 2/5
- Contribution specificity: 2/5
- Evidence fit: 2/5
- Method validity: unknown
- Positioning: 2/5
- Writing structure: 3/5
- Scope control: 3/5

Blocking risks:
- "Lightweight" is not operationally defined.
- The closest prior feedback systems are not named.
- The evaluation does not yet show why the model is educationally useful.

Next three actions:
1. Define lightweight in measurable terms.
2. Name the closest prior systems and the exact difference.
3. Build a claim-to-evidence matrix for accuracy, latency, and feedback quality.

Better prompts to ask next:
- Use $paper-mentor in Contribution Mapper mode...
- Use $paper-mentor in Methods Audit mode...
```
