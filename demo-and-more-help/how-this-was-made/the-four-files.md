# The four files

The repo is four markdown files plus this help folder. No code, nothing
executable.

| file | role | written by |
|---|---|---|
| `starting-domain-expertise-from-operator.md` | the starting quality floor: global grading rules, feedback syntax, the two approved hook formats, the LinkedIn lexicon (bold, emphasis, above the fold, Click-TA, break point), the emoji lexicon | the operator, by hand (wrapped in `<operator_authored>` tags) |
| `alderman-ai-linkedin-grading-rubric.md` | the rubric itself, v2.1: 17 criteria, a grading view, a writing view, worked examples, rewrite deltas, and the validation record | induced by assistant sessions from operator grades; every adoption ruled on by the operator |
| `refinement-vector-1-critiques.md` | 10 generated posts (IDs P-008 to P-059) with the operator's pass-1 grade and a detailed critique of each | the posts by the generator; the critiques by the operator |
| `refinement-vector-2-full-rewrites.md` | 5 generated posts, each rewritten from scratch by the operator with a self-grade, key strengths, key weaknesses and rewrite notes | the operator, inside `<operator_response>` tags |

## How they feed each other

1. The **starting notes** are the floor: the mechanical rules any rubric
   needs before induction can say anything useful. They are also the
   *source*: when the rubric and the notes disagree, the rubric records that
   the notes win ("read the source, not the derivation").
2. The **rubric** is induced from graded posts and validated blind. Its
   v2 amendments were induced in part from the two refinement files.
3. The **refinement vectors** are two ways of getting richer signal than a
   bare grade. "Vector" here means a channel of feedback. The critiques are
   a middle ground between quick grading and rewrites; the rewrites are the
   most direct statement of taste the corpus has, and the most expensive.

## The names

The files were renamed on upload (from `git log`, 2026-08-28):

- `Global LinkedIn Grading Context.md` → `starting-domain-expertise-from-operator.md`
- `BoN-pass3-critiques.md` → `refinement-vector-1-critiques.md`
- `BoN-pass2-rewrites.md` → `refinement-vector-2-full-rewrites.md`

The file headers keep the internal names ("G5 pass 3 — detail critiques",
"G5 pass 2 — rewrites"). The rubric still refers to the starting notes by
their old name, `Global LinkedIn Grading Context.md`.

Back to the [index](INDEX.md).
