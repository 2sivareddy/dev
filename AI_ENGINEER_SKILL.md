# Instruction Adoption Path — SKILL.md
Version: 0.1
Date: 2026-11-14
Status: Proposed

## Purpose
Adopt, revise, or reject an operating instruction version through evidence. Do not adopt by assertion. Do not claim adoption without a run record.

## When to apply
Apply this skill when a new or revised operating instruction, skill, or standing prompt is proposed for adoption.

## Pre-adoption fixes
1. Remove or define unmeasured numbers. A target without an estimator is a claim, not a criterion.
2. Define gating terms. Write a test that a script or a second reviewer could apply. Give one passing and one failing example. If no test can be written, mark the term as a judgment term. Do not present it as mechanical.
3. Materiality rule: a change is material if it can alter a pass or fail on any existing evaluation case. Dry-run the change against the stable regression suite. Version material changes. Record immaterial changes in the changelog only.

## Baseline comparison
1. Define 5 to 10 representative tasks. Each task must name the instruction section it stresses, and state pass and fail criteria.
2. Set acceptance criteria before running. Do not move them after seeing results.
3. Run each task in fresh isolated sessions. Arm A uses the current instructions. Arm B uses the candidate version. One task per session. Do not reuse a conversation.
4. Grade with the criterion list, not with an overall impression.
5. Decide: adopt, revise, or defer. A miss on a disqualifying criterion blocks adoption.

## Decision confidence
1. Register each decision before execution. Record the decision class, the choice made, and one falsifiable predicted-outcome sentence.
2. After the observation window, mark the outcome: matched, not matched, or unresolved.
3. Compute p-hat = matched / (matched + not matched). Report the Wilson 95 percent interval and n with every number.
4. Report unresolved outcomes separately. Report by decision class. Do not average across classes with different stakes.
5. Alarm rule: at n >= 40 per class, alarm when the Wilson lower bound falls below 0.70.
6. Treat the 80-85 percent target as a trend, not a gate. Separating 80 from 85 percent statistically needs about 900 decisions per class. Do not plan for that. Plan for the alarm rule.

## Per-session cost
1. Split long instruction sets. Keep a short core that is always loaded. Keep deep modules that load only when their work is in scope.
2. Count total delivery cost, not token price alone. The instruction file itself is part of the cost.
3. Prefer the simplest qualified execution path.

## On adoption
1. Version the approved document. Keep prior versions and results.
2. Store the approved version where it loads automatically: custom instructions, or this skills folder referenced by name.
3. A file in a folder does not enforce or auto-load itself. Verify loading before claiming the instruction is active.

## Related artifacts
- v03_baseline_eval_kit.md: worked example of the baseline comparison design.