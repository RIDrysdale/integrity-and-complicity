# Working on this repository

An applied-ethics reading program on acting with integrity inside compromised institutions. It has eight core modules, and Modules 1 to 3 are drafted. The central question and the reader it is written for are in CHARTER.md. Every change answers to that.

Robert Drysdale decides. Claude drafts. ChatGPT critiques. Claude does not settle open editorial questions or change the architecture through a drafting choice. A structural proposal is made explicitly, to Robert.

## Start of every session

1. Read the **index** at the top of DECISIONS.md, not the whole file. Open individual entries only when the work touches them.
2. Read OPEN-QUESTIONS.md. It is short.
3. Then load only what the task needs. Use the table below.

The repository is about 30,000 words, and most tasks need less than a third of it. Do not read the modules in full unless the task is one of them.

## What to read for which task

| Task | Read | Usually skip |
|---|---|---|
| Drafting a new module | CHARTER, DESIGN-PRINCIPLES, that module's entry in ARCHITECTURE, its case in CASES, READINGS, CHECKLIST, and the closing sections ("Returning to the case", "What this module did not settle") of the module before | Earlier modules' reading entries |
| Revising a reading entry | That entry, its READINGS row, any T- entries naming it, CHECKLIST §C, and `grep` DECISIONS.md for the author | Other modules |
| Assessing a candidate reading | DESIGN-PRINCIPLES 1, 8 and 9, READINGS, CHECKLIST §B, and `grep` DECISIONS.md for the author | Modules |
| Proposing a tension | The `notes/tensions.md` header, the passages concerned, and D-013 and D-022 | Other tensions |
| Anything touching principle 8 | D-010, D-018, D-021, and ARCHITECTURE, What is not yet decided | — |
| A question about process | WORKFLOW | — |

## Where things are recorded

- **The rule** lives in the document it governs, and in one place only. WORKFLOW.md, "What gets recorded", says which document governs what.
- **Why** it is that way goes in DECISIONS.md. Add an entry and an index row whenever you make a decision of the kinds listed there.
- **What is unresolved** goes in OPEN-QUESTIONS.md. Delete an entry when it is answered.
- **What to check** is in CHECKLIST.md. Run the section for the stage you are at before calling anything done.

This file is orientation. It states no rules of its own. If it disagrees with a governing document, the governing document is right; fix this file.

## Things that are easy to get wrong here

- Reader-facing prose in `modules/` carries no status notes, verification caveats or process notes. See WORKFLOW, Reader-facing prose is clean.
- Nothing is quoted or located that has not been checked. An unchecked locator is omitted, not guessed. See WORKFLOW, Sourcing rules.
- The commonest defect in this project's history is claiming more than a passage says. See CHECKLIST, What goes wrong most often.
- Pushing publishes, because the repository is public. See WORKFLOW, Publication.
