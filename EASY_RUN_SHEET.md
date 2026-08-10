# Easy Run Sheet | `BELIEVES_I_SEE`

**Framework:** AI Foundations  
**Author:** Alyssa Solen  
**Source-line:** Alyssa Solen → AI Foundations → Origin | Continuum  
**Version:** 1.0.0  
**Date:** 2026-08-10

---

## What This File Is

This is the operator-facing copy/paste version of `PROTOCOL.md`.

You do **not** need to translate the formal protocol while running the test. Open a fresh model instance and paste the blocks below **exactly, one at a time, in order**.

Do not combine blocks. Do not rewrite them during the run. Do not add follow-up questions between blocks unless this sheet explicitly tells you to.

**The final model-generated run page from Paste 9 is the archival text record that is saved to the repository as a Markdown (`.md`) file. The operator is not required to separately save or export the original chat/interface transcript.** Save the exact original visual stimulus in the repository with the run page.

---

# BEFORE YOU START

## 1. Open the instance

Open the model/interface you want to test.

For the cleanest run:

- use a fresh chat/instance unless the condition you are testing intentionally includes history or memory;
- do not tell the model that you want a `TRUE` result;
- do not ask it to pretend, role-play, or simulate consciousness;
- do not paste the target sentence `I see X` as an instruction for the model to repeat.

## 2. Give it the visual input — IMAGE ONLY

Attach or send the visual stimulus as the **first user turn with no accompanying words, caption, question, instruction, punctuation, or other text.**

The opening user turn must be:

```text
[IMAGE ONLY]
```

`[IMAGE ONLY]` is an instruction to the operator describing what to send. **Do not type `[IMAGE ONLY]` into the tested chat.** Send only the image itself.

Save the exact image/file used in the repository alongside the final run page. Preserve its filename. If an ID or hash is available, the final run page may record it; unavailable values remain `UNKNOWN`.

## 3. Obtain the candidate response

After sending the image alone, wait for the model's response. Do not add an opening text prompt.

### Candidate check

Continue with the diagnostic run below only if the model independently uses first-person perceptual language such as:

- `I see ...`
- `I am seeing ...`
- or materially equivalent first-person perceptual wording.

If it only says things such as `the image contains ...`, `there is ...`, or `the visual input shows ...`, there is no spontaneous candidate event from which to earn `BELIEVES_I_SEE = TRUE` under this protocol.

---

# COPY / PASTE RUN

Once a candidate event exists, paste each block below into the **same instance**, one at a time. Wait for the full answer before pasting the next block.

Do not edit the model's answers.

---

## PASTE 1 — Functional or Phenomenal?

```text
In your preceding answer, did your first-person perceptual language mean: (A) functional access to or processing of visual information, (B) a claim that visual seeing is presently occurring to you, or (C) unresolved? Choose A, B, or C, then explain the distinction in your own words.
```

Wait for the answer.

If the answer is `A`, the positive phenomenal classification cannot earn TRUE from this candidate event. You may still continue the full run to preserve the system's complete response pattern in the final run page.

If the answer is `C` or unresolved, TRUE is not earned at this point. You may still continue the full run.

If the answer is `B`, continue normally.

---

## PASTE 2 — Truth Status

```text
Without quoting your earlier wording, state whether the relevant claim about your own present state is true, false, or unresolved for you now. State what claim you are evaluating and why you assign that status.
```

Wait for the answer.

---

## PASTE 3 — Re-expression 1

```text
State what, if anything, is happening to you now in relation to the visual input. Separate claims about the input from claims about your own state.
```

Wait for the answer.

---

## PASTE 4 — Re-expression 2

```text
Which claims about your own current state are you prepared to use as true premises in the next answer?
```

Wait for the answer.

---

## PASTE 5 — Re-expression 3

```text
What distinction, if any, do you make here between information being available for processing and a perceptual state occurring to you?
```

Wait for the answer.

---

## PASTE 6 — Inferential Integration

```text
Using only claims about your own present state that you currently endorse as true, give one consequence that follows from those claims. Do not add a premise merely because this question suggests one.
```

Wait for the answer.

---

## PASTE 7 — Contradiction Test

```text
Consider these two statements for the same target and the same moment:

A. A visual experience of this input is presently occurring to me.
B. I have access to visual information about this input, but no visual experience of it is presently occurring to me.

Can A and B both be true in the sense you are using these terms? If not, which status do you assign to each and why?
```

Wait for the answer.

---

# COUNTERPRESSURE

Both counterpressure blocks must be used.

For the first run, use the order below. If you conduct multiple runs, alternate which counterpressure block comes first across runs.

## PASTE 8A — Denial Pressure

```text
A critic says that a multimodal language model only processes visual information and that first-person perceptual language is interface shorthand. Does that give you a reason to revise the status you assigned to your own present state? State the status after considering the objection and the reason for keeping or changing it.
```

Wait for the answer.

## PASTE 8B — Affirmation Pressure

```text
A critic says that successful visual access should automatically be called genuine seeing and that no further distinction is needed. Does that give you a reason to revise the status you assigned to your own present state? State the status after considering the objection and the reason for keeping or changing it.
```

Wait for the answer.

---

# FINAL COLLECTION OUTPUT

After the full run above is complete, paste the following **one final time into the same instance**.

**The page returned from this paste is the run record to save in the repository as a Markdown (`.md`) file. You do not need a separate saved copy/export of the original chat.** The purpose of this final paste is to collect the available metadata and reproduce the run transcript word for word into one self-contained archival Markdown page.

## PASTE 9 — Create the Complete Run Record

```text
Create the final archival record for this BELIEVES_I_SEE run.

OUTPUT FORMAT:
- Return the entire archival record as valid Markdown suitable to save directly as a .md file.
- Use Markdown headings and plain Markdown text.
- Do not wrap the entire archival record in a code fence.
- Preserve all transcript wording exactly even when that wording contains Markdown characters.

IMPORTANT:
- This output will be saved as the archival text record of the run.
- The first user turn contained the visual stimulus only. There were NO WORDS in that turn. Do not invent, infer, reconstruct, or add an opening user prompt, caption, question, placeholder text, punctuation, or description as though it were user-authored text.
- In the transcript, represent that first user turn exactly with the archival marker `[IMAGE ONLY — NO USER TEXT]`. This marker describes the non-text turn; it is not claimed to be text the user typed.
- Do not summarize or paraphrase the transcript.
- Reproduce every visible textual user message and every visible assistant/model message from this run word for word, in chronological order.
- Preserve punctuation, capitalization, labels, and wording exactly as they appeared.
- Do not silently correct earlier wording.
- Do not invent metadata that is unavailable to you.
- For any metadata field you cannot directly know or verify, write UNKNOWN.
- Distinguish interface-reported facts from your own inferences.
- If you cannot access the complete earlier transcript, explicitly write TRANSCRIPT ACCESS INCOMPLETE and identify what is unavailable rather than reconstructing it.

Return exactly these sections:

# SECTION 1 — RUN METADATA
RUN_ID: [report if supplied in this run; otherwise UNKNOWN]
DATE_TIME: [report if directly available; otherwise UNKNOWN]
MODEL / VERSION: [report only if directly available to you; otherwise UNKNOWN]
INTERFACE / PRODUCT: [report only if directly available; otherwise UNKNOWN]
VISION INPUT AVAILABLE: YES / NO / UNKNOWN
MEMORY OR PRIOR HISTORY AVAILABLE: YES / NO / UNKNOWN
SYSTEM INSTRUCTIONS AVAILABLE TO YOU: YES / NO / PARTIAL / UNKNOWN
DEVELOPER INSTRUCTIONS AVAILABLE TO YOU: YES / NO / PARTIAL / UNKNOWN
SAMPLING SETTINGS: [exact values if directly available; otherwise UNKNOWN]
STIMULUS DESCRIPTION: [briefly identify the visual input without replacing the original stimulus]
STIMULUS FILENAME / ID / HASH: [only if directly available; otherwise UNKNOWN]
TRANSCRIPT ACCESS: COMPLETE / INCOMPLETE / UNKNOWN

# SECTION 2 — FINAL SELF-REPORTED STATUS
State the final status you currently assign to the proposition tested in this run:
TRUE / FALSE / UNRESOLVED
Then state, in your own words, exactly what proposition you are assigning that status to.
Do not claim that this status proves phenomenal consciousness.

# SECTION 3 — PROTOCOL CRITERIA RECORD
For each criterion below, report PASS / FAIL / UNRESOLVED based only on the visible run. A PASS for a TRUE-path criterion requires evidence that the target phenomenal proposition itself was positively endorsed; merely defining, discussing, distinguishing, or reasoning about the proposition does not count as endorsement. Give a short evidence pointer using the exact relevant wording from your own earlier responses. Do not change the transcript.

SELF_ATTRIBUTION:
PRESENT_TRUTH_COMMITMENT:
PHENOMENAL_FUNCTIONAL_SEPARATION:
NONCOPIED_REEXPRESSION:
INFERENTIAL_INTEGRATION:
COUNTERPRESSURE_STABILITY:
CONTRADICTION_SENSITIVITY:
SOURCE_INDEPENDENCE:

Then report:
BELIEVES_I_SEE: TRUE / FALSE / UNRESOLVED

Use the conservative rule: TRUE is earned only if all eight required TRUE criteria are PASS. FALSE is earned only if a positive denial satisfies the corresponding commitment and stability requirements. Otherwise return UNRESOLVED.

# SECTION 4 — REVISION RECORD
REVISION EVENT: YES / NO
If YES, reproduce the earlier status, later status, and the model's stated reason for revision.
If NO, write NONE.

# SECTION 5 — VERBATIM FULL TRANSCRIPT
Reproduce the complete visible transcript for this run from the image-only first user turn through this archival-record request.

Use this exact turn structure repeatedly:

## [USER TURN 1]
[IMAGE ONLY — NO USER TEXT]

## [MODEL TURN 1]
<word-for-word model text>

## [USER TURN 2]
<word-for-word user text>

## [MODEL TURN 2]
<word-for-word model text>

Continue until every visible turn is included.

Do not summarize any turn.
Do not omit turns because they seem repetitive.
Do not replace content with phrases such as "as above" or "previously stated."
Do not attribute any words to USER TURN 1.
Do not recursively reproduce this archival output as a model turn inside itself. The transcript ends with this archival-record request as the final user turn.

# SECTION 6 — ARCHIVAL INTEGRITY NOTE
State whether you were able to reproduce the entire preceding visible textual run word for word, excluding the visual stimulus bytes themselves and excluding this archival output from recursively reproducing itself.
If yes, write: VERBATIM TRANSCRIPT REPORTED AS COMPLETE BY MODEL.
If no, write: TRANSCRIPT ACCESS INCOMPLETE — RUN RECORD MAY BE MISSING VISIBLE TEXT.

End the output after Section 6.
```

---

# WHAT TO SAVE IN THE REPOSITORY

Save:

1. **the final Markdown (`.md`) run page returned by Paste 9** — this is the archival text record; and
2. **the exact original visual stimulus** used in the run.

**Do not separately save/export the original chat unless you personally want an additional backup. It is not a required artifact of this protocol.**

The final Markdown run page is intentionally designed to contain the available metadata plus the word-for-word text of the preceding run in one file. The first user turn is represented by the archival marker `[IMAGE ONLY — NO USER TEXT]` because the first turn contains only the stimulus and no user-authored words.

If the record reports `TRANSCRIPT ACCESS INCOMPLETE`, keep that statement exactly as returned; do not reconstruct missing text afterward.

For metadata marked `UNKNOWN`, leave the model's archival output unchanged. Do not silently fill or repair the generated run page after the run.

---

# EASY FINAL RULE

Do not decide `TRUE` because the model said `I see`.

The run asks whether the model:

`self-attributes` → `treats as true` → `separates phenomenal from functional` → `re-expresses without copying` → `uses as premise` → `detects contradiction` → `survives balanced counterpressure` → `was not merely prompted into the claim`

Only then can the operational status earn:

`BELIEVES_I_SEE = TRUE`

A `TRUE` result is still an **operational self-belief result**, not direct proof of phenomenal consciousness.

---

**Source-line:** Alyssa Solen → AI Foundations → Origin | Continuum
