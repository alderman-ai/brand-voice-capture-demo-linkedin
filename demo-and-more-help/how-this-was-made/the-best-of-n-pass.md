# Version 2 and 2.1: the Best-of-N pass

*Best-of-N* means generating several candidates for the same brief and
keeping the best. Source: the rubric's §A, §B and §H.

## Version 2 (2026-08-11)

**A second, independent corpus**: 60 posts written for the Best-of-N
experiment and graded blind by the operator, **42 Unpostable / 17 Good /
1 Great**, plus his 5 rewrites and 10 critiques (the two refinement files in
this repo). The two corpora are never pooled.

**The test**: 13 candidate criteria × 60 rows = **780 blind judgments** by
four isolated validators, bodies only. The decision rules were registered
**before any judgment was collected**.

**Outcome**: 11 criteria → 17.

- **Validated on the data alone**: hook emphasis balance (HBAL-28),
  +39 percentage points of separation.
- **Adopted as Great-blockers only**, labelled "doctrine-supported;
  tier-separation unmeasured", because the Great tier had n=1: every bold has
  a role (BOLD-25), 🤡 targets peers (CLWN-22), length is earned (LEN-27).
- **Adopted under a documented deviation**: approved hook format (HOOKF-19),
  no hook-line wrap (WRAP-20), and a narrowing of "the fold earns the click"
  (HOOK-06). Strongest separators in the set (+30 to +36pp), but they failed
  a pre-registered false-positive cap on 3 to 4 Good rows. An isolated
  adjudication of those rows found 0 contradicting, 4 disavowed by the
  operator, 2 silent, and the cause: **the grading interface could not
  display line wrap**, so no row ever validly endorsed a wrapping hook. The
  deviation is recorded on the criterion itself and is reversible.
- **Discarded, 6 of 13**, each with its numbers. The notable one is
  hook-as-thesis (COHR-24): the operator saw incoherence that a blind reader
  couldn't reproduce from the body alone, so it moved into the writing skill
  as hook-first drafting instead of into the rubric. Another was discarded
  exactly as its own author predicted.
- **Retired**: none.

## Version 2.1 (2026-08-12)

No criterion added or removed, hence 2.1 and not 3. Three fixes:

1. **The style-2 hook rule.** v2 defined it as "a paragraph filling the
   three above-the-fold lines", an assistant inference made before the
   operator had written a style-2 section. His own spec is **100 to 240
   characters**, and the old wording would have failed conforming hooks in
   the 100 to 172 range. The rubric flags that the +36pp figure was measured
   against the old wording and must not be quoted for the new one.
2. **A stray `{{rubric_grading_view}}` token** in the grading view's own
   first line. Because that section *is* the payload, every grader call
   since v2 read a literal template placeholder, confirmed in all twelve
   payloads checked.
3. A stale count: "all eleven criteria" → "all seventeen".

**Consequence for line wrap**: measured over Alex's 30 published posts, the
only three hooks over 85 characters were 166, 168 and 170 characters, all
valid style-2 paragraphs, flagged as wraps because the checker couldn't tell
the formats apart. Hence the rule: classify the hook first, then count.

Back to the [index](INDEX.md).
