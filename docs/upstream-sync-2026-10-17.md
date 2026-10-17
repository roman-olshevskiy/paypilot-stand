# Upstream sync — 2026-10-17

Source: TarasFedorenkoFTV/paypilot-stand main, 4edc984 (3 new commits).
Target: roman-olshevskiy/paypilot-stand main, via PR only.

Changes: comparison cards expose run-condition / answer differences; an optional lightweight-model explanation is available; EXPLAIN_MODEL reaches Docker; OpenAI response parsing and API tests are updated.

Impact on completed labs:
- No changes to seed, profiles, base prompt, overlays or app/engines. Submitted L01 captures, proposed requirements and oracle numbers remain historical evidence.
- The new explain endpoint adds model usage when invoked. It is not an independent oracle or a replacement for trace analysis. Existing billing totals must not be recalculated as if explanation calls occurred in those runs.
- This is the original single-stand lineage, not paypilot-stand-shared. Future labs use shared; this PR keeps the earlier fork current without replacing it.
- No live model runs, Docker deployment or submitted-evidence edits are required for this merge.

Validation results are recorded in the PR.
