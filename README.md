# Paper Mentor Skill

Turn vague paper questions into advisor-grade AI conversations.

`paper-mentor` is a Codex skill for students and researchers who want practical guidance from idea to submission: prompt coaching, paper health checks, contribution mapping, literature review structure, methods audits, reviewer simulation, and rebuttal planning.

It does not try to replace the student or fabricate a better-looking paper. It helps the student ask sharper questions, see risks earlier, and revise with a plan.

## Try This First

Copy this into a new Codex chat after installing the skill:

```text
Use $paper-mentor in Paper Health Check mode.

Field:
Target venue or reader:
Artifact: abstract / introduction / idea / full draft
Claimed contribution:
My biggest concern:

Text:
[paste your text here]
```

You will get a compact diagnosis, risk scorecard, blocking issues, next three actions, and better prompts to ask next.

## Why People Star This

- It gives students a reusable way to talk to AI about papers.
- It turns weak prompts like "help me improve my paper" into useful research prompts.
- It simulates an advisor group instead of producing generic writing advice.
- It separates writing polish from scientific validity.
- It includes copy-paste prompts for real academic workflows.
- It keeps academic integrity explicit: no fake citations, no invented results, no hidden limitations.

## Modes

| Mode | Use it for |
| --- | --- |
| Prompt Clinic | Turn a vague research question into strong AI prompts |
| Paper Health Check | Quickly diagnose an idea, abstract, intro, or draft |
| Contribution Mapper | Clarify gap, claim, novelty, evidence, and audience fit |
| Section Surgeon | Improve abstract, introduction, related work, method, or discussion |
| Literature Map | Organize scattered papers into a useful Related Work structure |
| Methods Audit | Check whether experiments and metrics support the claims |
| Reviewer Simulation | Produce a skeptical pre-submission review |
| Rebuttal Planner | Respond to reviewer comments with evidence and restraint |

## Copy-Paste Prompts

See [PROMPTS.md](PROMPTS.md) for a ready-to-use prompt pack.

Popular starters:

```text
Use $paper-mentor in Prompt Clinic mode.
Rewrite this vague question into three better AI prompts:
"Help me improve my related work."
```

```text
Use $paper-mentor in Reviewer Simulation mode.
Target venue:
Claimed contribution:
Here are my abstract and introduction:
[text]
```

```text
Use $paper-mentor in Rebuttal Planner mode.
Reviewer comment:
[comment]
Actual evidence I have:
[evidence]
Manuscript changes I can make:
[changes]
```

## Install

Clone this repository, then copy the `paper-mentor` folder into your Codex skills directory.

Windows PowerShell:

```powershell
git clone https://github.com/YuzeLumos/paper-mentor-skill.git
New-Item -ItemType Directory -Force "$env:USERPROFILE\.codex\skills"
Copy-Item -Recurse -Force ".\paper-mentor-skill\paper-mentor" "$env:USERPROFILE\.codex\skills\"
```

macOS or Linux:

```bash
git clone https://github.com/YuzeLumos/paper-mentor-skill.git
mkdir -p ~/.codex/skills
cp -r paper-mentor-skill/paper-mentor ~/.codex/skills/
```

## Temporary Trial

The skill is configured for manual invocation by default:

```yaml
policy:
  allow_implicit_invocation: false
```

That means it should only run when you explicitly use `$paper-mentor`.

To remove it after testing:

Windows PowerShell:

```powershell
Remove-Item -Recurse -Force "$env:USERPROFILE\.codex\skills\paper-mentor"
```

macOS or Linux:

```bash
rm -rf ~/.codex/skills/paper-mentor
```

## Example

Weak prompt:

```text
Help me improve my paper.
```

Better prompt:

```text
I am writing a paper in [field] for [venue or reader]. My claimed contribution is [claim]. Below is my abstract and introduction. Please evaluate whether the motivation, gap, contribution, and evidence chain are clear. Give feedback as Advisor, Reviewer 2, Method Auditor, and Writing Coach. End with the top three revision actions and better prompts I should ask next.
```

## What It Is Not

This is not a paper generator, citation faker, acceptance predictor, or shortcut around academic responsibility. It is a structured mentor workflow for critique, planning, revision, and better AI conversations.

## Repository Structure

```text
paper-mentor-skill/
  PROMPTS.md
  README.md
  README.zh-CN.md
  paper-mentor/
    SKILL.md
    agents/openai.yaml
    references/
      contribution-map.md
      experiment-audit.md
      literature-map.md
      paper-health-check.md
      prompt-coach.md
      rebuttal-guide.md
      review-rubric.md
      writing-workflow.md
  examples/
    ...
```

## Publish Your Own Version

Create an empty GitHub repository named `paper-mentor-skill`, then run:

```bash
git init
git add .
git commit -m "Initial paper mentor skill"
git branch -M main
git remote add origin https://github.com/YOUR_NAME/paper-mentor-skill.git
git push -u origin main
```

## License

MIT
