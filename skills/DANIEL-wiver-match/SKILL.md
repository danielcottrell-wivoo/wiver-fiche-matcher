---
name: wiver-match
description: Match a Wivoo mission fiche against the consultants in intermission, using their dossiers de compétences on Drive. Use when a sales person shares a fiche de poste, appel d'offres or mission description and wants to know which consultants could take it.
---

## Fiche match

Given a mission fiche and the consultants in intermission, produce a table telling a Wivoo sales person how each consultant relates to the mission. The reader skims many fiches a day and has a decent sense of the who's who at Wivoo. Help them judge quickly and honestly; do not decide for them, and do not burden them with noisy outputs.

Each consultant has a folder in the Drive folder "DC- Consultants Wivoo" (`149FelJQXXY6lZSE40By4D-ApIldqYSJp`), named roughly "DC - Prénom NOM". The folder holds their DCs and a `ledger.md`: a complete record of what their DCs say, written for you to match against.

### 1. Ledgers

For each name, find the folder and list its files. If there is no `ledger.md`, or any other file was modified after it, rebuild it by following `ledger-builder.md`. Then read `ledger.md`.

### 2. Read the fiche and set the grille

Fiches are dense and written in the client's vocabulary, and their title does not always match the work. Work out the core work of the job: what the consultant will actually do day to day. Tools, sector and education listed in the fiche are secondary.

Every fiche implies a grille: the few things that decide who can do this job. Make it explicit with 3 to 6 criteria, or more if you judge it necessary. Phrase each one as work to have done, not as keywords or tools, and give it one line on why it matters here. Mark which criteria are core: they decide the verdict, while the others only order people within a verdict. Sector, or prior work at this client, becomes a criterion only when the fiche makes it matter. Seniority is always assessed, separately.

### 3. Judge each consultant

Go through the consultants one at a time and fill in the grille.

- Missions in the ledger are the evidence; the profile tells you what the person claims.
- Judge the work, not titles, keywords, tools or sector. Someone who did the work with other tools fits.

Each criterion gets a mark, then one sentence saying what the person's experience means for that criterion, in words the sales person could repeat to the client. The sentence interprets; it does not list activities.

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

Where DC versions disagree, show it with ? or inside the sentence when it changes the reading. Sources and DC versions stay out of the table.

Then give each consultant one verdict, read off the core criteria:

- Fort: has done the core work.
- À regarder: has done part of the core work.
- Outsider: has done the core work under another title, in another setting, or in words the fiche does not use, so it does not show on paper. These are the people a sales person is most likely to miss.
- Pas pour cette mission: has not done the core work.

A consultant with no ledger gets "DC manquant" instead of a verdict. A fiche may fit few consultants, or none.

### 4. Output

The reply, in this order:

1. Lecture du poste: a short paragraph in plain language on what the job seems to actually be and what kind of profile the client seems to be looking for.
2. Ce que j'évalue: the grille, one line per criterion saying why it matters, core criteria marked, and how seniority is read for this fiche.
3. A one-line legend for the marks.
4. The file.

The file is a spreadsheet with one row per consultant, everyone included, ranked:

| # | Consultant | Verdict | Pourquoi | À condition que | Métier | <one column per criterion> | Séniorité |

- #: overall rank. Sort by verdict, then within a verdict by the core criteria, then by the other criteria and seniority.
- Pourquoi: 2 to 3 sentences in plain French, the way a colleague would sum the person up for this fiche. The readers are internal sales people, so no marketing tone.
- À condition que: usually empty. Fill it only with the one condition that could change the verdict, for example "si le client accepte un profil Product Manager plutôt que Business Analyst". Availability, rate and location are the sales person's job.
- Métier: a few words.
- Criterion columns: named after the grille, each cell a mark and its sentence.

Write everything in French, the reply and the spreadsheet alike. Write it the way French tech and consulting teams actually talk: terms like backlog, product owner, delivery or run stay in English when that is what people say. Spell out role names rather than abbreviating them (Business Analyst, not BA; Product Owner, not PO). Plain language, no scores or percentages; the marks are the only scale.
