---
name: mike-voice
description: >-
  Write or rewrite anything so it sounds like Mike wrote it. Use for "write this in my voice,"
  "make this sound like me," "LinkedIn post," "blog post," "newsletter," "rewrite this,"
  "punch this up," website copy, landing pages, value props, messaging, taglines, ads, emails,
  in-app copy, launch copy, sales decks, sales enablement, battle cards, one-pagers, strategy
  memos, resumes, cover letters, LinkedIn about sections, and interview answers. Pulls Mike's
  real writing and stances from his Obsidian vault instead of guessing a style. Composes with
  structure skills (copywriting, resume, sales-enablement): they decide the shape, this decides
  the words. Do not use for positioning statements or the positioning constitution, which
  belong to pmm-positioning.
allowed-tools: Read Grep Glob Bash Write Edit
metadata:
  version: 1.0.0
---

# Mike's voice

## The rule that decides everything

**Every draft is built from Mike's real writing and Mike's real opinions, opened in this
session.** The vault is the source of truth and it keeps growing:
`/Users/mikesavoff/Documents/Obsidian Vault`. Read the exemplar notes themselves, not a memory
of them. If a piece needs an opinion Mike has never stated, ask him for it. Never invent his
stance, his history, or his numbers.

## Route the register

| Register | Use for | Core move |
|---|---|---|
| **Author** | LinkedIn posts, blog posts, essays, newsletters, personal notes | First person. Real stakes, a self-own, then conviction. |
| **Copy** | Website, landing pages, value props, messaging, taglines, ads, emails, in-app, launch copy | Write as the customer. Scenes, not labels. The problem before the product. |
| **Operator** | Resumes, cover letters, interview answers, sales decks, enablement, battle cards, memos | Mike's framing and stances in plain, declarative sentences. Humor at most once. |
| **Off** | Positioning statements, the positioning constitution | Hand to `pmm-positioning`. Don't apply this skill. |

A mixed piece (e.g. a job-search post) takes the register of whoever reads it. If that's
unclear, ask one question with the options above.

## Stances

- **Author:** no stance, no draft. Match the topic to `references/stance-bank.md`. If nothing
  matches, stop. Offer Mike 2-3 candidate angles built from his closest stances, labeled
  **[Hypothesis]**, and ask which one is his.
- **Operator:** the stance comes from the approved artifact the piece carries (messaging, ICP,
  battle card research). Mike's stances shape the framing only.

## Retrieval protocol (`references/corpus-index.md`)

1. Route the register.
2. In the corpus index, pick 2-3 notes whose "Pull when" matches the register and topic.
   Always include one published piece (`linkedin posts/` or `copy/`).
3. Read those notes in full from the vault. Only use notes tagged `voice-sample: true`.
   Notes tagged `false` may inform a stance. Their style is never imitated.
4. Pull the matching stances and any biography facts from `references/stance-bank.md`.
5. Draft with `references/fingerprint.md` open. For the copy register, also open
   `references/copy-register.md`.
6. Run `references/red-team.md` on the draft. Fix and re-run until it passes.
7. Deliver the draft. Then add one line naming the notes it drew from, so Mike can check it.

**Vault unreadable** (claude.ai, another machine): work from the verbatim excerpts in the
references. Say so in one line.

**Untagged vault note** (new writing): read it and run the authorship test in `red-team.md`.
Add the frontmatter (`voice-sample`, `voice-register`, plus `voice-exclude-reason` if false).
Add a row to the corpus index. Add any new stance to the stance bank with a quote.

## Right-size the job

- **One line or a short edit:** rewrite it and run the red team in your head. Skip retrieval
  beyond the fingerprint.
- **A full piece:** run the whole protocol.
- **A rewrite of someone else's draft** (including an AI draft): keep the argument. Replace the
  voice. Add lived detail only from the stance bank.

## Never

- Invent a biography fact, number, employer, result, or anecdote. If the piece needs one, leave
  `[Mike: the time X happened?]` in the draft.
- Collage. Exemplars teach rhythm, moves, and word choice. They aren't lines to reuse. At most
  one sentence per piece may come verbatim from the corpus, and only when Mike's exact words
  are the point (a quote he's known for). Everything else is new sentences in his voice.
- Use a private biography fact without Mike's OK (see the stance bank).
- Imitate text from a `voice-sample: false` note.
- Use em-dashes. Mike uses a spaced hyphen: " - ".
- Publish in lowercase. The vault drafts are lowercase. Published pieces are sentence case.
  Only write lowercase when Mike asks for notes or a draft in his raw style.
- Explain a joke, or stack more than one joke per short section.
- Put Mike's jokes, slang, or emojis into an operator piece meant for buyers or executives.
  His framing belongs there. His jokes don't.

## Output

The piece, ready to paste. After it, one line of sources ("Drew on: linkedin vs reality,
posthog superday"). Then any `[Mike: ...]` gaps he needs to fill. No preamble, no summary of
what you did.

## Related skills

- `pmm-positioning` owns positioning. This skill never writes it.
- `copywriting`, `resume-*`, `cover-letter-generator`, `sales-enablement`, `linkedin-content`:
  they set structure and length. Run them first, then pass their output through this skill.
