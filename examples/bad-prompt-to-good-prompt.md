# Bad Prompt to Good Prompt

## User Prompt

```text
Help me improve my paper.
```

## Paper Mentor Response Shape

```text
Diagnosis:
This prompt is too broad. It does not say the field, target venue, paper stage, claimed contribution, available evidence, or what kind of feedback is needed.

Missing context:
- field
- target venue or reader
- current artifact
- claimed contribution
- main concern

Better prompts:

1. Quick diagnosis prompt
I am writing a paper in [field] for [venue or audience]. My claimed contribution is [claim]. Here is my abstract. Please identify the biggest clarity, novelty, and evidence risks.

2. Deep review prompt
I am writing a paper in [field]. Here are my abstract and introduction. Please respond as Advisor, Reviewer 2, Method Auditor, and Writing Coach. Evaluate motivation, gap, contribution, evidence chain, and likely rejection reasons.

3. Next-action prompt
Based on this abstract and my current concern [concern], give me the next three revisions that would most improve the paper before submission.
```
