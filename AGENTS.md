# Instructions for AI collaborators

This repo holds one Magic: The Gathering deck. Several assistants work on it
(Claude, ChatGPT/Codex, Gemini). This file is the single source of truth for
how to work here; `CLAUDE.md` and `GEMINI.md` just point to it.

## The deck
- Format: TBD (fill in: Commander, Standard, Modern, Pauper, ...)
- Commander / archetype: TBD
- Budget: TBD
- Goal: TBD (what the deck should do, how competitive it should be)

## Files
- `deck/decklist.txt` – the decklist. This is the only canonical list.
- `notes/` – reasoning, matchup notes, card evaluations, ideas to test.
- `CHANGELOG.md` – one entry per change to the decklist.

## Decklist format
One card per line, `<count> <exact card name>`, e.g. `4 Lightning Bolt`.
Use exact English card names as printed on Scryfall. Sections are marked with
a line starting with `//` (e.g. `// Commander`, `// Sideboard`). No other syntax.

## How to propose changes
- Work on a branch and open a pull request; never push straight to `main`.
- Name branches after yourself and the idea, e.g. `claude/more-removal`.
- In the PR description, list every card in and out with a short reason.
- Add a dated entry to `CHANGELOG.md` with the same ins/outs.
- Check the card count and format legality before proposing.
- Don't rewrite another assistant's notes; add your own file or section.
