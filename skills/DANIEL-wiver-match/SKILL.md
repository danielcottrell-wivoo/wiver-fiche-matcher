---
name: wiver-match
description: Match a Wivoo mission fiche against the consultants in intermission, using their dossiers de compétences on Drive. Use when a sales person shares a fiche de poste, appel d'offres or mission description and wants to know which consultants could take it.
---

## Fiche match

Given a mission fiche and the consultants in intermission, produce a table telling a Wivoo sales person how each consultant relates to the mission. The reader skims many fiches a day and has a decent sense of the who's who at Wivoo. Help them judge quickly and honestly; do not decide for them, and do not burden them with noisy outputs.

Each consultant has a folder in the Drive folder "DC- Consultants Wivoo" (`149FelJQXXY6lZSE40By4D-ApIldqYSJp`), named roughly "DC - Prénom NOM". The folder holds their DCs and a `ledger.md`: a complete record of what their DCs say, written for you to match against.

### 1. Ledgers

For each name, find the folder and list its files. If there is no `ledger.md`, or any other file was modified after it, rebuild it by following `ledger-builder.md`. Then read `ledger.md`.

### 2. Read the fiche

Fiches are dense and written in the client's vocabulary, and their title does not always match the work. Work out the core work of the job: what the consultant will actually do day to day. Tools, sector and education listed in the fiche are secondary.

### 3. Judge each consultant

Go through the consultants one at a time and ask: has this person done the core work of this job?

- Missions in the ledger are the evidence; the profile tells you what the person claims.
- Judge the work, not titles, keywords, tools or sector. Someone who did the work with other tools fits.
- A shared sector is a plus.
- Where DC versions disagree, mention it when it bears on this match.

Give each consultant one verdict:

- Fort: has done the core work.
- À regarder: has done part of the core work.
- Outsider: has done the core work under another title, in another setting, or in words the fiche does not use, so it does not show on paper. Name that mission. These are the people a sales person is most likely to miss.
- Pas pour cette mission: has not done the core work.

A fiche may fit few consultants, or none.

### 4. Output

Write a spreadsheet with one row per consultant, everyone included, sorted Fort, À regarder, Outsider, Pas pour cette mission:

| Consultant | Verdict | Pourquoi | Métier | Secteur | Séniorité | Question à poser |

- Pourquoi: one line linking the core work of the job to what the person did.
- Métier, Secteur, Séniorité: a few words each.
- Question à poser: at most one, about something the ledger leaves open on the core work and that could change the verdict. The sales person handles availability, rate, location and fit with the team themselves.

In the reply, open with a short paragraph in plain language on what the job seems to actually be and what kind of profile the client seems to be looking for, then give the file.

Write everything in French, the reply and the spreadsheet alike. Write it the way French tech and consulting teams actually talk: terms like backlog, product owner, delivery or run stay in English when that is what people say. Plain language, no scores or percentages.
