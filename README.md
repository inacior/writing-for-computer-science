# Sci-Wri

A skill that reviews, revises, and drafts scientific and technical writing to
the standards of Justin Zobel's *Writing for Computer Science*. It distills the
book into actionable rules for papers, theses, reports, and talks in computing
and mathematics.

## Installation

Copy the skill folder into your agent's skills directory, for example:

```bash
mkdir -p ~/.codex/skills
cp -R sci-wri ~/.codex/skills/
```

For Claude Code or other agents, use their skills directory (e.g.
`~/.claude/skills/sci-wri`) or register the path via the agent's skill config.

## Usage

Invoke the skill, then paste the text:

```
/sci-wri

[your text]
```

Or ask directly: "Review this abstract using sci-wri" / "Rewrite this
introduction to match Writing for Computer Science."

## What it covers

| Reference | Contents |
| --- | --- |
| `references/01-article-structure.md` | Title, abstract, introduction, survey, results, conclusions, composing the paper |
| `references/02-editing-checklist.md` | Full revision and consistency checklist |
| `references/03-style.md` | Economy, tone, sentence and paragraph structure, ambiguity, word choice, tense, usage, sexist language |
| `references/04-punctuation-math.md` | Punctuation conventions and mathematical notation, numbers, units |
| `references/05-figures-algorithms.md` | Graphs, diagrams, tables, captions; algorithm presentation and complexity |
| `references/06-experiments-refereeing-talks.md` | Hypotheses and experiments, refereeing, and short talks |

## Design

- `SKILL.md` holds the workflow, core principles, and the most common fixes, and
  points to the detailed reference files (progressive disclosure).
- Reference files are structured notes extracted from the book, with watchlists
  and before/after examples drawn from the original.

## Source

Based on *Writing for Computer Science* by Justin Zobel (Springer). The book
text was parsed to Markdown and distilled; the skill contains guidance derived
from it, not the book itself.

## Version history

- **1.0.0** — Initial release. Workflow, core rule cards, and six reference
  files distilled from all 11 chapters.
