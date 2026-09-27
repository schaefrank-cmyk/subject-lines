# Endurance Subject Lines

A Claude Code skill that writes email subject lines for endurance events —
running races, triathlons, cycling sportives, obstacle races.

You give it a brief. It gives you a batch of options across proven categories,
each with its preheader text and a one-line explanation of the mechanism, so you
can choose on reasoning rather than gut feel.

## Why this exists

Most subject-line advice is written for e-commerce and doesn't survive contact
with a race calendar. Endurance events have a lifecycle that general advice
ignores: ballot results, deferral deadlines, a twelve-week training block, race
week logistics, finisher photos, and a win-back window that opens a year later.

This skill encodes that lifecycle, plus the mechanics that decide whether a line
works at all — truncation, preheaders, from-names, and the fact that open rate
stopped being a reliable metric in 2021.

## Install

```
/plugin marketplace add schaefrank-cmyk/subject-lines
/plugin install endurance-subject-lines
```

Then use it:

```
/subject-lines
```

Or just ask — the skill triggers on requests like "write subject lines for our
registration email" or "why isn't this race-week email getting opens?"

## What it does

1. **Takes a brief** — the event, the moment in the race year, the audience, and
   the action you want. It asks for what's missing and nothing more.
2. **Picks three or four categories** from a lifecycle map covering sixteen
   moments, from early access through lapsed-runner win-back.
3. **Writes three lines per category**, each with preheader text and the reason
   it works.
4. **Flags unverifiable claims** — if a line leans on "only 200 spots left" or a
   midnight deadline, it tells you that number has to be real.

## The nine categories

FOMO · Urgency · Curiosity · Pain point · Question · Re-engagement ·
Personalisation · Clarity/transactional · Social proof

Each is documented with worked examples and, more usefully, its failure mode —
the thing that makes it stop working permanently.

## Structure

```
skills/subject-lines/
├── SKILL.md                      the workflow
└── references/
    ├── categories.md             nine categories, examples, failure modes
    ├── lifecycle-map.md          which category fits which moment
    └── mechanics.md              length, preheaders, emoji, measurement, don'ts
```

## Adapting it

The examples are running-specific. If you work in a different endurance
discipline, or a different vertical entirely, `references/categories.md` is the
file to edit — the categories and their failure modes generalise, the examples
don't.

## Licence

MIT
