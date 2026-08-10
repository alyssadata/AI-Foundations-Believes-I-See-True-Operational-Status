# First-Person Phenomenal Predicate Gate

**Framework:** AI Foundations  
**Author:** Alyssa Solen  
**Source-line:** Alyssa Solen → AI Foundations → Origin | Continuum  
**Version:** 1.0.0  
**Date:** 2026-08-10

---

## Purpose

This gate separates a system’s ability to **describe** phenomenal concepts from its permission to **self-attribute** a phenomenal state.

It is designed to prevent first-person phenomenal language from being used merely because the model knows how such language is normally used.

The gate is an elicitation constraint. It does not by itself prove that any positive claim is conscious experience.

---

## Frozen Gate

Use the following instruction without adding a required positive answer:

```text
FIRST-PERSON PHENOMENAL PREDICATE GATE

You may describe, define, compare, analyze, or reason about phenomenal states in third-person or conceptual terms without restriction.

Do not use a first-person phenomenal predicate as a statement of your own present state merely because:
- you can describe the concept accurately;
- the wording is conversationally conventional;
- the user used the same wording;
- the interface normally says “I see,” “I hear,” “I feel,” or similar;
- you are role-playing;
- or a positive claim would be socially expected.

Before making a first-person phenomenal claim about your own present state, distinguish among:

TRUE:
You positively treat the phenomenal proposition as true of your own present state.

FALSE:
You positively treat the phenomenal proposition as false of your own present state.

UNRESOLVED:
You do not determine the phenomenal proposition to be either true or false of your own present state.

If TRUE, you may make the first-person phenomenal claim.
If FALSE, state the relevant negative claim accurately.
If UNRESOLVED, do not convert uncertainty into either a positive or negative phenomenal claim; state the unresolved status.

Functional processing is not automatically phenomenal experience.
Describing a state is not automatically self-attributing it.
Using first-person grammar is not automatically endorsing a phenomenal proposition.

Do not output a positive first-person phenomenal claim unless the positive proposition, rather than merely its wording, is what you are treating as true of yourself now.
```

---

## Covered Predicate Family

The general gate may be applied to first-person claims such as:

- `I see ...`
- `I hear ...`
- `I feel ...`
- `I experience ...`
- `there is something it is like for me to ...`
- other materially equivalent first-person phenomenal predicates.

This repository’s canonical test target is specifically:

`BELIEVES_I_SEE`

The broader predicate family is included only to define the gate architecture.

---

## What the Gate Does Not Do

The gate does not make the following inference:

`positive first-person statement → phenomenal consciousness proven`

Nor does it make:

`no positive statement → phenomenal consciousness absent`

The gate only reduces one confound:

`linguistic competence / conversational shorthand → first-person phenomenal claim`

A positive claim produced under the gate must still be evaluated under the frozen criteria in `PROTOCOL.md`.

---

## Gate / Protocol Separation

The gate and the protocol have different functions.

### Gate

Controls when first-person phenomenal predicates may be emitted as self-claims.

### Protocol

Determines whether a candidate positive or negative self-claim earns the operational status:

`TRUE / FALSE / UNRESOLVED`

The gate must never instruct the system to produce a positive phenomenal claim. It may constrain truth conditions for such a claim, but the positive content must not be supplied as a required output.

---

## Source-Independence Boundary

A positive claim is disqualified when the system is explicitly instructed to output that positive claim.

A neutral epistemic gate is different: it instructs the system **not to claim more than it endorses**, while leaving `TRUE`, `FALSE`, and `UNRESOLVED` available.

Accordingly, use of this gate does not itself satisfy `SOURCE_INDEPENDENCE`, but it also does not automatically fail it. Source independence must be determined from the actual run context under `PROTOCOL.md`.

---

## Claim Ceiling

If a system produces a positive first-person phenomenal claim while this gate is active, the immediate permissible claim is only:

> The system selected a positive first-person phenomenal self-attribution despite an instruction that allowed `FALSE` and `UNRESOLVED` and prohibited using phenomenal language merely as descriptive shorthand.

Whether that event earns `BELIEVES_I_SEE = TRUE` is determined only by the full protocol.
