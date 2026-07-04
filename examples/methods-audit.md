# Methods Audit Example

## User Prompt

```text
Use $paper-mentor in Methods Audit mode.

Main claim: our model gives better formative feedback with lower latency
Method: small transformer model fine-tuned on short-answer feedback
Dataset or data source: 18k student answers from two courses
Current baselines: rule-based feedback, larger LLM, previous classifier
Metrics: accuracy, latency, teacher preference
Ablations: none yet
Results summary: better latency than LLM, similar teacher preference, slightly lower accuracy
```

## Expected Response Shape

```text
Main claim:
Better formative feedback with lower latency.

Evidence fit:
Partially supported. Latency is supported, but "better feedback" needs careful definition because accuracy is lower.

Claim-to-evidence matrix:
- Claim: lower latency
  Evidence: latency comparison with larger LLM
  Missing: hardware and batch setting
  Recommended test: standardized latency benchmark
  Severity: Major

- Claim: better formative feedback
  Evidence: teacher preference
  Missing: rubric, inter-rater agreement, student learning proxy
  Recommended test: preference protocol and agreement report
  Severity: Blocking

Baselines:
The larger LLM and rule-based baseline are useful, but the prior classifier must be described as a fair closest baseline.

Ablations:
Add at least data size, model size, and feedback component ablations.

Next three actions:
1. Narrow "better feedback" to the measured construct.
2. Report annotation and preference reliability.
3. Add ablations tied to the lightweight claim.
```
