---
name: subject-lines
description: Writes email subject lines for endurance events — running races, triathlons, cycling sportives, obstacle races — from a short brief. Generates a batch of options across proven categories, each with its preheader and the reason it works. Use when the user asks for subject lines, email subject line ideas, or help with the subject line for a race email; wants options for a registration push, price-increase deadline, ballot result, race-week send, results or photos email, or lapsed-runner win-back; or asks why a subject line isn't getting opens.
---

# Endurance Event Subject Lines

Generate subject lines for race emails from a brief. The output is a batch of
options across several categories, each paired with preheader text and a short
reason it works, so the user can choose on judgement rather than vibes.

The job is **selection and reasoning**, not volume. Twelve considered lines with
their logic beat fifty variations of the same idea.

## Workflow

### 1. Establish the brief

You need four things. Ask only for what's missing — don't interrogate someone
who already gave you enough.

| Need | Why it changes the output |
| --- | --- |
| **The event** | Distance, location, and whether it's mass-participation or niche |
| **The moment** | Where in the race year this sits — see `references/lifecycle-map.md` |
| **The audience** | Everyone, first-timers, returning finishers, lapsed, ballot losers |
| **The action** | Register, defer, buy photos, read a training guide, join a waitlist |

If the user gives you a one-liner like "subject lines for our registration
email," ask for the moment and the audience. Those two change the output more
than anything else. Don't ask for all four when two will do.

**Also ask whether per-runner data is available** — finish times, bib numbers,
rank, previous races run, weeks until their race date. If it is, personalisation
becomes available, and it outperforms every other category. Don't assume it
isn't available; most event platforms have it and marketers forget.

### 2. Pick the categories

Read `references/lifecycle-map.md` and find the moment. It names a primary and
secondary category for each point in the race year.

Generate across **three or four categories**, not one. The user is choosing a
direction as much as a line, and seeing urgency next to personalisation next to
clarity makes the choice concrete.

Read `references/categories.md` for what each category is, when it earns its
place, and its failure mode.

### 3. Write the lines

Three per category. Each line gets:

- **The subject line**
- **Preheader** — a second sentence that continues the thought, never an echo
- **Why it works** — one sentence, naming the mechanism

Check every line against `references/mechanics.md` before you present it. The
checks that catch the most problems:

- Does the meaning land in the first 30–35 characters?
- Is the preheader written, or defaulted?
- Is it one technique, cleanly, rather than three fighting?
- If it claims a deadline, a number or a scarcity, is that claim real?

### 4. Flag what you can't verify

If a line depends on a fact you were given rather than one you can check — "only
200 spots left," "62% come back," "prices rise at midnight" — mark it. Say
plainly that the number has to be true.

This matters more in this category than most. A list learns within two or three
sends whether your deadlines mean anything, and once it decides they don't,
urgency stops working for that sender permanently. Don't let someone ship a
fake deadline without saying so.

### 5. Present

Group by category. Lead with the category you'd actually pick and say why in one
sentence. Don't hedge across all four — the user asked for help choosing.

Close with the one thing that would most improve the next send. Usually it's
per-runner data, a real number to replace a placeholder, or a preheader strategy
the programme doesn't have yet.

## Rules

- **Never stack techniques.** "🔥 FINAL CALL: Kyra, only 200 spots before prices
  rise at MIDNIGHT" is four techniques in 35 characters. One, executed cleanly.
- **Logistics emails stay plain.** Confirmations, bib numbers, race-week
  instructions: no emoji, no discounts, no exclamation marks. The moment an
  essential email looks promotional it gets treated as promotional, by the
  reader and by the filter.
- **Don't optimise for opens.** Apple's Mail Privacy Protection has made open
  rate unreliable since 2021. If the user frames success as open rate, say so
  and point them at clicks and downstream registrations.
- **Personalisation needs a fallback.** Any line with a merge field ships with a
  default value and a seed-list test, or it doesn't ship.
- **Curiosity gaps must pay off.** If the email doesn't deliver what the subject
  line implied, the line is a liability regardless of its click rate.

## References

- `references/categories.md` — the nine categories, with examples and failure modes
- `references/lifecycle-map.md` — which category fits which moment in the race year
- `references/mechanics.md` — length, preheader, from-name, emoji, measurement, what not to do
