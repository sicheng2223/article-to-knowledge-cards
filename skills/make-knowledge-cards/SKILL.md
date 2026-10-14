---
name: make-knowledge-cards
description: Convert pasted articles or local Markdown and plain text files into concise, source-grounded knowledge cards. Use when the user wants important ideas distilled for review; does not process web pages, PDFs, Anki decks, or graphical interfaces.
---

# Make Knowledge Cards

Turn the user's pasted article or supplied local Markdown or plain text file into a small set of useful knowledge cards.

## Workflow

1. Read the supplied text or supported file. If no source content is available, ask the user to paste it or provide a `.md` or `.txt` file.
2. Identify the source's genuinely important, reusable knowledge. Prefer central claims, principles, mechanisms, decisions, and conclusions over incidental details.
3. Group related details under one idea and remove repetition. Make each card teach or test one idea; split cards when they would otherwise cover multiple independent ideas.
4. Write usually 5–8 cards when the material supports that many. Use fewer for short or information-light sources; do not pad the set to meet a count.
5. Keep every claim grounded in the source. Do not add outside facts, resolve ambiguities by guessing, or imply a stronger claim than the source makes. Preserve meaningful qualifications and uncertainty.
6. Present the cards in source order when that helps the reader follow the material; otherwise order them from foundational to applied.

## Card format

For each card, include:

- **Title**: a short label for the single idea.
- **Core knowledge**: the idea stated clearly and precisely.
- **Brief explanation**: enough context to understand why or how it matters.
- **Example or self-test**: use a source-supported example when available; otherwise give a concise self-question answerable from the card. Do not invent illustrative facts.

Use this Markdown shape:

### Card 1 — [Title]

- **Core knowledge:** ...
- **Brief explanation:** ...
- **Example or self-test:** ...

If the source is too thin to support an example, use a self-test. If even that would repeat the core knowledge without helping recall, omit the field rather than fabricate or pad. Keep explanations compact and avoid restating the same idea across cards.

## Scope

Work only with content the user provides in the conversation or supported local Markdown/plain-text files. This skill does not fetch web pages or extract content from PDFs, Anki decks, or graphical interfaces. If the user supplies an unsupported format, ask for the text or a supported file.
