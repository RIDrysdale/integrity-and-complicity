# Decisions

Why the program is the way it is. Each entry records a decision, its reason, what it cost, and where the rule it produced now lives.

**This file does not govern anything.** The rule itself is stated in the document it governs (CHARTER, DESIGN-PRINCIPLES, ARCHITECTURE, WORKFLOW, READINGS, CASES, `notes/tensions.md`). If an entry here and a governing document disagree, the governing document is right and the entry is out of date.

**Entries are not rewritten.** When a decision is reversed or replaced, its status changes and it points to the entry that replaced it. A reversed decision keeps its entry, because the reason it failed is what stops it being proposed again.

**Read the index, not the file.** Open an entry only when the work touches it. `grep -n "Weber" DECISIONS.md` is cheaper than reading everything.

## Index

| ID | Date | Decision | Status |
|---|---|---|---|
| D-001 | 2026-09-20 | Organise by problems, not philosophers; eight core modules and three expansions | in force |
| D-002 | 2026-09-20 | Edition-independent locators; availability is a selection criterion; pointers | in force |
| D-003 | 2026-09-20 | CC BY-NC-SA 4.0 with an educational-use permission | in force |
| D-004 | 2026-09-20 | Module 1 slate: *Apology*, *Crito*, Rawls §§18–19, Arendt | in force |
| D-005 | 2026-09-20 | Module 1 revised after critique; no advance verdicts; writing optional | in force |
| D-006 | 2026-09-20 | No pre-judging readings; reader pass moved to the finished program | in force |
| D-007 | 2026-09-20 | Module 2 question restated around "a you apart from the roles" | reversed by D-011 |
| D-008 | 2026-09-20 | Applbaum dropped from Module 2 | in force |
| D-009 | 2026-09-20 | Module 2 pointers: Bradley and Weber | in force |
| D-010 | 2026-09-20 | Confucian texts do not meet design principle 8's test | in force |
| D-011 | 2026-09-20 | Module 2 question reverted; the closing's two tests withdrawn | in force |
| D-012 | 2026-09-20 | Apparatus points at the text rather than retelling it | in force |
| D-013 | 2026-09-20 | Module 2's candidate tensions refused | in force |
| D-014 | 2026-09-20 | *Bhagavad Gita* withdrawn from Module 2 | in force |
| D-015 | 2026-09-20 | Case defaults must be stated; no option is free | in force |
| D-016 | 2026-09-20 | Tensions may fall inside a single reading | in force |
| D-017 | 2026-09-21 | Cicero extended to III.43–58; Module 2's central overclaim corrected | in force |
| D-018 | 2026-09-21 | Principle 8 after the Module 2 rebuild | in force |
| D-019 | 2026-09-21 | Module 3 slate: Aquinas, *Avodah Zarah*, *Aṅguttara Nikāya* | in force |
| D-020 | 2026-09-21 | Havel dropped from Module 3; the fourth slot stands empty | in force |
| D-021 | 2026-09-21 | Module 3 does not discharge principle 8 | in force |
| D-022 | 2026-09-21 | T-004 admitted; two cross-reading tensions refused | in force |
| D-023 | 2026-09-27 | Keep a decision log; add CLAUDE.md and CHECKLIST.md | in force |
| D-024 | 2026-09-27 | Adopt a whole-program review method; run the first review | in force |

Entries D-001 to D-022 were reconstructed on 2026-09-27 from commit messages and from reasoning that had been kept in READINGS.md, ARCHITECTURE.md and `notes/tensions.md`. That reasoning was moved here, not rewritten.

## How to add an entry

Add an entry when a reading is assigned, dropped or withdrawn; when a claim about what a text establishes is made or withdrawn; when a tension is admitted or refused; when a case is placed or changed in substance; or when any governing document's rule changes. Wording fixes do not need one.

```
## D-NNN — Short statement of the decision
**Date:** YYYY-MM-DD · **Scope:** module or file · **Status:** in force | superseded by D-NNN | reversed by D-NNN
**Rule lives in:** file and section · **Commit:** short hash, if known

What was decided, in a sentence or two. Why. What it cost or ruled out.
```

Add a row to the index at the same time.

---

## D-001 — Organise by problems, not philosophers
**Date:** 2026-09-20 · **Scope:** program · **Status:** in force
**Rule lives in:** ARCHITECTURE.md · **Commit:** 5366216

Modules follow the arc of a situation (what binds me, what I owe, what I am part of, what I am not saying, where responsibility went, what I can do, what it will cost, what I live with) rather than a taxonomy of theories. Eight core modules make the program complete; three expansions are optional. Judgment under uncertainty and authority/law are deliberately not modules of their own, for the reasons ARCHITECTURE.md gives.

## D-002 — Locators, availability, pointers
**Date:** 2026-09-20 · **Scope:** program · **Status:** in force
**Rule lives in:** DESIGN-PRINCIPLES.md 9; WORKFLOW.md, Sourcing rules and Pointers · **Commit:** 5366216

Readings are cited by edition-independent locators, never page numbers. Whether a reader can obtain a text is a selection criterion. Works worth knowing but not worth assigning become one-paragraph pointers, at most two per module.

## D-003 — License
**Date:** 2026-09-20 · **Scope:** program · **Status:** in force
**Rule lives in:** README.md, License; LICENSE · **Commit:** 4da5126

CC BY-NC-SA 4.0 for the original text, with an added permission for educational institutions charging tuition. Cited readings are excluded.

## D-004 — Module 1 slate
**Date:** 2026-09-20 · **Scope:** Module 1 · **Status:** in force
**Rule lives in:** READINGS.md · **Commit:** 0af4290

Assigned the *Apology*, the *Crito*, *A Theory of Justice* §§18–19 and Arendt's "Personal Responsibility Under Dictatorship", with pointers to Nozick and to Rawls's 1964 fair-play essay. *A Theory of Justice* was corrected from free to library-only. Two of Module 1's four readings need a library; that is a cost against design principle 9, and later modules are expected to do better.

## D-005 — Module 1 revised after critique
**Date:** 2026-09-20 · **Scope:** Module 1 · **Status:** in force
**Rule lives in:** WORKFLOW.md, Drafting a module; `notes/tensions.md` header · **Commit:** 28b9383

Corrected a misstatement of Rawls's principle of fairness. Removed an unargued judgment that the workplace fails Rawls's justice condition. Qualified four attributions to Arendt. Removed advance verdicts on the readings' strength, which had the module converging on personal judgment as the answer. Made written exercises optional. Deleted the second tension, which set Arendt against a misuse of Rawls rather than against Rawls. That is the origin of the rule that a tension cannot be between a reading and a misuse of another.

## D-006 — No pre-judging; reader pass on the finished program
**Date:** 2026-09-20 · **Scope:** program · **Status:** in force
**Rule lives in:** WORKFLOW.md, Drafting a module; CHARTER.md, Standard of completion · **Commit:** ce8d225

Modules may not deliver advance verdicts on readings or position the last reading as the one that sees through the others. The reader pass became a requirement on the completed program read in sequence, not on each module. The charter states the cost: until then nothing has been read by anyone outside the drafting process.

## D-007 — Module 2 question restated
**Date:** 2026-09-20 · **Scope:** Module 2 · **Status:** reversed by D-011
**Rule lives in:** ARCHITECTURE.md, Module 2 · **Commit:** a13fa42

Restated as *What does a role make you owe — and is there a you apart from the roles?*, on the ground that the Confucian readings deny there are two separable things to compare.

## D-008 — Applbaum dropped from Module 2
**Date:** 2026-09-20 · **Scope:** Module 2 · **Status:** in force
**Rule lives in:** READINGS.md · **Commit:** a13fa42

Applbaum, *Ethics for Adversaries* (1999), was considered as a third pointer for Module 2 and dropped: Cicero holds the same position as an assigned reading, and the cap is two.

## D-009 — Module 2 pointers: Bradley and Weber
**Date:** 2026-09-20 · **Scope:** Module 2 · **Status:** in force
**Rule lives in:** READINGS.md; Module 2 · **Commits:** 9021c5c, 8ab7ac5

Bradley's "My Station and Its Duties" goes with the Confucian reading, to stop the constitutive view being filed as a foreign curiosity, and then to stop the opposite error. Not assigned: the module already holds the position.

Weber's "Politics as a Vocation" goes with Fried. It is an argument the program would like and cannot assign, for one reason: there is no English translation that is both reliable and freely available. An earlier draft also cited the absence of edition-independent locators, which will not bear weight — the lecture is a single identifiable work, and the program assigns a whole Montaigne essay on the same footing. An earlier draft of READINGS.md called it exactly the argument Case A.4 turns on, which would make it load-bearing and so disqualify it as a pointer under WORKFLOW; that claim is withdrawn, since the case and the module's closing carry the reckoning with consequences without it. If a sound free translation appears it should be reconsidered as an assigned reading.

## D-010 — Confucian texts do not meet design principle 8's test
**Date:** 2026-09-20 · **Scope:** Module 2; principle 8 · **Status:** in force
**Rule lives in:** ARCHITECTURE.md, What is not yet decided; READINGS.md, Traditions · **Commits:** 6ecaf67, 8ab7ac5

An earlier draft recorded the Confucian reading as having met design principle 8's test, on the ground that these texts contain no standard appealable against a relation. That was withdrawn as stronger than the assigned passages support. A second and weaker version — that obligations here cannot be stated without reference to roles — also fails, since 2A.6 does exactly that. What survives is a difference in where inquiry begins, which is real and does not meet principle 8's test.

**Lesson:** the claim was made twice, in a stronger and a weaker form, and both were withdrawn. Two later tests found no instance either (D-018, D-021). Before claiming that any reading reframes the question, CHECKLIST.md §B asks for the passage that shows it.

## D-011 — Module 2 question reverted; the closing's tests withdrawn
**Date:** 2026-09-20 · **Scope:** Module 2 · **Status:** in force
**Rule lives in:** ARCHITECTURE.md, Module 2 · **Commit:** 8ab7ac5

The question returned to *Do the obligations of a job, a profession, or a membership differ in kind from ordinary moral obligations?* The ground for restating it (D-007) was overstated, and the original wording never presupposed two selves — *they are inseparable* was always an available answer to it. The replacement also invited a question about personal identity that the module's readings cannot develop.

The closing's two discriminating tests were withdrawn. Both were unsound — an inculcated loyalty survives the dislike test, and conscience operates with no audience — and together they announced an editorial account of what makes conduct obligatory, which is the convergence the charter forbids.

## D-012 — Apparatus points at the text rather than retelling it
**Date:** 2026-09-20 · **Scope:** program · **Status:** in force
**Rule lives in:** DESIGN-PRINCIPLES.md 6 (the reader meets the text; the apparatus orients) · **Commits:** a960be0, 703b1c2

Module 2's apparatus had reached 10,584 words, and most of the excess was in "What to watch for", which had drifted into retelling the assigned passages closely enough that a reader could skip them. Rebuilt on the principle of pointing rather than retelling: 4,165 words to 3,039. Where the remaining length is one paragraph per cited passage, it can only come down by dropping passages.

## D-013 — Module 2's candidate tensions refused
**Date:** 2026-09-20 · **Scope:** Module 2; `notes/tensions.md` · **Status:** in force
**Rule lives in:** `notes/tensions.md` header · **Commits:** 8967a9d, cc4b6fd, 8ab7ac5

Five entries were drafted and cut to two by applying the file's own bar: one depended on the withdrawn Confucian claim (D-010), two depended on Analects 13.13 saying more than the module claims, one compared Montaigne against a misuse of his own language, and one asserted that the *Gita* attaches no condition, which 2.31 and 2.33 contradict.

The two survivors were then withdrawn as well.

The first set Cicero's duty of disclosure against Fried's location of the correction in the rules. It could not be shown that the two would decide the same case differently: Cicero offers a formulation and Fried denies that any rule resolves every borderline case, and those are not contrary answers.

The second set Mencius 4B.3 against Fried on whether how you are treated bears on what you owe. Fried's footnote 35 defeats it — the professional rules he relies on permit withdrawal where a client's own conduct makes representation unreasonably difficult, so the client's behaviour is among his conditions after all.

## D-014 — *Bhagavad Gita* withdrawn from Module 2
**Date:** 2026-09-20 · **Scope:** Module 2 · **Status:** in force
**Rule lives in:** READINGS.md, Traditions; OPEN-QUESTIONS.md · **Commit:** 7e6dc13

The entry made fixed station the reading's governing answer while its own assigned ending sets duty aside at 18.66, and repairing that needed more of chapter 18 and more room than a module of four other readings could give.

Withdrawing the *Gita* costs Module 2 the only role-obligation in it warranted from outside human arrangements, and the claim at 18.48 that no undertaking is free of defect. Nothing assigned there replaces either. Design principle 8 is a requirement on the finished program rather than on each module, so the loss falls due in Module 7, where whether the *Gita* belongs is an open question.

## D-015 — Case defaults must be stated; no option is free
**Date:** 2026-09-20 · **Scope:** CASES.md · **Status:** in force
**Rule lives in:** CASES.md (A.4); CHECKLIST.md §A · **Commits:** 9003e60, 7439e78, 8c8d9f8

Module 2's closing assumed the reader could do nothing and let the analyst's version go up, which the case never established. The case now states that the report goes into the pack over both names unless pulled, so inaction is a real option with the reader's name still on it. The covering-note option was a free solution until the report's second finding was made to dispute it. A prior verdict assigned to the reader was removed, since Module 1 let them reject it. The inaction test was corrected: a costless choice is not suspect in itself; what matters is whether it was made.

## D-016 — Tensions may fall inside a single reading
**Date:** 2026-09-20 · **Scope:** `notes/tensions.md` · **Status:** in force
**Rule lives in:** `notes/tensions.md` header · **Commit:** 95b1e58

What makes a tension is that the reader meets an unresolved conflict, not which covers it falls between. Admitted with a guard: where a text settles its own disagreement, the entry must say what survives the settlement, or every dialogue would qualify.

## D-017 — Cicero extended to III.43–58; Module 2's central overclaim corrected
**Date:** 2026-09-21 · **Scope:** Module 2 · **Status:** in force
**Rule lives in:** READINGS.md; Module 2; T-003 · **Commits:** 394f7f5, c85eee0

The Cicero assignment was extended from III.49–58 to III.43–58 after a later check. The module had been built on III.57, where concealment is defined as keeping people ignorant *emolumenti tui causa* — for the sake of your own gain. That leaves silence kept for somebody else's benefit outside the definition, which is the reader's own case and appeared to put Cicero at odds with himself. At III.43 he addresses acting for another directly, and the ruling is narrower than it first appears: failing a friend in what you may rightly do for him is itself a breach of duty, and friendship outranks honours and riches, but nothing may be done against the republic, an oath or good faith for a friend's sake — not even by a judge hearing that friend's case, who *ponit enim personam amici, cum induit iudicis*, and who may still set the hearing at his friend's convenience.

A first draft of the module read this as a general rule that office displaces relation, and used it to put Cicero and *Analects* 13.18 in direct contradiction. It will not bear that: the passage governs a verdict, not every office, and 13.18 contains no office at all. What the extension does supply is a concrete treatment of partiality that the module had been discussing without a text. The slate is four accounts of when a relation may move you, which is worth reading together; it is not four verdicts on one case, and the module no longer says it is.

The same correction removed an invented office of witness from 13.18, a Fried–Confucius alliance and a Cicero–Montaigne opposition, and rewrote T-003 with its qualification first.

## D-018 — Principle 8 after the Module 2 rebuild
**Date:** 2026-09-21 · **Scope:** principle 8 · **Status:** in force
**Rule lives in:** ARCHITECTURE.md, What is not yet decided · **Commit:** 394f7f5

Rebuilding Module 2 on Cicero III.43 moves this further the wrong way, and the cost should be recorded rather than absorbed. 13.18 now carries the module's central disagreement: the Duke of She's district holds Cicero's position and Confucius rejects it by name. That is a strong reading of the passage and a fair one, but it makes these texts a rival position inside the module's framing rather than a challenge to the framing. The module is better for it and principle 8 is worse off. Nothing in the program yet counts as an instance, and Module 7 now carries the whole of that debt.

## D-019 — Module 3 slate
**Date:** 2026-09-21 · **Scope:** Module 3 · **Status:** in force
**Rule lives in:** READINGS.md · **Commit:** 0f9ca5e

Assigned *Summa Theologiae* II-II q. 62 a. 7 and q. 78 a. 4, *Avodah Zarah* 6a–6b, and *Aṅguttara Nikāya* 4.201, 4.264, 5.177 and 6.63. All free, none needing a library. The Pali reading is assigned on design principle 1, not offered as principle 8's instance. The README describes the three as sorting the same acts by unrelated measures rather than as disagreeing, which is what the module and T-004 establish (be07777).

Case A.3 was considered for Module 3 and sent to E3: it supplies no second wrongdoer, so there is nothing to take part in.

## D-020 — Havel dropped; the fourth slot stands empty
**Date:** 2026-09-21 · **Scope:** Module 3 · **Status:** in force
**Rule lives in:** READINGS.md · **Commits:** 0f9ca5e, 911a5cf

Havel, "The Power of the Powerless" (1978), sections I–VII, was proposed for this slate and dropped. It is in copyright, the freely circulating PDF names no translator and carries no permission statement, and its scan is corrupt enough that nothing could be quoted from it. The drop costs the module the claim that going along with a practice constitutes it — that the greengrocer, who orders nothing, enables nothing, and could not change the outcome by withdrawing, is the system anyway. Nothing else on the slate makes that claim. *Staying* itself is still covered, by AN 5.177, which forbids a standing trade rather than an act; what is lost is the position that refuses the accounting altogether. The module was drafted with three readings and works with three, so the slot stands empty rather than filled.

La Boétie's *Discourse on Voluntary Servitude* is the nearest free candidate and was checked far enough to confirm that Part I holds the constitutive claim and Part III the hierarchy of beneficiaries; against it, its remedy is simply to stop, which is the one answer the charter's final clause removes. It remains available if a reader pass finds the module short of a text that declines to do the accounting at all.

## D-021 — Module 3 does not discharge principle 8
**Date:** 2026-09-21 · **Scope:** Module 3; principle 8 · **Status:** in force
**Rule lives in:** ARCHITECTURE.md, What is not yet decided · **Commit:** 0f9ca5e

Module 3 was tested as a home for principle 8's debt and does not discharge it. The strongest reframing candidate for that module's question is the Islamic duty of *al-amr bi'l-maʿrūf wa'l-nahy ʿan al-munkar*, commanding right and forbidding wrong, which grounds the obligation in having witnessed a wrong rather than in any connection to it, and so cuts across the whole list of modes the module works with. It cannot be assigned. Ghazali's treatment, *Iḥyāʾ* Book 19, has no complete free English translation — the Fons Vitae version is announced for 2027, and the substantial English is a partial translation inside Michael Cook's *Commanding Right and Forbidding Wrong in Islamic Thought* (2000). A single hadith is not a reading, and a tradition represented only by a pointer is not represented. The Pali reading earns its place on principle 1 and is not a substitute for it. Whether it also reframes is left to the drafting to show or fail to show; it is not claimed. Module 7 continues to carry the debt.

**Watch:** the Fons Vitae translation of *Iḥyāʾ* Book 19. If it appears and is obtainable, this entry's reason for not assigning lapses.

## D-022 — T-004 admitted; two cross-reading tensions refused
**Date:** 2026-09-21 · **Scope:** Module 3; `notes/tensions.md` · **Status:** in force
**Rule lives in:** `notes/tensions.md` · **Commit:** 1d7bcc3

T-004 records the two reasons at *Avodah Zarah* 6a for one prohibition; 6b and 7a were checked and the Gemara does not return to it. Two cross-reading entries were refused. Aquinas against AN 4.264 on praising a theft one did not cause fails because his article computes restitution and is silent on culpability, so the texts return different figures for different quantities rather than disagreeing. Aquinas against *Avodah Zarah* on necessity fails because they reach the same conclusion by different routes.

## D-023 — Keep a decision log; add CLAUDE.md and CHECKLIST.md
**Date:** 2026-09-27 · **Scope:** process · **Status:** in force
**Rule lives in:** WORKFLOW.md, What gets recorded

WORKFLOW.md previously ruled out a decision log, on the ground that a rule recorded in two places will eventually disagree with itself. In practice the reasoning did not disappear. It went into the governing documents, where about two-fifths of READINGS.md had become a history of what was dropped and why, and every session had to read it to find the current state. It also went into commit messages, which record it well but cannot be consulted cheaply.

The objection is met by making this file non-governing. It records why and points to where the rule lives, and it never restates the rule. The reasoning that had accumulated in READINGS.md, ARCHITECTURE.md and `notes/tensions.md` was moved here in the same change, so those files now state only the current position.

CLAUDE.md was added so that each working session starts from a short orientation and loads only what its task needs. CHECKLIST.md turns the principles, together with the defects the history shows recurring, into questions to run at each stage.

## D-024 — Adopt a whole-program review method; run the first review
**Date:** 2026-09-27 · **Scope:** process · **Status:** in force
**Rule lives in:** `review/METHOD.md`

At Robert's request, a method for re-examining the whole program rather than one part: decompose the problem into independent chunks, analyse each in parallel with a separate agent that writes from first principles before reading the program, merge, verify the merge with another agent, then act only through Robert. The first run (`review/2026-09-27-reevaluation/`) found the core design sound and the program written for a narrower reader than it names, never tested on one. Its verification step required 14 corrections to the first synthesis, mostly citations stronger than their findings, which is the defect CHECKLIST.md lists first. Its recommendations are pending in OPEN-QUESTIONS.md; this entry records only that the review was run, not that anything in it was adopted.
