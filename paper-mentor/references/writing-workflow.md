# Writing Workflow

Use this reference when the user asks for help drafting, restructuring, or improving sections.

## Section Jobs

Abstract:

- State problem, gap, approach, key evidence, and contribution.
- Avoid unexplained jargon and unsupported broad claims.

Introduction:

- Establish importance.
- Define the gap.
- Explain why the gap is hard or unresolved.
- State the contribution.
- Preview evidence.

Related Work:

- Organize by concept, method, dataset, debate, or limitation.
- Compare against the user's contribution.
- Avoid paper-by-paper summaries unless chronology is essential.

Method:

- Explain what was done, why it is appropriate, and what assumptions it relies on.
- Include enough detail for informed evaluation or reproduction.

Experiments or Evaluation:

- Match experiments to claims.
- Include baselines, metrics, ablations, and limitations.
- Explain negative or mixed results honestly.

Discussion:

- Interpret findings.
- State limits.
- Explain implications without overselling.

## Revision Workflow

1. Identify the section's job.
2. Extract the main claim of each paragraph.
3. Check whether claims appear in a logical order.
4. Flag missing evidence, missing transitions, and unsupported scope.
5. Suggest a revised outline before rewriting prose.
6. Rewrite only after the structure is clear.

## Paragraph Test

For each paragraph, identify:

- role in the section
- topic sentence
- evidence or reasoning
- link to the paper's contribution
- transition to the next paragraph

## Output Preference

When improving a section, prefer:

- diagnosis first
- revised outline second
- paragraph-level edits third
- candidate text only when useful

For candidate text, state assumptions and ask the user to verify field-specific claims, citations, and results.
