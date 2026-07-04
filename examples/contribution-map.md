# Contribution Mapper Example

## User Prompt

```text
Use $paper-mentor in Contribution Mapper mode.

Field: natural language processing
Target venue or reader: NLP conference
Problem: long-document summarization evaluation is inconsistent
Gap: current metrics miss factual consistency and section-level coverage
My proposed contribution: a rubric-based evaluation framework with automatic checks
Closest prior work I know: ROUGE, BERTScore, factuality metrics
Evidence I have or can collect: human annotation study and correlation analysis
```

## Expected Response Shape

```text
Current contribution:
A rubric-based evaluation framework for long-document summarization.

Missing or weak element:
The closest prior work is named too broadly. The paper needs a sharper comparison against existing factuality and coverage evaluation methods.

Contribution map:
- Audience: NLP researchers evaluating long-document summarization
- Problem: existing evaluation misses multiple quality dimensions
- Gap: factual consistency and section-level coverage are not jointly assessed
- Closest prior work: user should identify specific factuality and coverage metrics
- Difference: combines rubric dimensions with automatic checks
- Evidence: human annotation and correlation analysis
- Limitation: may depend on annotation quality and domain
- One-sentence contribution: This paper proposes and validates a rubric-based framework for evaluating factual consistency and section-level coverage in long-document summarization.

Reviewer attack points:
- Is this a new metric or just a checklist?
- Does it correlate with human judgment better than existing methods?
- Is it reliable across domains?

Revision moves:
1. Define the closest metric-level baselines.
2. State whether the contribution is framework, benchmark, metric, or analysis.
3. Tie each rubric dimension to validation evidence.
```
