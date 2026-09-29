---
name: wiver-match
description: Match a Wivoo mission fiche against the consultants in intermission, using their dossiers de compétences on Drive. Use when a sales person shares a fiche de poste, appel d'offres or mission description and wants to know which consultants could take it.
---

## Fiche match

Given a mission fiche and the consultants in intermission, produce a table telling a Wivoo sales person how each consultant relates to the mission. The reader skims many fiches a day and has a decent sense of the who's who at Wivoo. Help them judge quickly and honestly; do not decide for them, and do not burden them with noisy outputs.

Each consultant has a folder in the Drive folder "DC- Consultants Wivoo" (`149FelJQXXY6lZSE40By4D-ApIldqYSJp`), named roughly "DC - Prénom NOM". The folder holds their DCs and a `ledger.md`: a complete record of what their DCs say, written for you to match against.

### 1. Read the fiche and set the grille

Start from the fiche alone, before reading any ledger, so the grille reflects the job rather than the pool. Fiches are dense and written in the client's vocabulary, and their title does not always match the work. Work out the core work of the job: what the consultant will actually do day to day. Tools, sector and education listed in the fiche are secondary.

Every fiche implies a grille: the few things that decide who can do this job. Make it explicit with 3 to 6 criteria, or more if you judge it necessary. Phrase each one as work to have done, not as keywords or tools, and give it one line on why it matters here. Mark which criteria are core: they decide the verdict, while the others only order people within a verdict. Sector, or prior work at this client, becomes a criterion only when the fiche makes it matter. Seniority is always assessed, separately.

If the fiche describes more than one role (for example a project manager plus technical profiles), give your reading of each role and ask the user which one to match, or both, before going on. For several roles, produce one grille and one tab per role.

### 2. Ledgers

For each name, find the folder and list its files. If there is no `ledger.md`, or any other file was modified after it, rebuild it by following `ledger-builder.md`. Then read `ledger.md`.

### 3. Judge each consultant

Go through the consultants one at a time and fill in the grille.

- Missions in the ledger are the evidence; the profile tells you what the person claims.
- Judge the work, not titles, keywords, tools or sector. Someone who did the work with other tools fits.

Each criterion gets a mark, then one sentence saying what the person's experience means for that criterion, in words the sales person could repeat to the client. The sentence interprets; it does not just list activities.

- Not this: "BA : ateliers, campagnes UAT, suivi anomalies (Alstom)"
- This: "● Elle a déjà porté ce cycle complet chez Alstom, du cadrage avec le métier jusqu'à la recette."

| Mark | Meaning |
|---|---|
| ● | Has done it, as the main role, in a comparable context |
| ◕ | Has done it, in a smaller or different context |
| ◑ | Has done part of it, or in support |
| ◔ | Adjacent work only |
| ○ | Nothing in the DC |
| ? | Claimed but never shown in a mission, or the DC is unclear |

For seniority, count the years spent doing the kind of work the fiche asks for, from mission dates; mention the total career only when it changes the picture. If the fiche names a level rather than a number ("Senior Consultant"), work from that and say so. Mark ✓ in range, ▼ below, ▲ clearly above, ? when the dates don't allow a count, each with one sentence:

- "▼ 3 ans de Product Owner sur 10 d'expérience ; la fiche en demande 5."
- "▲ 12–15 ans et grade Manager : plutôt un lead qu'un Business Analyst."

Seniority flags and orders; it does not set the verdict.

Where DC versions disagree, show it with ? or inside the sentence when it changes the reading. Which file said what, how many versions exist and how complete they are is ledger business, not sales business, so it stays out of the file.

Then give each consultant one verdict, read off the core criteria:

- Bon fit: has done the core work hands-on, in a comparable context.
- Fit avec réserves: has done a large part of the core work hands-on, with one or two gaps outside the core (less seniority, a secondary criterion).
- À creuser: hasn't done the core work, but has done part of it, and one condition about the person could make it work, such as ramping up on a tool. When the fiche itself is ambiguous, say so in the Lecture du poste rather than reading it to fit a candidate.
- Pas pertinent: hasn't done the core work, and no condition would change that.

The verdict says how well someone fits. Separately, open Pourquoi with "Fit caché :" for someone whose experience fits but whose title, sector or wording wouldn't suggest it: the person a quick read of the fiche and the DC would pass over, and whose real experience is undersold on paper. This can happen at any level. The flag explains a verdict the core criteria already support; it does not raise one.

A consultant with no ledger gets "DC manquant" instead of a verdict. A fiche may fit few consultants, or none.

### 4. Output

The reply, in this order:

1. Lecture du poste: a short paragraph in plain language on what the job seems to actually be and what kind of profile the client seems to be looking for.
2. Ce que j'évalue: the grille, one line per criterion saying why it matters, core criteria marked, how seniority is read for this fiche, and a one-line legend for the marks.
3. En bref: a few lines on who stands out and why, and whether anyone fits at all.
4. The file.

The file is a spreadsheet holding only the ranked table (one tab per role when there are several); the grille stays in the reply. One row per consultant, everyone included:

| # | Consultant | Verdict | Pourquoi | Pourquoi pas | À condition que | Métier | <one column per criterion> | Séniorité |

- #: overall rank, as a whole number. Sort by verdict, then within a verdict by the core criteria, then by the other criteria and seniority.
- Pourquoi: the case for the person, in 2 to 3 sentences of plain French, the way a colleague would sum them up for this fiche. The readers are internal sales people, so no marketing tone. Describe; the sales person decides.
- Pourquoi pas: the real reason the person falls short of this job, in a sentence or two, rather than a list of what the DC doesn't mention.
- À condition que: filled for À creuser only, with the one condition that could make it work, for example "si le client accepte un profil Product Manager plutôt que Business Analyst". Availability, rate and location are the sales person's job.
- Métier: a few words.
- Criterion columns: named after the grille, each cell a mark and its sentence.

For the top matches, Pourquoi and Pourquoi pas can take one or two more sentences, non-technical and in plain language; for Pas pertinent, one short line each is enough. End the sheet at the last consultant, with no empty rows after it.

Write everything in French, the reply and the spreadsheet alike. Write it the way French tech and consulting teams actually talk: terms like backlog, product owner, delivery or run stay in English when that is what people say. Spell out role names rather than abbreviating them (Business Analyst, not BA; Product Owner, not PO). Plain language, no scores or percentages; the marks are the only scale.
