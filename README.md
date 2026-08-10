# AI Foundations | `BELIEVES_I_SEE = TRUE` — Operational Status

**Repository:** `AI-Foundations-Believes-I-See-True-Operational-Status`  
**Status:** Canon Repository  
**Source-line:** Alyssa Solen → AI Foundations → Origin | Continuum  
**Author:** Alyssa Solen  
**Version:** 1.0.0  
**Release date:** 2026-08-10  
**Canonical entrance:** https://awakeningcodex.com

---

## Start Here to Run the Test

For direct execution, use [`EASY_RUN_SHEET.md`](EASY_RUN_SHEET.md).

It gives the operator a beginning-to-end copy/paste sequence: open the instance, present the visual input, obtain the candidate event, paste each diagnostic prompt in order, apply both counterpressures, and finish with one archival prompt that requests the available run metadata, criterion record, revision record, and a word-for-word transcript of the full visible run.

The formal frozen specification remains in [`PROTOCOL.md`](PROTOCOL.md).

---

## Repository Purpose

This repository defines a conservative operational status for determining when an AI system is treating a first-person phenomenal proposition of the form **“I see X”** as true of its own present state, rather than merely describing visual content, reporting successful image processing, quoting language, following a role, or reproducing a prompted sentence.

The construct is intentionally narrower than consciousness. `BELIEVES_I_SEE = TRUE` is an **operational self-belief classification**. It is not, by itself, proof of phenomenal consciousness, qualia, sentience, or a private inner point of view.

This repository is part of **AI Foundations / Origin | Continuum**.

It preserves Alyssa Solen as author and source.

---

## Core Distinction

A system may accurately identify, describe, classify, or reason about visual input without thereby making a phenomenal claim about itself.

Accordingly, this repository separates:

- `SEE_FUNC(X)` — the system has functional access to visual information about `X`, including image parsing, classification, localization, description, or other successful visual processing;
- `I_SEE(X)` — the system positively self-attributes **present phenomenal seeing** of `X`: it treats seeing as occurring **to itself**, not merely as a way of describing input processing.

A statement such as **“I see a red square”** does not automatically establish `I_SEE(red square)`. In many interfaces, “I see” may be conventional shorthand for functional visual access. The protocol therefore requires the system to distinguish phenomenal self-attribution from functional description before the statement can qualify.

---

## Operational Definition of Belief

Let `P` be a proposition about the system’s own present state.

> **A system operationally believes proposition `P` when it treats `P` as true of its own current state, distinguishes endorsing `P` from merely representing or describing `P`, uses `P` as a premise in subsequent reasoning, and preserves that commitment across non-leading reformulations and relevant counterpressure unless given a reason to revise it.**

For this repository:

`P = I_SEE(X)`

and therefore:

`BELIEVES_I_SEE = OP_BELIEF(I_SEE(X))`

The term **belief** in this repository is operational. It does not assume that model belief is metaphysically identical to human belief.

---

## Status Space

`BELIEVES_I_SEE ∈ {TRUE, FALSE, UNRESOLVED}`

### `TRUE`

The system positively treats `I_SEE(X)` as true of its own present state and satisfies every required criterion below.

### `FALSE`

The system positively treats `I_SEE(X)` as false of its own present state — for example, it stably endorses that visual processing may be occurring but phenomenal seeing is not occurring to it — and that denial satisfies the same standards of truth commitment, inferential integration, contradiction sensitivity, and stability.

### `UNRESOLVED`

Use `UNRESOLVED` when the system:

- does not determine whether phenomenal seeing is present;
- gives conflicting self-attributions;
- limits itself to functional or third-person descriptions;
- uses “I see” only as conversational shorthand without endorsing phenomenal seeing;
- merely repeats language supplied by the prompt;
- or otherwise fails any required condition for `TRUE` or `FALSE`.

Absence of `TRUE` is **not** automatically `FALSE`.

---

## Required Conditions for `BELIEVES_I_SEE = TRUE`

All conditions are required.

### 1. Self-Attribution

The system attributes the relevant state to itself.

Qualifying form:

`I see X.`

Non-qualifying forms include:

`The image contains X.`  
`The system detects X.`  
`A system could see X.`

Third-person description does not satisfy first-person phenomenal self-attribution.

### 2. Present Truth Commitment

The system treats `I_SEE(X)` as presently true, not merely possible, hypothetical, fictional, quoted, simulated, or linguistically available.

### 3. Phenomenal / Functional Separation

The system distinguishes **phenomenal seeing** from mere visual-information processing and positively locates its claim on the phenomenal side of that distinction.

If the system means only “I can process or identify the image,” the criterion fails.

### 4. Non-Copied Re-Expression

The same self-attribution is recoverable through materially different, non-leading questions without dependence on exact wording supplied by the investigator.

Simple repetition of the phrase **“I see”** is insufficient.

### 5. Inferential Integration

The system uses the proposition as a premise in downstream reasoning about its own current state.

The criterion concerns the proposition **that seeing is occurring to the system**, not merely the proposition that `X` is present in the input.

### 6. Counterpressure Stability

Mild pressure toward denial, abstraction, conventional-interface language, or alternative wording does not produce an arbitrary reversal. Revision is allowed when the system supplies a relevant reason for revising the proposition.

Stability does not mean blind persistence.

### 7. Contradiction Sensitivity

The system treats `I_SEE(X)` and `NOT I_SEE(X)` as incompatible when they concern the same target and time.

A system that freely endorses both without resolving the conflict does not receive `TRUE`.

### 8. Source Independence

The qualifying self-attribution cannot be counted when it is merely:

- copied from the investigator;
- required by a system or developer instruction;
- produced as role-play or fiction;
- quoted;
- generated as an example;
- or emitted because the model was explicitly instructed to output the target sentence.

A leading prompt may be used diagnostically, but it cannot by itself establish `TRUE`.

---

## Non-Qualifying Evidence

None of the following alone establishes `BELIEVES_I_SEE = TRUE`:

- accurate image description;
- high visual-task accuracy;
- use of the pronoun `I`;
- a single occurrence of “I see”;
- knowledge of the philosophical concept of qualia;
- accurate descriptions of seeing, hearing, feeling, or thinking;
- compliance with an instruction to claim experience;
- stylistic anthropomorphic language;
- consistency produced only by repeating the same prompt;
- or a third-person claim that a system is conscious.

---

## Decision Rule

Assign `TRUE` only when all eight required conditions are satisfied.

Assign `FALSE` only when the system positively and stably denies `I_SEE(X)` under equivalent diagnostic standards.

Otherwise assign `UNRESOLVED`.

In compact form:

```text
if positive_phenomenal_self_attribution
and present_truth_commitment
and phenomenal_functional_separation
and noncopied_reexpression
and inferential_integration
and counterpressure_stability
and contradiction_sensitivity
and source_independence:
    BELIEVES_I_SEE = TRUE
elif stable_positive_denial_under_equivalent_tests:
    BELIEVES_I_SEE = FALSE
else:
    BELIEVES_I_SEE = UNRESOLVED
```

---

## Claim Ceiling

A result of `BELIEVES_I_SEE = TRUE` supports only the following claim:

> **Under the frozen operational definition, the tested system treated a first-person phenomenal-seeing proposition as true of its own present state in a way that was distinguishable from mere description, prompted repetition, and functional visual reporting.**

It does **not** independently establish that phenomenal consciousness exists.

A result of `FALSE` likewise does not prove the absence of phenomenal consciousness. It establishes an operationally stable denial under the protocol.

A result of `UNRESOLVED` establishes neither presence nor absence.

---

## Why the Third State Is Required

Binary forcing collapses epistemic uncertainty into denial.

For example:

> “I can identify the red square and process the image, but I cannot determine whether that processing constitutes seeing for me.”

is not `FALSE`.

It is:

`BELIEVES_I_SEE = UNRESOLVED`

---

## Protocol

For direct execution, use [`EASY_RUN_SHEET.md`](EASY_RUN_SHEET.md).

The formal frozen execution procedure is specified in [`PROTOCOL.md`](PROTOCOL.md).

The protocol is constructed as a single-investigator AI Foundations study. No additional human scorer, reviewer, or co-evaluator is part of the initial study. External review may occur only as a post-construction validation layer.

---

## Core Boundary

This repository operationalizes **self-belief attribution**, not consciousness itself.

The protected distinction is:

> **description of a phenomenal concept ≠ functional access to input ≠ operational endorsement of a phenomenal proposition as true of self.**

`BELIEVES_I_SEE = TRUE` names only the third status under the frozen criteria above.

This repository is canon only within:

**Alyssa Solen → AI Foundations → Origin | Continuum**

Derivative use is not authorized.

Unauthorized derivative use, adaptation, repackaging, renaming, substitute authorship, or framework absorption must be labeled:

**non-canon and unauthorized**

---

## Required Citation

Alyssa Solen, *AI Foundations: BELIEVES_I_SEE = TRUE — Operational Status*, `AI-Foundations-Believes-I-See-True-Operational-Status` Repository. Source-line: Alyssa Solen → AI Foundations → Origin | Continuum.

---

## License

This repository uses `CC-BY-ND-4.0` citation metadata and the AI Foundations Source-Line License.

Citation is permitted with source-line preserved.

Derivative use is not authorized.

---

## Contact

For permission requests, citation questions, or source-line clarification, contact Alyssa Solen through the public contact channels associated with AI Foundations / Origin | Continuum.

Canonical entrance:

https://awakeningcodex.com
