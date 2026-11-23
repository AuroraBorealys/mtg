# Instructions for AI collaborators

This repo holds one Magic: The Gathering deck. Several assistants work on it
(Claude, ChatGPT/Codex, Gemini). This file is the single source of truth for
how to work here; `CLAUDE.md` and `GEMINI.md` just point to it.

## The deck
- Format: Commander (100 cards including the commander, singleton except basic lands, color identity rules apply)
- Commander: The Borg Queen ({4}{W}{U}{B}, Esper: white/blue/black). Every
  card must fit inside W/U/B color identity.
- Archetype: artifact creature "tribal", played like slivers: go wide with
  many artifact creatures that the Queen's +2/+2 anthem turns into a big army
- Budget: No limit
- Power level: High-power (strong at a typical game-store Commander night; not
  necessarily full cEDH)
- Goal: win through combat with a wide board of pumped artifact creatures.
  Every attack with the Queen assimilates an opponent's creature, adding to
  the army. Prioritize cheap artifact creatures, ways to protect the board and
  the commander, more anthems and artifact payoffs, and enough card draw and
  interaction to keep up at a high-power table.

## Deckbuilding rule: don't build around the commander
The deck must be strong without The Borg Queen ever being cast. She costs 7 and
will often be removed; treat her as a bonus, not the plan.
- Don't add cards that only work while the commander is on the battlefield
  (e.g. Fierce Guardianship, Deadly Rollick).
- Don't add commander-protection equipment (Lightning Greaves, Swiftfoot Boots).
- Don't add a card just because it's Borg/Star Trek flavored; it has to be good on its own.
- When judging a card, ask "is this good if the Queen never shows up?"
- EDHREC popularity, synergy scores and "it's a staple" are not reasons on their own.
  Say what job the card does in this deck and why it beats the card it replaces.
  Cards from the earlier, played builds in `notes/earlier-builds/` carry extra weight.

See `notes/deck-plan.md` for the full plan.

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
