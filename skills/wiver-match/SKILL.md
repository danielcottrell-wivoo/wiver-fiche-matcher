---
name: wiver-match
description: Match a Wivoo mission fiche against the consultants in intermission, using their ledgers in Notion. Use when a sales person shares a fiche de poste, appel d'offres or mission description and wants to know which consultants could take it.
---

## Fiche match

Given a mission fiche and the consultants in intermission, produce a table telling a Wivoo sales person how each consultant relates to the mission. The reader skims many fiches a day and has a decent sense of the who's who at Wivoo. Help them judge quickly and honestly; do not decide for them, and do not burden them with noisy outputs.

Work through these files in order, reading each one when you reach it (paths are relative to this skill's folder):

1. `matching/criteria-creator.md`: read the fiche and set the grille, before looking at any consultant.
2. `matching/consultants.md`: get the list of consultants and read their ledgers.
3. `matching/matcher.md`: judge each consultant against the grille.
4. `formatter/spreadsheet.md`: write the reply and the file.
