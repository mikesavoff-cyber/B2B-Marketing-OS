# Corpus index

The vault is `/Users/mikesavoff/Documents/Obsidian Vault`. Paths below are relative to it.
Every note has a `voice-sample` property. Only `true` notes are style exemplars.
If the vault isn't readable, the same notes are verbatim in `vault-snapshot.md`.

Published pieces are the strongest evidence of the finished voice. Vault notes are drafts
(lowercase, rougher): they show the thinking and the phrasing, not the final polish.

## Published (read one of these for every full piece)

| Note | Register | Pull when | Signature lines |
|---|---|---|---|
| `linkedin posts/posthog superday.md` | author | Admiration, ambition, culture, a long shot, rejection turned into conviction | "companies that taste like AI-generated broccoli" · "(it's on their website, next to the team's feet pics)" · "The success of your product is not measured just by data. It's measured by how people feel about it and how they describe that feeling." |
| `linkedin posts/jobs in 2027.md` | author | Reacting to someone else's article, AI anxiety, job market, burnout | "Joke's on both of them - I don't have a job right now. 🤡" · the vertical "no / matter / their / role." · "Obviously - chill the heck out first." |
| `linkedin posts/tactiq and whats next.md` | operator | Resume, cover letter, about section, job-search post, "what I do" | "I joined Tactiq at 300K users. Now they're over 1,000,000." · "What do I do best? / Create, ship, and refine the story that lands the right customers." |
| `copy/atomus.md` | copy | Any customer-facing copy | "Wanna hear the really bad part?" · "a pain in the Behance" · "Make your boss say 'You're too good for us.'" |

## Vault drafts

| Note | Register | Pull when |
|---|---|---|
| `why marketing is struggling so much.md` | author | Marketing vs leadership, founders, internal marketing, trust |
| `marketing marketing to founders.md` | author | Same theme, shorter; "felt it before I could articulate it" |
| `linkedin vs reality.md` | author | Advice vs real work, frameworks don't transfer, numbered lessons |
| `pmm is not getting replaced.md` | author | AI, slop, hype, what AI is actually good for in PMM, personal life |
| `wtf is context engineering.md` | author | Explaining a technical topic as a self-described "simple product marketer" |
| `define your icp and their problem, ... writes itself.md` | author | Problem framing, messaging, teaching a method with steps and examples |
| `icp + acv = $$$.md` | author | ICP, ACV, GTM motion; a punchy post that addresses someone by name |
| `market > marketing > product marketing.md` | author | Defining marketing vs PMM; tight definitional lists |
| `what is great product marketing without great distribution?.md` | author | Generalist, only marketer in the room |
| `nothing has changed for over a decade.md` | author | Short hook: same problems 10 years later |
| `problem framing.md` | author | One-line thesis on problem framing |
| `why marketers should start a business.md` | author | One-line jab at blaming leadership |
| `emotional storytelling in b2b.md` | author | Stub. Thesis only, no argument yet |
| `how to simplify positioning sprints.md` | author | Stub. "i never do the whole sophisticated and smart sounding marketing spiel" |
| `posthog interview.md` | operator | Interview answers, "how I work," values: extreme empathy, annoying curiosity, ship around and find out |
| `posthog/messaging ideas.md` | copy + operator | Dev-tool copy riffs (LLM cost); self-description for interviews; sharp interview questions |
| `posthog/questions.md` | operator | Questions Mike asks a hiring team |
| `Revolut/Revolut.md` | operator | Strategic take on a company's narrative; trust over mechanics |

## Excluded (`voice-sample: false`)

| Note | Why | Allowed use |
|---|---|---|
| `competing with competitors vs competing with what customers think about them.md` | AI-drafted style: em-dashes, "Here's what it means in practice", "That's the whole job." | The belief-map idea is a stance. Never imitate the style. |
| `Claude outputs/` | Written for Claude, not by Mike as writing | None |
| `Untitled.md`, `how do you defend the purchase to a cfo.md`, `how to build a marketing function that drives results.md`, `when someone likes a post - i want this signal registered.md` | Empty. Titles only | The titles are topics Mike wants to write about. Ask before drafting one |

## Maintenance

When a note is added, tagged, or used for something its "Pull when" wouldn't surface, update
this table in the same session. A note isn't indexed until every stance it argues is in
`stance-bank.md` with a quote. This applies to published pieces most of all: they are Mike's
public positions. Then rerun `scripts/snapshot.py` so the fallback stays current.
