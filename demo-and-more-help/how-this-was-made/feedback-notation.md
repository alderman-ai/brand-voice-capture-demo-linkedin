# Feedback notation

Taste capture lives or dies on how the expert's notes are written. The
starting notes (`starting-domain-expertise-from-operator.md`) define the
notation so "they aren't ambiguous to the assistant processing the notes."

## The conventions

- **Attribution tags.** Pairs of tags mark who wrote a document or section:
  `<operator_authored>` around the starting notes, `<operator_response>`
  around each rewrite. Anything outside the tags is not the operator's voice.
- **Inline notes** use `///<note>`, often inside backticks. On a rewrite, the
  assistant must be able to read the post as if the notes weren't there, or
  say that it can't.
- **Structured fields**: a `Notes:` or `Feedback:` section under a post, or a
  designated field in a spreadsheet such as Airtable.
- **Coverage rule**: "Silence does not equal endorsement." The operator may
  skip a category he has commented on many times, and that must not lower
  its weight. Dismissing a post as "ai slop" is not total condemnation
  either.

## The two refinement formats

- **Critiques** (`refinement-vector-1-critiques.md`): the generated post
  quoted, the pass-1 grade, then a bullet critique "before reveal". The
  "After the reveal" sections were left empty.
- **Rewrites** (`refinement-vector-2-full-rewrites.md`): the generated post,
  the pass-1 grade, then the operator's rewrite with four fixed headings:
  Self-grading, Key strengths, Key weaknesses, Rewrite Notes. The rewrite
  notes are where most v2 doctrine came from: reordering words so a bolded
  string stands alone as a clause, choosing an emoji for its colour against
  its neighbour, and why 🔥🚗 beats 🛣️🔥 for a human reader.

## The hook-as-thesis finding

In his closing notes to the rewrites file, the operator records a design
change he hadn't yet scoped: the hook should be the body's thesis, so hook
generation should be a **separate skill** that outputs the hook plus a short
"body direction", which makes the pair an atomic artifact you can run
Best-of-N on by itself. The same idea failed as a rubric criterion
(hook-as-thesis was discarded in v2 because a blind reader couldn't
reproduce it) and moved into the writing side instead.

Back to the [index](INDEX.md).
