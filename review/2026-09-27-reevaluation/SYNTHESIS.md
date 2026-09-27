# Synthesis

Merge of chunk reports 01–04 (`review/METHOD.md` §3). Each claim cites the finding it rests on, with that finding's own label: **01-F3 (J, med–high)** means report 01, finding 3, a Judgment of medium-to-high confidence; **E** marks Evidence. Where the synthesis goes beyond any finding, the text says so.

This is the corrected version. The first draft was checked in VERIFICATION.md, which required 14 corrections. The draft mis-cited four findings. It presented judgments as evidence. It offered an inference of the orchestrator's own as a convergence between chunks. And it dropped findings that cut against its framing. All 14 are applied here.

The four agents and the orchestrator are drawn from one model family. Agreement between them is weak evidence, and it is weakest where they shared a premise.

## Verdict

The core design holds. Carrying the arc in escalating cases and the concepts in modules is sound (02-F7, J med). The form suits a reader working alone better than predicted (04-F6, J med–high). The classical texts suit this reader (03, Balance). The guard against self-justification and heroism is stronger than a first-principles design produced (01-F6, E+J high).

The problems are of two kinds.

1. **Nothing has been tested on a reader, and nothing states what reading should achieve** (01-F1 E high; 01-F2 E high).
2. **The program is written for a narrower reader and problem than it names.** It assumes one office professional with library access, reasoning alone with argumentative texts, who has already noticed a wrong (01-F3 J med–high; 02-F3 J med–high; 02-F4 E high / J med). Several other findings are consequences of that picture. In the orchestrator's judgment, the rest are independent problems of load and access (04-F1–F3, 04-F7, 03-F3), plus the architecture's gap on those harmed (02-F2, 02-F5).

Most fixes are cheap because Modules 4 to 8 are unwritten.

## Where the chunks converge

### 1. No reader test before completion; no stated outcome
01-F2 (E high) and 04-R5 both find that no reader test is planned until the program is finished: the only one is Robert's read-through (D-006). 01-F1 (E high) alone finds that no outcome is stated anywhere, so that nobody could tell whether the program worked. The charter names the cost itself: an error in the form "would be repeated across every module before anyone noticed."

### 2. A narrower reader than the one named
- **The reader.** 01-F3 (J med–high) finds the program written for a graduate office professional with library access. The charter's church, school and community organisation appear nowhere in the modules or cases (verified by grep). 01-F4 (J med) adds that the recurring case limits who can use the program, "though less than it seems": some readers can transpose it and others cannot.
- **Collective action.** 02-F3 (E high that it is absent; J med–high that it is a gap) finds every response an individual's. ARCHITECTURE line 89 does acknowledge that the carving assumes "an individual agent deciding", but no entry records collective action as considered and left out.
- **Kinds of text.** 03-F1 (E high) finds no empirical work, testimony or literature assigned, and no decision on genre. 03-F4 (J low) suggests the cause is that the form is built around texts that argue.

*Orchestrator's judgment:* these three are one narrowing seen from three sides, and it looks inherited rather than chosen. No finding establishes that.

### 3. The positions record
04-F4 (E high) and 04-F5 (J high) find that comparing positions across modules is "part of the point", yet it rests on memory alone. Module 3's case itself says the remembered version "has been improving". A one-page record would give the comparison somewhere to live (04-R2). 01-F9 (E med) adds that this before-and-after comparison measures *change* in judgment, not improvement, on a case the reader has already seen. The record serves the reader. It is not by itself a test of the program; for that, 01-R1 uses an unseen case.

## Orchestrator's inference: drift and the sourcing rule

This is the orchestrator's inference from two separate findings. No chunk made it, and it has not been tested.

- 02-F4 (E high for placement; J med for the conclusion): the charter's example of "a culture that slowly shifts what everyone treats as normal" has its only home in Module 8. Noticing a wrong has no designated home; Arendt in Module 1 partly touches it.
- 03-F2 (E med, from a map built largely from memory): none of the 20 empirical works mapped would pass a strict free-and-locatable test. Design principle 9 itself says "prefer", and allows in-copyright work where there is no substitute. 03-F3 (E high for the texts; J med that it is drift) finds that practice has tightened toward the strict version.

**The inference:** the part of the problem the architecture reaches last is the part whose best literature the program's practice keeps out. If that is right, fixing either alone would leave the gap. Moving drift earlier without evidence to read would leave it thin. Admitting evidence without moving drift would put it at the end. It is offered as a reason to take 02-R3 and 03-R1 together, not as a finding.

## Questions for Robert

**A. Access against completion.** 03-R2 proposes restating principle 9 as a budget, for example one library-only text per module, and then *re-weighing* Havel and Weber. Havel was dropped for an unreliable copy as well as for copyright (D-020), so a budget alone would not readmit him. On the other side, 04-F9 (J med) predicts that Module 1's first library-only text is the likeliest place a reader stops, and 01-F3 counts library access as part of what narrows the reader. Recommendation 16's Ghazali candidate is in copyright (03-F10), so it depends on how this is decided.

**B. Those harmed, against load.** 02-F1 (E high / J high) and 02-F2 (E high / J med) find the gap flagged in two module closings, with no reason recorded for leaving it optional. 02-R1 offers three options:

- (a) a ninth module, which adds the most load and moves the completion line;
- (b) an outward-facing brief for an unwritten Module 5 or 7, which is cheap but "risks being flagged again rather than filled";
- (c) merging Modules 4 and 6 and using the freed slot, which adds no module but means editing Module 3's hand-off.

The program is estimated at 45 to 55 hours already (04-F2, J med; the hours are estimates).

**C. When to test on readers.** Two options:

- 01-R1: pilot Module 1 now with five to eight readers across the charter's settings, using an unseen before-and-after case.
- 04-R5: a cheaper timed test of Module 1 or 2 on one outside reader.

Both test the form. The D-006 pass tests the sequence, which is a different test. D-006 deliberately held reader testing back until the program is finished, so this revisits a recorded decision.

**D. Literature.** 03-F4 (E med) finds that nine free, chapter-locatable literary works were never considered. 03-R5 notes the cost: the "What kind of argument this is" apparatus does not fit fiction, and it adds load. No chunks conflict on this. It is simply undecided and unrecorded.

## Recommendations

Nothing here has been applied.

### Tier 1: cheap, no change to the architecture
1. **State the time** each module and the whole program take, after an honest recount of the primary texts (04-R1). 04-F11 (E low) suggests the stated times for Montaigne and the suttas may be low.
2. **Add a one-page positions record**, with each closing quoting back the earlier module's options (04-R2). Writing stays optional. It touches the charter's framing, so Robert decides.
3. **Mark one question per reading** as the one to answer if nothing else (04-R3).
4. **Add a signpost for a reader in difficulty now**, listing *kinds* of help and naming no body that has not been checked (01-R3, 01-F5 E high).
5. **Add one sentence in Module 1** saying that relief and remainder come later, in Module 8 (01-R5, 01-F7 J med). The report has low confidence this helps; a pilot would show.
6. **Add a check for time and commentary-to-text ratio** to CHECKLIST §D (04-R4). D-012's figure of 3,039 words is out of date: "What to watch for" in Module 2 is now about 3,413 words (VERIFICATION).
7. **Restate ARCHITECTURE's organising logic:** cases carry the arc, and modules carry the concepts (02-R5).
8. **Record why Kutz (2000) and Lepora and Goodin (2013) are not in Module 3**, or add one as a pointer (03-R7, 03-F6).
9. **Correct CHARTER line 23.** It says "Written exercises are offered", but the modules contain only suggestions to write (04-F10, E high). This is a small correction under METHOD §5, but the wording is Robert's.

### Tier 2: structural decisions for Robert
10. **Test on readers now:** 01-R1 or the cheaper 04-R5 (question C).
11. **State four to six program outcomes in CHARTER**, naming capacities rather than conclusions (01-R2).
12. **Move drift earlier:** place A.2 in Module 4 or 5, and leave Module 8 with endurance and aftermath (02-R3). Whether noticing also needs a home is open; 02 lists it as unplaced but does not recommend one.
13. **Decide whether Modules 4 to 6 teach any empirical evidence.** If they do, the cheapest vehicle is a short sourced paragraph held to the pointer standard (03-R1). Of all the recommendations, this is the one most likely to change what the program is.
14. **Put those harmed on the core path**, choosing among 02-R1's options (question B).
15. **Write collective action into Module 6's brief, and probably Module 5's** (02-R2).
16. **Decide the reader question.** Either narrow the charter, or widen the cases and add one prompt per module to put the reader's own situation in the case's place, with a caution against writing down real specifics (01-R4).
17. **Restate principle 9 as a budget, or keep it strict** (03-R2; question A).

### Tier 3: carry into drafting Modules 4 to 8
18. **Write Case C before Module 4** (02-R4). This is already an open question.
19. **Test the principle 8 candidates** as each module is drafted:
    - *Shabbat* 54b–55a (Module 4);
    - Mencius 5B1 with *Analects* 18.1 (Module 6);
    - *Zhuangzi* ch. 4 (Module 6 or 8);
    - Bhishma Parva §43 with Ghazali, *Iḥyāʾ* Book 14 (Module 7). Ghazali is in copyright and depends on question A.

    All are low-to-medium confidence and none has been passage-tested (03-R3). The project has made and withdrawn a claim of this kind before, in two forms (D-010). Robert must also rule on whether the Talmud counts as outside the Western canon (03-F7).
20. **Consider free public-inquiry reports as case sources**: TRC vol. 4, Francis 2015, and Horizon (03-R4). Whether they include people who stayed and were right is not checked; Horizon volume 1 covers impact and redress.
21. **Add Zheng (2018, CC-BY) to Module 5's candidates** (03-R6).

## Where the program does well

Recorded so that the list of problems is not mistaken for the whole picture.

- **Guarding against the self-justifying reader and the heroic reader** (01-F6).
- **The form for a solo reader** (04-F6).
- **The two-axis design** (02-F7).
- **The classical texts** (03, Balance).
- **Keeping E1 as an expansion** is defensible (02-R6).
- **The outcomes it already serves.** The drafted modules serve three of 01's seven proposed outcomes strongly and one partly (01-F10).

## What this review did not do

- It tested nothing on a reader. Every judgment about readers is a model's prediction.
- The primary-text lengths and hours in 04 are estimates, because the source sites were blocked.
- 03's map is largely from memory. VERIFICATION saw only search listings and snippets for the bibliographic claims; Sefaria, ctext.org and the primary pages were blocked.
- No candidate reading was put through CHECKLIST §B.
