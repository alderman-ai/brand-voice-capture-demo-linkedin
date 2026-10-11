# The loop: write, grade, rewrite

A rubric on its own is a style guide. What makes it worth building is that an
agent can **grade against it**.

## One file, two views

The rubric (`alderman-ai-linkedin-grading-rubric.md`) holds the same criteria
twice:

- a **writing view**: 14 instructions, in order, for the agent writing the
  post ("write the hook first", "count the hook lines before shipping",
  "spend emphasis like a budget", "then read it as a stranger scrolling");
- a **grading view**: the same criteria as checks, run in a fixed order.
  Hard fails first; the grader writes its reasoning before its verdict and
  quotes each criterion it relies on.

Put the two together and a workflow can loop: draft, grade, rewrite what
failed, grade again, until what reaches a person only needs last-mile edits.

## The rubric loops too

The expert's feedback comes in at three speeds, all described in this repo:

- **Quick grades**: just the grade, no notes, in large tables. Fast, and
  not shown here.
- **Critiques**: redlining a draft, like comments on a Google Doc
  (`refinement-vector-1-critiques.md`, ten posts).
- **Full rewrites**: the expert rewrites the post from scratch and explains
  every choice (`refinement-vector-2-full-rewrites.md`, five posts). The
  slowest, and the richest signal.

Every proposed criterion is then tested against posts Alex had already
graded: does it actually separate the Unpostable ones from the Good ones? If
it doesn't, it goes. In the second round, 13 candidate criteria were tested
against 60 graded posts, and 6 were thrown out.

## The bottleneck is the expert's time

Alex's starting notes are explicit about it: "Silence does not equal
endorsement." He comments on what is most instructive, skips what he has
already said many times, and sometimes just marks a post Unpostable. The
rubric is built to cope with that rather than to demand more of his time.

For client work, the full rewrites are the bottleneck. In his words: "They
aren't going to do this." The next page is about what that means for an
agency.

Back to the [index](INDEX.md).
