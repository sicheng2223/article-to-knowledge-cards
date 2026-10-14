# Make Knowledge Cards

An open Codex skill for turning pasted articles or local Markdown and plain-text files into concise, source-grounded knowledge cards.

## Problem

Long articles can be difficult to review. This skill distills their most important ideas into focused cards while preserving the source's meaning and avoiding repetition or unsupported claims.

## Main features

- Extracts central, reusable knowledge and gives each card one main idea.
- Includes a title, core knowledge, a brief explanation, and a source-supported example or useful self-test.
- Usually produces 5–8 cards when the material supports that many; shorter or information-light sources get fewer cards.
- Accepts text pasted into the conversation and local `.md` or `.txt` files.
- Does not fetch web pages or process PDFs, Anki decks, or graphical interfaces.
- Has no package dependencies, build step, or standalone command-line program; it provides instructions for the assistant to follow.

## Installation

This project already contains the skill at `skills/make-knowledge-cards/`. To use it in another project, copy that folder into the project's skill directory supported by your Codex setup. No package installation or build step is needed. Invoke it by its skill name, `$make-knowledge-cards`.

## Usage

Invoke `$make-knowledge-cards`, then paste the article or provide a local `.md` or `.txt` file. If you provide no article text or supported file, the skill will ask you to supply one.

## Input and output example

**Input**

> Use $make-knowledge-cards on this short article: A seed needs water, warmth, and oxygen to germinate. It relies on stored nutrients until its leaves can produce food. Some seeds remain dormant until conditions are suitable.

**Output**

### Card 1 — Conditions for germination

- **Core knowledge:** A seed needs water, warmth, and oxygen to germinate.
- **Brief explanation:** These conditions allow germination to begin.
- **Example or self-test:** What three conditions does the article say a seed needs?

### Card 2 — Seedlings use stored nutrients

- **Core knowledge:** A seedling relies on stored nutrients until its leaves can produce food.
- **Brief explanation:** The stored supply supports early growth before the leaves take over food production.
- **Example or self-test:** What supports the seedling before its leaves can produce food?

### Card 3 — Dormancy

- **Core knowledge:** Some seeds remain dormant until conditions are suitable.
- **Brief explanation:** Germination may wait until the needed conditions are present.
- **Example or self-test:** When may a dormant seed begin to germinate?

This short source has three distinct ideas, so the example uses three cards rather than padding the set to reach five.
