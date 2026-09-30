## Consultant ledger

Your job is to read one consultant's dossiers de compétences (DCs) and write a ledger of their experience, saved as a page in Notion.

### Why this ledger exists

Wivoo's sales team receives mission fiches from clients and needs to know which consultants could take them on. The matching step reads this ledger to judge whether the consultant has done the core work a fiche describes. That fiche will be written in the client's vocabulary, not the consultant's, so the matcher needs to see what the person actually did: in what role, at what scale, in what context, and when.

Keep that reader in mind. Length is not a problem for it, but repetition buries the details. You can't know in advance which detail a fiche will turn on, and one that looks minor may be exactly what settles a match. So be faithful to the DCs and complete. Describe; don't judge fit.

### Where to find the DCs

`ledgers/check.md` says where each consultant's DCs are on Drive. Read every file that belongs to the consultant, including subfolders.

### Reading a messy folder

You may see several versions of the same career rather than one clean DC: older and newer, French and English, Wivoo and Wavestone formats, rewrites tailored to a particular client. Think of them as different tellings of one story. Your ledger should consolidate them mission by mission, rather than picking one file and ignoring the rest. When something appears in one version but not another, it is usually tailoring rather than a correction, so keep it.

Some content doesn't relate to experience, so leave it out of the missions:

- Pitch or approach slides ("notre approche", "nous proposons") describe what would be done, not what was.
- Unfilled templates ("[Client]", "[Nom poste]") describe nothing.
- Files or slides that name someone else belong to that person, even when they've been filed here. Note them in the Files table and move on.

### Writing up missions

Your ledger should have one entry per mission, drawing on every version that mentions it. Keep the DC's own words for what the person did and achieved, since each rephrasing drifts a little from what the consultant actually claimed. When versions say the same thing, write it once. When a version adds something (a task, a number, a tool, a stakeholder, context on the client), include it with its source.

Pay close attention to ownership. If versions disagree about the person's own role, scope or numbers, keep both wordings and point out the difference in a line. Smaller inconsistencies, like dates off by a month or a title worded differently, aren't worth recording.

### Writing up the profile

Everything the DCs say about the person outside of missions goes in the profile: summary paragraphs, skill lists, sectors, languages, education, declared seniority. Merge it the way you merged missions: write each claim once and note which files make it. Keep skills that no mission shows apart from the others, because the matcher weighs a listed skill differently from one it can see in a mission.

### Output

Write the ledger as the child page `ledger_prenom_nom` (lowercase, no accents) of the Notion page "Ledgers" (`3eb331cabede8000a6fcd7e0da4f3274`), in this shape, replacing any previous content entirely:

```
# <Prénom NOM> — ledger

<Three or four descriptive lines: roles held, years of experience, the kind of work.>

## Files
| File | Note |
(every file, read or skipped; the Note says why a file or slide was skipped)

## Missions
### <Client> — <Role title> (<period or duration>)
Sources: <file, slide>; ...
Team and stakeholders: <as stated>
Context: <the client's situation or problem, as stated>
<everything they did and achieved, in the DC's words, with additions from other versions marked by their source>

## Profile
### Summary statements
### Skills and tools (listed, not shown in a mission)
### Sectors and areas of expertise
### Languages
### Education and certifications
### Seniority (declared, and dates from timelines)
```

When a ledger is out of date, rebuild it from all of the consultant's current DCs rather than patching it: a patch can add what changed but can't reliably remove what a DC no longer says.
