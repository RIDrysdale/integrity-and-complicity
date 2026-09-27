# Whole-program review: method

How to step back and re-examine the whole program rather than one module. Use it when the question is *is this the right program?*, not *is this entry right?* Run it rarely: after the core path is drafted, after a reader pass, or when something structural looks wrong.

```
Big problem → Decompose → Analyze each chunk (in parallel) → Merge → Verify → Act
```

## 1. State the problem

Write the problem in the review's `00-problem.md` as the reader would put it, not as the program currently frames it. Then decompose it into chunks.

A good chunk:

- **can be answered without the others' answers.** If chunk B needs chunk A's conclusion, merge them or run them in sequence.
- **has a question that could come back "the current program is wrong here."** A chunk that can only confirm is not worth running.
- **is small enough for one agent to finish in one sitting** and report in under 2,000 words.

Three to five chunks. More than that and the merge becomes the bottleneck.

## 2. Analyze each chunk

Each chunk goes to a separate agent with a brief in `00-problem.md`. Every agent follows the same rules.

1. **Write from first principles before opening the program.** Answer the chunk's question from the problem statement alone, and save that section before reading CHARTER, ARCHITECTURE, READINGS or the modules. This is the check against anchoring: the existing design cannot shape an answer that was written before it was seen.
2. **Then compare with the program.** Say where the program agrees with the first-principles answer, where it departs from it, and whether the departure is a considered choice (look in DECISIONS.md) or an unexamined one.
3. **Label every finding** as **Evidence** (something checkable: a count, a quotation, a bibliographic fact, a file and line) or **Judgment**, with confidence: high, medium or low.
4. **Say what was not checked.** An unverified bibliographic detail is marked unverified, never guessed. This is the program's own sourcing rule (WORKFLOW, Sourcing rules).
5. **Write only to the chunk's own file.** Edit nothing else. Reviews propose; they do not change governing documents.

Each report uses this form, so the merge can read the top section first and stop there if it needs to.

```
# NN — Chunk name
## Summary            (≤150 words: the three to five findings that matter most)
## Question
## First principles   (written before reading the program)
## Comparison with the program
## Findings           (numbered; each labelled Evidence/Judgment and high/medium/low)
## Recommendations    (ranked; each with what it would cost)
## Not checked
```

## 3. Merge

The orchestrator reads every Summary first, then the Findings, and opens the rest only where reports conflict or a finding looks load-bearing. `SYNTHESIS.md` records:

- where chunks **converge.** Agreement between agents drawn from one model is weak evidence, because they share blind spots. Convergence counts for more when the agents reached it from different starting points.
- where chunks **conflict,** stated as the question Robert has to decide.
- **recommendations,** each tagged with the chunk findings it rests on.

## 4. Verify

A separate agent checks `SYNTHESIS.md` against the chunk reports and the repository.

- Does every claim trace to a finding?
- Did any Judgment get promoted to Evidence on the way?
- Is any recommendation stronger than its findings support?
- Spot-check at least five bibliographic or availability claims against their sources.

Findings go in `VERIFICATION.md`, and the synthesis is corrected before anyone acts on it.

## 5. Act

A review does not change the architecture by itself (CHARTER, Editorial authority).

- Structural proposals go to Robert explicitly, as options with costs.
- Questions he has not decided go into OPEN-QUESTIONS.md.
- What he decides goes into the governing document, with a DECISIONS.md entry that cites the review.
- Small corrections the review turns up (a broken link, a wrong count) can be fixed directly, as normal work.

## Record

Each review lives in its own dated directory under `review/`. The reports are kept, because the synthesis cites them and a later review should be able to see what an earlier one missed. They are working documents and are never cited to a reader.
