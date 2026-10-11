# Capture your brand voice and put it into your content workflows

**The working files from getting AI to write in one person's voice and grade
its own drafts until they only need last-mile edits.** Early and unpolished,
by [alex alderman](https://alderman.ai).

You're probably here from a LinkedIn message you didn't ask for. Fair 😇
The short version:

🔸 **What this is:** the working files from turning one person's writing
taste (mine: ~10 years and 2,000+ LinkedIn posts) into a rubric an AI agent
can write against *and* grade against.

🔸 **Why an agency should care:** AI writes *fine*. Your agency sells the gap
between fine and right-for-this-brand, and right now that gap lives in one or
two senior heads. Written down as a rubric, an agent can use it: write,
grade, rewrite, until a draft only needs last-mile edits.

One post from these files, before and after:

> **AI draft, opening lines:** The QA step everyone skips 𝗶𝘀𝗻'𝘁 𝗯𝗲𝗳𝗼𝗿𝗲 𝘆𝗼𝘂 𝗽𝘂𝗯𝗹𝗶𝘀𝗵. It's two weeks after. / The ten-minute audit that found four problems in one client's pipeline ⤵️
>
> **My note on it:** "Hook is 100% ambiguous to what intended audience you want to click on this post. Lots of fields have QA."
>
> **My rewrite:** 🔎 Agentic workflows 𝗵𝗮𝘃𝗶𝗻𝗴 𝗤𝗔 𝗹𝗼𝗼𝗽𝘀 𝗮𝗿𝗲 𝗻𝗼 𝗹𝗼𝗻𝗴𝗲𝗿 "𝗻𝗶𝗰𝗲 𝘁𝗼 𝗵𝗮𝘃𝗲". In 2026 they're non-negotiable. But not all QA is created equal. Here's how to go from intermediate to advanced 👇

Notes like that one are the raw material the rubric's 17 criteria were built from.

🔸 **The one thing to do:** have your own AI assistant walk you through it.
Paste this into your agentic assistant (Claude Code, Cursor, Codex, or any
agent that can read a folder):

```text
Clone https://github.com/alderman-ai/brand-voice-capture-demo-linkedin and open the folder.
Read its CLAUDE.md, then walk me through the demo.
```

You get a two-line menu:

1. **Why this is useful**: the idea behind it, one short page at a time.
2. **How this was made**: the method and the numbers, for a technical reader.

It explains the method, with my own graded posts as the examples. It won't
grade, rewrite or write posts for you with my rubric: the rubric is still
early (see "Honest status" below), and I don't put my name on its verdicts
about anyone else's writing.

Radši česky? Pište asistentovi česky a odpoví vám česky.

**No coding assistant?** The same pages read fine right here on GitHub:
start at [demo-and-more-help](demo-and-more-help/README.md).

**Never been to GitHub before?** Here's the marketing-friendly summary:
https://claude.ai/public/artifacts/9c96fcd8-6b5d-4ce8-b3e1-36137e75442c
(the missing section of my phone number isn't a typo, it's a redaction)

Nothing to install and nothing runs on your machine: this repo is markdown
files your assistant reads. That's it.

---

## Why I built it

Converting subjective taste and domain expertise into grading evals for
agents is one of my key areas of research, and my former GTM career makes
brand voice in content ops the main area of application. It's also the area
where I had the largest corpus to start the improvement flywheel on.

## What's in here

A small sample from early in the process of building the rubric-refining
method I'm still actively iterating on. They aren't polished documents, but
they should be legible with a little patience. Most legible first:

- **`starting-domain-expertise-from-operator.md`**: the extraction of my
  own 10 years of writing LinkedIn posts (😀🔫). Any rubric needs some
  quality floor to begin with: mechanical things like character counts
  before a line wraps, or that you need unicode to bold text on LinkedIn.
  This first iteration blended too much of the mechanical with my
  individual taste. I've gotten better at finding that line since.
- **`refinement-vector-2-full-rewrites.md`**: the grunt work. Taking agentic
  output and not just redlining it, but rewriting it entirely, with
  extensive notes. For client work this is the major bottleneck: clients
  aren't going to do this. But most corporate brands are 90% the same, so
  it's mostly a matter of tweaking word choice, especially in
  non-native-English countries in tech: how much of modern tech vocabulary
  stays English, even in the native language. That's the biggest dial to
  tweak for the CEE region. And that's very doable.
- **`refinement-vector-1-critiques.md`**: originally meant as a quick middle
  ground between dropbox grading and rewrites. The first iteration was
  basically partial rewrites. Now it's more like a comment-on-a-Google-Doc
  redlining experience.
- **`alderman-ai-linkedin-grading-rubric.md`**: an early version, with 17
  grading criteria and only 3 possible grades (Unpostable | Good | Great).
  I've since added Postable as the second of four. Most clients are
  perfectly fine with Postable, and it takes very little to achieve:
  basically the domain expertise extraction plus some minor refinements.
  Good as a floor is mostly for marketing agencies.

### Not shown

- Other grading vectors, mainly massive Airtables with super quick dropbox
  grading and no notes. There's no methodology I'm hiding there. It's just
  a. boring and b. I don't want to expose my entire ~2,500 corpus of
  self-written posts online.
- Another vector called **post silhouette**, probably the biggest
  breakthrough. You can see a small peek via the summary link above.
- Much more refined versions of the files shown. You get it.

### Honest status

The rubric calls itself "a directional instrument, not a validated one" in
its own header: its first version was built on ~20 unique graded posts, and the Great grade
rests on a single as-written example. It says so up front instead of hiding
it, and so do the help pages (menu line 1, "Honest limits").

## Want to talk?

You already have me in your LinkedIn messages: just reply there. One word is
enough and we'll find 30 minutes. A "no thanks" works too.

Found this some other way? Book the 30 minutes here:
https://calendar.app.google/biAvGYqEqUtmtsNv9 or see [alderman.ai](https://alderman.ai).

## Repo layout

```
README.md                      you are here, written for you (the human)
CLAUDE.md / AGENTS.md          identical; how your assistant orients itself
alderman-ai-linkedin-grading-rubric.md     the rubric (v2.1)
starting-domain-expertise-from-operator.md the starting quality floor
refinement-vector-1-critiques.md           10 posts, graded and critiqued
refinement-vector-2-full-rewrites.md       5 posts, rewritten with notes
demo-and-more-help/            the two menu lines:
  why-this-is-useful/          the idea, for agency owners
  how-this-was-made/           the method, for technical readers
LICENSE                        MIT
```
