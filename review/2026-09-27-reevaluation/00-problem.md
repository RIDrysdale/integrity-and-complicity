# Re-evaluation, 2026-09-27: problem and decomposition

Method: `review/METHOD.md`. Orchestrated by Claude at Robert's request; four analysis agents, one verification agent.

## The big problem

> Design a reading program for an adult interested in applied ethics, specifically ethics inside a compromised system: someone who lives or works within an institution that is compromised, dysfunctional, unjust or corrupt, who is often dependent on it, implicated in it and benefiting from it, who is rarely certain they are right, and for whom leaving is impractical or undesirable. The program should leave them better able to think about, and act in, that situation.

That is the problem as a reader would put it. It deliberately does not say how the current program answers it: eight modules, anchor cases, classical texts and so on. Whether those answers are right is what the review is testing.

**State of the program at the start of this review:** Modules 1 to 3 of 8 are drafted. Nothing has been tested on a reader. About 35,000 words sit in the repository.

## Decomposition

Four chunks, each answerable without the others.

| # | Chunk | The question | Could come back "wrong" because… |
|---|---|---|---|
| 01 | Reader and outcomes | Who concretely is this for, and what should they be able to do afterwards that they could not before? How would anyone know whether the program achieved it? | The program may be written for a reader other than the one it names, or have no testable outcome at all. |
| 02 | Problem map | What are the parts of the problem of acting inside a compromised system, and in what order does a person meet them? | The eight-module carving may omit a part, split one part in two, or follow a discipline's order rather than the reader's. |
| 03 | Literature and access | What is the best material on this problem, across philosophy, the social sciences, history, literature and traditions outside the West, and what can a reader actually obtain? | The slate may be missing central work, and the rule preferring free texts may systematically exclude part of the field. |
| 04 | Form and load | Is the module form the right vehicle for a self-directed adult? That form is: a case first, three or four readings chosen to disagree, commentary, questions, and a return to the case. How much does it ask of the reader? | The form may be too heavy to complete, or may fit a seminar better than a person reading alone. |

The build process (drafting, verification, critique) was examined earlier the same day; see DECISIONS.md, D-023, and CHECKLIST.md. It is left out here, and the merge takes those findings into account.

## Rules for every agent

Follow `review/METHOD.md` §2 exactly.

- Write the **First principles** section before reading CHARTER, ARCHITECTURE, DESIGN-PRINCIPLES, READINGS, CASES or `modules/`. You may read this file and METHOD.md first.
- Label findings Evidence or Judgment, with confidence.
- Mark anything you could not verify.
- Write only to your own file.
- Keep the report under 2,000 words, with a Summary of 150 words or fewer.
