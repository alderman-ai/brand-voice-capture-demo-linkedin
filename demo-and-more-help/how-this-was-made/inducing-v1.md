# Version 1: inducing the rubric (2026-08-09)

*Induction* here means deriving criteria from graded examples and the
grader's notes, rather than writing them top-down. Source: the rubric's §A
and §F.

## The corpus

34 induction rows from a 45-row table, "LinkedIn Post Taste Extraction — v2":

- **14 S2-arm rows**: 7 `authored` (by the operator) and 7 `captured` (real
  posts by real named people);
- **14 `baseline` rows**: naive, zero-skill generations, added by operator
  ruling so the Unpostable tier had honest material;
- **6 `rewrite` rows**: the operator's own rewrites, promoted from his
  grading notes with his inline grades.

Of the other 11 rows: 5 held out, 3 duplicate-consistency copies, 3 left
ungraded and excluded by operator ruling.

## The test

23 candidate criteria (20 first-pass plus 3 refined in a second pass) ×
34 rows = **782 judgments**, made by fresh subagents that saw **post bodies
only**: no grades, no notes. A criterion survived only if it separated the
tiers.

**11 survived**: six disqualifiers (hard fails), four voice criteria, one
holistic gate. Disqualifiers are 6/11 = 55% against a composition target of
at least 25%.

## What got discarded, and why

- **Seven fluent, plausible, useless criteria** (SKIM-01, CLAIM-10,
  CLOSE-11, FLOW-07, REGM-09, AIR-08, STAN-18): met at near-identical rates
  across all three tiers. "Unable to separate the tiers, which is exactly what the
  validation pass exists to catch."
- **SPEC-17**: naive generations are full of *fake* specificity, so the
  criterion read slop as strong.
- **Bolding (v1's BOLD-12)**: too rare to gate. It came back in v2 as
  BOLD-25, once the rewrites supplied the evidence.
- **EPAL-13**: its Good hits were almost exactly the
  generator's fixed two-line hook template. It encoded "written by our
  generator", not taste: a provenance check firing as designed.

## Two checks worth copying

- **Fingerprint guard.** Every criterion that separated Good from Great was
  tested against third-party posts the operator graded Good. Satisfied by
  none of them → tagged `voice` (his style, not quality). This is what later
  lets the rubric grade client content without punishing it for not sounding
  like him.
- **Boundary reproduction.** The tier rules reproduce 4/4 Great rows and 7/8
  Good rows. The one miss is the post that cleared every listed criterion and
  was still only Good, which is why the holistic gate exists.

Back to the [index](INDEX.md).
