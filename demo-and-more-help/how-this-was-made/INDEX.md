# how-this-was-made/

**How the rubric in this repo was built, for a technical reader.** This is
where line 2 of the assistant's menu lands. Jargon is allowed here; each page
defines its terms where they first appear.

## The build story in ten sentences

It starts with the operator (Alex) writing down, in his own words, the
global rules and lexicon he applies to every LinkedIn post: hook formats,
character limits, what "bold" means, an emoji taxonomy. Version 1 of the
rubric was then *induced* (derived from graded examples rather than written
top-down) from 34 posts he had graded Unpostable, Good or Great, with his
freeform notes as the source of candidate criteria. 23 candidate criteria
were tested by blind validators (fresh subagents that saw post bodies only,
no grades, no notes): 782 judgments, and only the 11 criteria that actually
separated the tiers survived. Version 2 came from a second, independent
corpus: 60 posts from a Best-of-N experiment (generate several candidates,
keep the best), graded blind by Alex, plus his 10 critiques and 5 full
rewrites, which are the two refinement files in this repo. 13 new candidates
went through 780 more blind judgments under decision rules registered before
any judgment was collected; 6 became new criteria, one existing criterion
was narrowed and 6 were discarded, and the three hook adoptions that broke a
pre-registered rule say so on the criterion itself. Version 2.1 swapped
an assistant-inferred rule for the operator's own wording and removed a stray
template token that every grader call since v2 had been reading literally.
The result is one criterion core with two views: a grading view that is the
complete grader prompt, and a writing view that is the same criteria as
instructions. Third-party posts are cited by record ID only, every superseded
version is kept byte-identical, and the honesty clause comes before any
number.

## The pages

1. [The four files](the-four-files.md) -- what each file is, how they feed
   each other, and why they're named "refinement vectors".
2. [Version 1: inducing the rubric](inducing-v1.md) -- the 34-row corpus,
   23 candidates, 782 blind judgments, and what got discarded and why.
3. [Version 2 and 2.1: the Best-of-N pass](the-best-of-n-pass.md) -- 60
   posts, pre-registered rules, the documented deviation, and the two
   v2.1 fixes.
4. [One core, two views](one-core-two-views.md) -- the grading view as a
   grader payload: evaluation order, citation rules, the voice-authority
   rule, and "classify the hook first".
5. [Feedback notation](feedback-notation.md) -- how the operator's notes
   are written so an agent can parse them, and the hook-as-thesis finding.
6. [Provenance and honesty rules](provenance-and-honesty.md) -- the archive
   chain, third-party protection, and the forbidden inferences.
7. [Timeline](timeline.md) -- dates from the rubric's own header and from
   `git log`.

Every fact traces to a file in this repo (mostly the rubric's §A, §F and §H)
or to `git log`. Paths the rubric cites under `Working/` and `Deliverables/`
live in Alex's private workspace and are not in this repo.
