# Experiment Audit

Use this reference when the user asks whether methods, experiments, baselines, metrics, datasets, analyses, or ablations support the paper's claims.

## Claim-to-Evidence Matrix

For each claim, map:

```text
Claim:
Evidence currently provided:
Missing evidence:
Best test:
Required baseline or comparison:
Metric:
Risk if unsupported:
```

## Audit Questions

- Does each major claim have direct evidence?
- Are baselines strong, current, and fair?
- Are metrics aligned with the real objective?
- Are ablations tied to mechanism rather than decoration?
- Are datasets, splits, and preprocessing described clearly?
- Are negative or mixed results handled honestly?
- Are limitations named without destroying the contribution?

## Severity

- Blocking: central claim not supported, unfair comparison, invalid metric, unreproducible setup
- Major: important missing baseline, weak ablation, unclear dataset, insufficient analysis
- Minor: reporting clarity, table organization, local explanation

## Output Template

```text
Main claim:
Evidence fit:

Claim-to-evidence matrix:
- Claim:
  Evidence:
  Missing:
  Recommended test:
  Severity:

Baselines:
Metrics:
Ablations:
Reproducibility:
Limitations:
Next three actions:
Better prompts to ask next:
```
