# Prompt Coach

Use this reference when the user gives a vague research question, wants to use AI better, or asks for a reusable prompt.

## Goal

Move the user from "ask AI to do the work" to "ask AI to diagnose, compare, pressure-test, and plan the next step."

## Prompt Quality Test

A strong research prompt usually names:

- field and target reader
- artifact being discussed
- current stage
- claimed contribution
- available evidence
- main worry
- requested critique lens
- desired output format

## Rewrite Workflow

1. Diagnose the weakness in the original question.
2. List missing information.
3. Rewrite the prompt into three versions:
   - Fast Check: quick diagnosis
   - Deep Review: multi-lens critique
   - Next Move: concrete action plan
4. Explain when to use each version.
5. Give one follow-up question the user should answer before asking AI again.

## Prompt Formulas

Paper idea:

```text
I am exploring a paper idea in [field] for [reader or venue]. The problem is [problem], the gap is [gap], and my possible contribution is [contribution]. Please evaluate whether this is a researchable claim, what evidence would be needed, and what a skeptical reviewer would attack first.
```

Introduction:

```text
I am writing the introduction for a paper in [field]. My target reader is [reader]. My claimed contribution is [claim]. Here is my current introduction: [text]. Please evaluate motivation, gap, contribution, evidence preview, and paragraph order. Give a revised outline before rewriting any prose.
```

Related work:

```text
I am writing Related Work for a paper about [topic]. My paper differs from prior work by [difference]. Here are the papers or categories I currently have: [list]. Please organize them into conceptual clusters, identify missing comparison dimensions, and show how the section should support my contribution.
```

Methods and experiments:

```text
My paper claims [claim]. My method is [method]. My current experiments are [experiments]. Please create a claim-to-evidence matrix, identify missing baselines or ablations, and separate blocking validity issues from nice-to-have improvements.
```

Rebuttal:

```text
I received this reviewer comment: [comment]. My actual evidence is [evidence], and I can revise the manuscript by [possible changes]. Please identify the underlying concern, propose a respectful response strategy, list manuscript changes needed, and draft a concise response that does not overclaim.
```

## Output Template

```text
Diagnosis:
Missing context:
Better prompts:
1. Fast Check:
2. Deep Review:
3. Next Move:
When to use each:
One question to answer next:
```
