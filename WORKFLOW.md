# Workflow

Deliberately short. Only rules that change an outcome belong here. Process that does not improve the program is overhead.

## Roles

- **Robert** decides what the program contains and authorizes any push or publication.
- **Claude** is primary author. Drafts directly into the repository. Does not resolve open editorial questions and does not change the architecture through a drafting choice.
- **ChatGPT** is critic. Reviews drafts for weak justifications, forced readings, hidden assumptions, and gaps.

Neither model's agreement with the other establishes anything.

## Unit of work

**One reading entry at a time.** Draft it, have it reviewed, move on. A whole module is too large a unit to hold in review at once.

## Drafting a module

Do not pre-judge a reading for the reader. No advance verdicts on which arguments are strongest, no warning the reader against a text before they meet it, and no positioning of the final reading as the one that sees through the others.

Sequence carries an argument whether or not one is intended: the last reading and the last question acquire authority from their position alone. Test every reading against the others in both directions, and turn the module's sharpest question on whichever reading the draft treats most gently.

## Sourcing rules

1. Cite by edition-independent locator: Stephanus, Bekker, section, chapter, verse. Never by page number.
2. Prefer freely and durably available texts. Availability is a selection criterion (design principle 9).
3. Paraphrase by default. Quote only from a text with a live link, and never from a transcription known to contain errors.
4. Author, title, and year are always checked. A locator that has not been checked is omitted, not guessed.

## Verification status

Two flags per reading in READINGS.md:

- **checked** — the text was opened, the locators exist, the attributed argument is actually in it.
- **unchecked** — anything else.

Interpretations are always the editors' and are never marked checked. The README says so once, for the whole program, so no reader-facing prose carries a status banner.

## Pointers

A pointer is a short editorial note about a work the program does **not** assign. It names the work, states its position, explains why the position matters to the module's problem, and says why the work is not assigned. It is written in the editors' voice.

- No reading assignment, no questions to carry, no quotations.
- Verification burden is author, title, year.
- At most two per module, and a module must work completely for a reader who ignores every pointer.
- **If an argument cannot be compressed into one paragraph without damaging the module, it is load-bearing and needs an assignable text.** Find an accessible one instead of pointing.

## Recurrence

A work may be assigned in more than one module. The reader returns to it with a changed question, in the way anchor cases recur and escalate under design principle 7.

- Each assignment takes its own passages and its own question. A reader does not re-read the same pages.
- Each assignment stands alone. A reader who meets the work only in the later module is not missing something essential from the earlier one.
- The second assignment is earned when that module is built, not reserved in advance.

A work that keeps returning acquires authority the program does not intend. If a text appears in more than two modules, or if it begins to function as the program's answer, it is doing something design principle 2 forbids.

## Reader-facing prose is clean

Modules contain no editorial status, no verification caveats, no process notes. Status lives in READINGS.md. Limitations a reader genuinely needs — an omitted locator, a work behind a library barrier — are stated in one plain sentence, not a banner.

## What gets recorded

Settled rules live in the document they govern: principles in DESIGN-PRINCIPLES.md, sourcing and process here, structure in ARCHITECTURE.md. There is no separate decision log, because a rule recorded in two places will eventually disagree with itself.

OPEN-QUESTIONS.md holds only what is genuinely unresolved. When a question is settled, the answer is written into the document it governs and the entry is deleted.

Exchanges between Claude and ChatGPT are not recorded. Drafts, critiques, disagreements, and the reasoning behind a choice are working conversation, not program material. What survives is the change itself, written into the relevant document. If an argument matters enough to preserve, it belongs in the program's prose where a reader will meet it, not in a file about how the program was made.

## Commits

After any substantial change, prompt Robert to make a fresh commit, and supply a suggested message with the prompt: one sentence, or a short paragraph when several things changed together. The message should describe what changed in the program, not the conversation that produced it.

Substantial means a new or reworked module, a reading assigned or dropped, a change to the architecture, the principles, or this file. Fixing a typo is not.

Robert makes the commit. Whether it is also pushed is a separate decision each time.

## Publication

No push, no remote change, no upload without Robert asking for that specific thing. The GitHub repository is public; while it is, any push publishes drafts. Permission to write locally is not permission to publish.
