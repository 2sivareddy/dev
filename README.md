# dev

Personal workspace for reusable AI engineering instructions and evaluation artifacts, by 2sivareddy. This repository is the version-controlled archive. The runtime copies live in a private Google Drive skills folder.

## Contents

| File | Purpose | Status |
|---|---|---|
| AI_ENGINEER_SKILL.md | Adoption path for operating instructions: pre-adoption fixes, baseline comparison, decision-confidence estimator (Wilson intervals, alarm rule), per-session cost rules. | Proposed |
| AI_ENGINEER_JUDGE_SKILL.md | Honest judge protocol: role labels, evidence-based verdicts with severity, coverage statements, honesty rules, bias controls, calibration, feedback loop. | Proposed |
| v03_baseline_eval_kit.md | 8-task kit comparing a candidate instruction set (Arm B) against default behavior (Arm A) in fresh sessions. Acceptance criteria are set before running. | Proposed, not yet run |
| generate_v03_baseline_eval_kit.py | Standalone script that regenerates the kit file deterministically. | Implemented, not independently tested |

## Status model

Every artifact reports its status: proposed, approved, implemented, tested, deployed, verified. No completion is claimed without evidence.

## Usage

- Regenerate the kit: `python generate_v03_baseline_eval_kit.py`
- Run the baseline comparison per the kit protocol before adopting any instruction set.
- Keep this repository and the Google Drive skills folder in sync on material changes.

A change is material if it can alter a pass or fail on any existing evaluation case.

## Notes

- This repository is public.
- The skills remain status Proposed until the baseline evaluation runs and passes its acceptance criteria.
