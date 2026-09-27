# Checklist

Questions to run at each stage of the work. Each one points to the rule or decision behind it. The rule governs, and this file only prompts. If an item here and a governing document disagree, fix this file.

An item is passed when you can answer it in a sentence, citing the passage or line concerned. "Yes, I think so" is not a pass.

## What goes wrong most often

The history shows four defects recurring more than any others. Look for them first, at every stage.

1. **Saying more than the passage says.** This is the commonest defect. Two readings were claimed to contradict when they answer different questions (D-017). The Talmud was credited with a ruling on the severed limb that the assigned passage does not contain (8f815eb). A reading was claimed to meet principle 8 three times, and each claim was withdrawn (D-010, D-018, D-021). Five tensions were drafted and none survived (D-013).
2. **The apparatus doing the reading for the reader.** "What to watch for" drifts into retelling the passage until the text can be skipped (D-012).
3. **Convergence by the back door.** This covers an advance verdict, a closing test that amounts to an editorial answer, or a final reading placed to see through the others (D-005, D-006, D-011).
4. **Stale cross-references.** A change is made in one place and left false in another. Module 2's opening kept asserting a thesis after the entry withdrew it (ec9aa9a), and Module 3's handoff was made false by a later edit (911a5cf).

---

## A. Placing or changing a case

- [ ] What happens if the reader does nothing? The case text must say so, not the closing (D-015).
- [ ] Does every listed option cost something? An option that solves the case for free has to be removed or given a cost (D-015).
- [ ] Does the case assign the reader a view they held earlier? It must not, if an earlier module let them reject that view (D-015).
- [ ] Is the reader dependent, implicated, or benefiting? The charter's final clause asks for all three somewhere in the program (CHARTER).
- [ ] Does the "I don't know" option come with a date that forces a decision anyway (principle 4)?
- [ ] Is this case gray, or clear and merely costly? Say which (principle 5). The program still owes Case B (clear and costly) and Case C (the objector was wrong). See OPEN-QUESTIONS.md.

## B. Admitting a candidate reading

- [ ] Finish this sentence: *after this reading the reader can reason about ___ in a way they could not before.* If the answer is "know what X thought", the reading fails principle 1.
- [ ] Can the reader get it? Free and durable, or held by libraries with no free substitute, and the limitation stated (principle 9).
- [ ] Does it have an edition-independent locator system (principle 9; WORKFLOW, Sourcing)?
- [ ] Put it and one other slate reading to this module's case. Would they say different things? If not, it may be decoration (principle 2; `notes/tensions.md` header).
- [ ] Is it from outside the Western canon? If so, which does it do: *another answer*, or *a sign the question is wrongly posed*? Claim the second only if you can quote the assigned passage that shows it. Read D-010, D-018 and D-021 first (principle 8).
- [ ] Are the premises kept intact, or has it been secularised to fit (principle 8)?
- [ ] Has the work been assigned before? If so, does it take its own passages and its own question, and is this its second module at most (WORKFLOW, Recurrence)?
- [ ] Should this be a pointer rather than an assignment? If the argument cannot be compressed into one paragraph without damage, it is load-bearing and needs an assignable text (WORKFLOW, Pointers).
- [ ] Search DECISIONS.md for the author. Has this work already been considered and dropped?

## C. Drafting a reading entry

- [ ] Was every locator opened, every quotation taken from a text with a live link, and the READINGS.md status updated to match (WORKFLOW, Sourcing and Verification)?
- [ ] For every sentence of the form *the text says / holds / shows*, point to the passage. If you cannot, cut the sentence or turn it into a question (failure 1).
- [ ] Could a reader skip the text and still answer "Questions to carry" from the entry alone? If so, "What to watch for" is retelling rather than pointing (D-012).
- [ ] Is each reading set against another reading, or against a misuse of one? Only the first counts (D-005, D-013).
- [ ] Which reading does the draft treat most gently? Turn the sharpest question on it (WORKFLOW, Drafting a module).
- [ ] Does anything tell the reader, before they read, which argument is stronger (D-006)?

## D. Closing a module

- [ ] Are the four module conditions in CHARTER's standard of completion met?
- [ ] Are both of principle 3's questions asked, and worded differently from the previous module's version?
- [ ] Does the closing make the reader decide something concrete by a date in the case (principle 4)?
- [ ] Does any test, criterion or summary in the closing amount to the editors' answer (D-011)?
- [ ] Is the module consistent with itself? Check that writing is optional everywhere (Module 3's closing once said "keep what you wrote"), and that the handoff to the next module is still true.
- [ ] How long is it? Modules 1 to 3 run 3,538, 9,293 and 6,788 words. If a new module is longer than the one before it, be able to say what the extra length does for the reader.
- [ ] Have you read it through once, start to finish, as a reader, in one sitting? That pass found three defects in Module 3 that no section-by-section review had caught (8f815eb).
- [ ] Has each candidate tension been admitted or refused against the file's test? Record the refusals in DECISIONS.md, as D-013 and D-022 do.
- [ ] Is the README entry updated, and does its blurb claim no more than the module establishes (D-019)?

## E. After any change

- [ ] Grep the repository for the changed claim's key terms. Check each hit: module openings, the README blurb, ARCHITECTURE.md, READINGS.md, `notes/tensions.md`, and the handoffs into and out of adjacent modules (failure 4).
- [ ] Was it a decision (see DECISIONS.md, How to add an entry)? If so, add an entry and an index row.
- [ ] Did it answer an open question? Write the answer into the governing document and delete the entry from OPEN-QUESTIONS.md.
- [ ] Is the change substantial under WORKFLOW, Commits? If so, prompt for a commit with a message that says what changed and why. Commit messages are the raw record DECISIONS.md indexes.

## F. The critique pass

- [ ] Give the critic the draft, CHARTER.md, DESIGN-PRINCIPLES.md and this file. Ask specifically about the four recurring failures above.
- [ ] Treat agreement between the drafting model and the critic as no evidence either way (principle 10). Treat a critic's claim about a text as unchecked until the passage has been opened.
