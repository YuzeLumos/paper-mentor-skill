# Prompt Clinic Example

## User Prompt

```text
Use $paper-mentor in Prompt Clinic mode.

Rewrite this vague research question into three better AI prompts:
"Help me fix my related work."

My field: human-computer interaction
My current stage: first full draft
What I want to decide: whether the related work supports my contribution
```

## Expected Response Shape

```text
Diagnosis:
The prompt is too broad. It does not say what the contribution is, which literature areas are included, or what "fix" means.

Missing context:
- target venue or reader
- claimed contribution
- current literature clusters
- closest competing work

Better prompts:

1. Fast Check:
I am writing Related Work for an HCI paper. My contribution is [claim]. Here are my current section headings and one-paragraph summary. Please tell me whether the section supports the contribution or reads like a paper list.

2. Deep Review:
I am writing Related Work for an HCI paper about [topic]. My contribution differs from prior work by [difference]. Here is the section. Please organize the literature into conceptual clusters, identify missing comparison dimensions, and flag where I overstate prior limitations.

3. Next Move:
Given my Related Work draft and contribution claim, list the three highest-impact revisions I should make before editing prose.

One question to answer next:
What is the closest prior work that a skeptical reviewer would compare your paper against?
```
