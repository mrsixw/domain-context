---
name: domain-context
description: Build and sharpen a project glossary and decision context when terminology is ambiguous, CONTEXT.md needs updating, or an ADR records a meaningful architectural choice.
---

# Domain Context

Maintain a concise shared language between the user, agent, and codebase.

## Workflow

1. Read the existing `CONTEXT.md`, glossary, and nearby ADRs before proposing terms.
2. Identify overloaded, vague, or inconsistent domain language.
3. Test each candidate term against concrete scenarios and edge cases.
4. Cross-reference the term with the code, configuration, and interfaces that use it.
5. Update the project glossary only with language supported by the evidence.
6. Offer an ADR only when the decision is difficult to reverse, surprising without context, or the result of a real trade-off.

Keep the glossary authoritative and concise. Do not rewrite code merely to introduce terminology unless the user asks for implementation.
