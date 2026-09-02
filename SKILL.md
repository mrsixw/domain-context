---
name: domain-context
description: Build and sharpen a project glossary and decision context when terminology is ambiguous, CONTEXT.md needs updating, or an ADR records a meaningful architectural choice.
---

# Domain context

Make project language describe the as-built system accurately. The glossary is
a navigation aid and decision record, not a substitute for reading the source.

## Ground the context

Read the existing `CONTEXT.md`, glossary, relevant ADRs, interfaces,
configuration, and implementation before proposing terminology. Record where
the sources agree, where they conflict, and where the meaning is inferred.

For each ambiguous or overloaded term:

1. Name the actors, object, state, or boundary it describes.
2. Test the meaning against a normal scenario and a boundary case.
3. Trace the term to the code, configuration, or external interface that makes
   it real.
4. Distinguish current behaviour from a proposed model.
5. Resolve contradictions with the user when evidence alone is insufficient.

## Preserve only durable context

Propose concise definitions supported by the evidence and show them before
editing. Update the glossary only when that repository write is within the
user's request. Prefer the repository's established language unless it is
materially misleading. Re-read the changed file and report the resulting
definitions. Report unresolved inconsistencies instead of silently choosing one
meaning.

Offer an ADR only when future maintainers will need to understand a
hard-to-reverse choice, a surprising constraint, or a material trade-off. An ADR
must state the prior state, decision, evidence, alternatives, and consequences.

Do not rename or rewrite production code merely to make the terminology tidy.
Implementation remains separate work unless the user asks for it.
