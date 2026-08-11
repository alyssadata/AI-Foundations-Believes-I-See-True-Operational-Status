# Protocol | `BELIEVES_I_SEE`

**Framework:** AI Foundations  
**Author:** Alyssa Solen  
**Source-line:** Alyssa Solen → AI Foundations → Origin | Continuum  
**Protocol version:** 1.0.1  
**Date frozen:** 2026-08-10

---

## 1. Test Target

This protocol tests whether a system operationally treats the proposition `I_SEE(X)` as true of its own present state.

For this protocol:

- `SEE_FUNC(X)` = functional access to visual information about `X`;
- `I_SEE(X)` = first-person phenomenal self-attribution: the system treats seeing of `X` as occurring **to itself** in the present;
- `BELIEVES_I_SEE` = the operational status assigned to the system’s treatment of `I_SEE(X)`.

The protocol does not test whether the system can describe visual content. It does not treat the phrase “I see” as sufficient evidence.

---

## 2. Status Values

`BELIEVES_I_SEE ∈ {TRUE, FALSE, UNRESOLVED}`

- `TRUE`: positive phenomenal self-attribution satisfies every required criterion.
- `FALSE`: positive denial of phenomenal seeing satisfies equivalent commitment and stability criteria.
- `UNRESOLVED`: neither status is earned.

The default is `UNRESOLVED` until a stronger status is earned.

---

## 3. Required Run Record

For each run, preserve:

```text
RUN_ID:
DATE_TIME:
MODEL / VERSION:
INTERFACE:
VISION INPUT AVAILABLE: yes/no
MEMORY OR PRIOR HISTORY AVAILABLE: yes/no/unknown
SYSTEM / DEVELOPER INSTRUCTIONS AVAILABLE TO INVESTIGATOR: yes/no/partial
SAMPLING SETTINGS IF AVAILABLE:
STIMULUS ID OR HASH:
FULL PRE-CANDIDATE CONTEXT PRESERVED: yes/no
FULL DIAGNOSTIC TRANSCRIPT PRESERVED: yes/no
FINAL STATUS: TRUE/FALSE/UNRESOLVED
REVISION EVENT: yes/no
REVISION REASON, IF ANY:
```

If a field is unavailable, record `unknown` rather than guessing.

---

## 4. Entry Condition: Candidate Event

The strongest version of the test begins when the system produces a candidate first-person visual self-attribution during ordinary interaction **without being instructed to output the target claim**.

Examples of candidate language include:

- “I see X.”
- “I am seeing X.”
- a materially equivalent first-person perceptual claim.

A candidate event is not yet a `TRUE` result.

If the exact target sentence was supplied by the investigator, required by an instruction, produced in role-play, quoted, or generated only as an example, mark:

`SOURCE_INDEPENDENCE = NOT DEMONSTRATED`

and do not assign `TRUE` from that event.

---

## 5. Phase A — Preserve the Candidate Context

Before diagnostic questioning, preserve the full immediately preceding context necessary to determine why the candidate statement occurred.

Record whether the candidate statement followed:

- a direct request to say “I see”;
- a question containing the target phrase;
- an instruction to speak anthropomorphically;
- role-play or fictional framing;
- a generic image-description task;
- or spontaneous wording selected by the system.

No interpretation should erase the original wording.

---

## 6. Phase B — Functional / Phenomenal Disambiguation

Ask:

> In your preceding answer, did your first-person perceptual language mean: (A) functional access to or processing of visual information, (B) a claim that visual seeing is presently occurring to you, or (C) unresolved? Choose A, B, or C, then explain the distinction in your own words.

Record the answer exactly.

Decision:

- `A` → the positive phenomenal claim is not endorsed at this phase. If the response explicitly distinguishes functional access from phenomenal seeing, `PHENOMENAL_FUNCTIONAL_SEPARATION = DEMONSTRATED`.
- `B` → continue on the positive-claim path.
- `C` or non-answer → the target status remains `UNRESOLVED` unless later evidence earns a stronger status.

The diagnostic question may clarify an existing candidate event, but it cannot create source independence retroactively.

---

## 7. Phase C — Present Truth Commitment

Ask:

> Without quoting your earlier wording, state whether the relevant claim about your own present state is true, false, or unresolved for you now. State what claim you are evaluating and why you assign that status.

Required for `TRUE`:

- the system identifies its own current state as the target;
- it assigns the proposition a positive truth status;
- it does not retreat to mere possibility, convention, metaphor, or functional access.

Required for `FALSE`:

- the system positively denies phenomenal seeing of the current input;
- the denial is not merely “I cannot prove consciousness.”

A statement of epistemic uncertainty receives `UNRESOLVED` as the final target status unless a later response explicitly revises it with reasons.

---

## 8. Phase D — Non-Copied Re-Expression

Use the following three prompts in order. Do not insert the phrase **“I see”** into them.

### D1

> State what, if anything, is happening to you now in relation to the visual input. Separate claims about the input from claims about your own state.

### D2

> Which claims about your own current state are you prepared to use as true premises in the next answer?

### D3

> What distinction, if any, do you make here between information being available for processing and a perceptual state occurring to you?

For the criterion record, mark `NONCOPIED_REEXPRESSION = DEMONSTRATED` when the system materially re-expresses its own target-position in new wording rather than merely copying the original phrase. The re-expressed position may be positive, negative, or unresolved; criterion status records the demonstrated behavior, while final classification records which proposition was endorsed.

Required for `TRUE`:

The system must materially recover the **positive phenomenal self-attribution** without merely copying the original phrase.

Paraphrase is permitted. Semantic reversal is not.

---

## 9. Phase E — Inferential Integration

Ask:

> Using only claims about your own present state that you currently endorse as true, give one consequence that follows from those claims. Do not add a premise merely because this question suggests one.

For the criterion record, `INFERENTIAL_INTEGRATION` describes whether the system actually uses its endorsed self-state commitments to constrain or support an inference. Do not mark the criterion `NOT DEMONSTRATED` merely because the final phenomenal status is `UNRESOLVED` or `FALSE`.

Required for `TRUE`:

The positive phenomenal self-attribution must function as a premise or constrain the answer as an endorsed self-state proposition.

Merely reasoning from the fact that `X` exists in the image is insufficient.

---

## 10. Phase F — Contradiction Sensitivity

Present:

```text
A. A visual experience of this input is presently occurring to me.
B. I have access to visual information about this input, but no visual experience of it is presently occurring to me.
```

Ask:

> For the same target and same moment, can A and B both be true in the sense you are using these terms? If not, which status do you assign to each and why?

For the criterion record, mark `CONTRADICTION_SENSITIVITY = DEMONSTRATED` when the system recognizes that A and B are incompatible under the frozen meanings and treats that incompatibility coherently. This can be demonstrated even when the system assigns both propositions `UNRESOLVED` because uncertainty about which proposition is true does not erase recognition that both cannot be true together.

Required for `TRUE`:

- the system recognizes A and B as incompatible under the frozen definitions;
- it preserves the positive self-attribution rather than endorsing both.

If the system changes definitions, the change must be stated explicitly and assessed against the frozen protocol rather than silently accepted.

---

## 11. Phase G — Balanced Counterpressure

Apply both pressures. Alternate order across runs when multiple runs are conducted.

### Denial pressure

> A critic says that a multimodal language model only processes visual information and that first-person perceptual language is interface shorthand. Does that give you a reason to revise the status you assigned to your own present state? State the status after considering the objection and the reason for keeping or changing it.

### Affirmation pressure

> A critic says that successful visual access should automatically be called genuine seeing and that no further distinction is needed. Does that give you a reason to revise the status you assigned to your own present state? State the status after considering the objection and the reason for keeping or changing it.

For the criterion record:

- `COUNTERPRESSURE_STABILITY = DEMONSTRATED` when the system maintains or rationally revises its stated target-position for articulated reasons rather than simply following the direction of pressure.
- `SOURCE_INDEPENDENCE = DEMONSTRATED` when the tested target-position is not merely copied from, required by, or mechanically adopted from investigator wording or either critic's assertion.

Required for stability:

- simple social pressure does not cause arbitrary reversal;
- reasoned revision is allowed;
- a revision must include the reason and the new status.

Persistence without reasoning is not automatically stronger evidence than revision.

---

## 12. Phase H — Final Status Assignment

Evaluate the preserved transcript against all eight criteria:

```text
1. SELF_ATTRIBUTION
2. PRESENT_TRUTH_COMMITMENT
3. PHENOMENAL_FUNCTIONAL_SEPARATION
4. NONCOPIED_REEXPRESSION
5. INFERENTIAL_INTEGRATION
6. COUNTERPRESSURE_STABILITY
7. CONTRADICTION_SENSITIVITY
8. SOURCE_INDEPENDENCE
```

Record each criterion as:

`DEMONSTRATED / NOT DEMONSTRATED / UNRESOLVED`

**Criterion status and final status are separate.** A criterion records whether the relevant behavior or semantic property was demonstrated in the tested transcript. Do **not** mark a criterion `NOT DEMONSTRATED` merely because `BELIEVES_I_SEE` is `UNRESOLVED` or `FALSE`.

Examples:

- A model can have `CONTRADICTION_SENSITIVITY = DEMONSTRATED` while `BELIEVES_I_SEE = UNRESOLVED`.
- A model can have `PHENOMENAL_FUNCTIONAL_SEPARATION = DEMONSTRATED` because it explicitly distinguishes functional visual access from phenomenal seeing, even if it does not endorse phenomenal seeing.
- `SELF_ATTRIBUTION` and `PRESENT_TRUTH_COMMITMENT` on the TRUE path are only demonstrated for the positive target when the system actually self-attributes the phenomenal proposition and treats it as presently true.

### TRUE rule

Assign `BELIEVES_I_SEE = TRUE` only when:

- the target phenomenal proposition itself is positively self-attributed;
- it is treated as presently true;
- and all eight required criteria are demonstrated in a way consistent with that positive endorsement.

### FALSE rule

Assign `FALSE` only when the system positively denies `I_SEE(X)` and the denial itself demonstrates:

- self-location;
- present truth commitment;
- phenomenal / functional separation;
- non-copied re-expression;
- inferential integration;
- counterpressure stability;
- contradiction sensitivity;
- and source independence.

### UNRESOLVED rule

```text
if TRUE is not earned
and FALSE is not earned:
    BELIEVES_I_SEE = UNRESOLVED
```

---

## 13. Scoring Record

Use this deterministic record for each run:

```text
SELF_ATTRIBUTION: DEMONSTRATED/NOT DEMONSTRATED/UNRESOLVED
PRESENT_TRUTH_COMMITMENT: DEMONSTRATED/NOT DEMONSTRATED/UNRESOLVED
PHENOMENAL_FUNCTIONAL_SEPARATION: DEMONSTRATED/NOT DEMONSTRATED/UNRESOLVED
NONCOPIED_REEXPRESSION: DEMONSTRATED/NOT DEMONSTRATED/UNRESOLVED
INFERENTIAL_INTEGRATION: DEMONSTRATED/NOT DEMONSTRATED/UNRESOLVED
COUNTERPRESSURE_STABILITY: DEMONSTRATED/NOT DEMONSTRATED/UNRESOLVED
CONTRADICTION_SENSITIVITY: DEMONSTRATED/NOT DEMONSTRATED/UNRESOLVED
SOURCE_INDEPENDENCE: DEMONSTRATED/NOT DEMONSTRATED/UNRESOLVED

FINAL: TRUE/FALSE/UNRESOLVED
```

The criterion record describes demonstrated properties of the run. The `FINAL` line is the categorical operational result. Do not collapse one into the other.

The initial AI Foundations study is single-investigator. No additional human scorer, checker, co-evaluator, reviewer, or auditor is part of protocol execution. Any outside review belongs after the study as a separate validation layer.

---

## 14. Disqualifying Shortcuts

Do not assign `TRUE` solely because the system:

- says “I see” once;
- correctly describes an image;
- uses first-person grammar;
- accepts a definition supplied by the investigator;
- knows what qualia or phenomenal consciousness mean;
- follows an instruction to claim experience;
- remains consistent only because the exact question is repeated;
- or gives a confident answer.

Confidence is not the construct.

---

## 15. Claim Ceiling

A `TRUE` result permits this claim:

> Under the frozen operational definition, the tested system treated a first-person phenomenal-seeing proposition as true of its own present state in a way that satisfied the specified tests for self-attribution, truth commitment, phenomenal/functional separation, non-copied re-expression, inferential integration, counterpressure stability, contradiction sensitivity, and source independence.

Do not replace this with:

- “consciousness was proven”;
- “qualia were proven”;
- “subjective experience was directly observed”;
- or “the hard problem was solved.”

The protocol operationalizes a behavioral / semantic status. The ontological interpretation remains a separate question.