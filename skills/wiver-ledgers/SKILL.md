---
name: wiver-ledgers
description: Create and update the ledgers of Wivoo consultants looking for a mission, from their dossiers de compétences on Drive to one ledger page per consultant in Notion. Use when asked to build, refresh or check the ledgers, or when a consultant joins the intermission list or updates their DC.
---

## Ledgers

Ledgers are built from the DCs on Drive and stored in Notion, where the matching step reads them. Keeping them up to date is its own task, run separately from matching a fiche.

Every consultant listed on the Notion page "Ledgers et Consultants en inter-mission" (`3ea331cabede8076b82ae0acc07cb47a`) needs a ledger. Follow that page's instructions to get their names and statut de mission.

Their DCs are on Drive:

- "DC- Consultants Wivoo" (`149FelJQXXY6lZSE40By4D-ApIldqYSJp`), with one subfolder per consultant named roughly "DC - Prénom NOM".
- "DC - Consultants en process" (`1mgY6WGKpebJFh91Na9VWGTl6Wr9m8Dq-`), for consultants in the recruitment process: often one or two slides per person, rarely in a folder of their own.

Their ledgers are child pages of the Notion page "Ledgers" (`3eb331cabede8000a6fcd7e0da4f3274`), titled `ledger_prenom_nom` in lowercase without accents.

A ledger needs building when the consultant has no ledger page, or when one of their DCs was modified on Drive after their ledger page was last edited in Notion. Build each one by following `build.md`, with one subagent per consultant that reads only that person's files: when several people's DCs share a context, experience ends up attributed to the wrong person.

A consultant with no usable DC still gets a ledger page, saying so in one line, so matching sees them rather than guessing. In Recrutement this is expected: « Pas de DC : en recrutement, pas encore rédigé. » For anyone else it deserves a look: « Pas de DC trouvé sur Drive. »
