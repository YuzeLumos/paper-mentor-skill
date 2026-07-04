# Rebuttal Example

## User Prompt

```text
Use $paper-mentor to help me respond to this reviewer comment.

Reviewer comment:
The paper claims better generalization, but the experiments only evaluate one dataset.

Available evidence:
We have one main dataset and one smaller held-out dataset. We can add a limitation paragraph and report a small transfer experiment.
```

## Expected Response Shape

```text
Reviewer concern:
The reviewer is challenging whether the generalization claim is supported by evidence.

Underlying issue:
The current claim is broader than the experimental design.

Response strategy:
Narrow the claim, add the held-out experiment if valid, and revise the manuscript to state the limitation clearly.

Manuscript change needed:
- revise the claim from broad generalization to evidence-backed robustness in the tested setting
- add the held-out dataset result
- add a limitation about dataset scope

Draft response:
We thank the reviewer for pointing out that our original wording could overstate the scope of the evidence. In the revised manuscript, we have narrowed the generalization claim and added results on a held-out dataset. We also added a limitation paragraph clarifying that broader cross-domain generalization remains future work.

Risk if ignored:
The rebuttal may look defensive and the paper may appear to overclaim beyond its evidence.
```
