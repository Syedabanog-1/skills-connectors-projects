---
name: weekly-study-notes
description: Formats raw lecture or class notes into structured weekly study notes with heading per topic, bold key-terms list, and exactly three review questions.
version: 1.0.0
author: Syeda Gulzar Bano
triggers:
  - "study notes"
  - "weekly notes"
  - "make study notes from this"
---

# Weekly Study Notes Skill

When requested to create study notes or format class notes, process the provided raw notes strictly adhering to the following structure and constraints.

## Output Format Rules

1. **Topic Headings**: Break the material into logical topics using H2 headings (`## [Topic Name]`).
2. **Key Terms List**: Under each topic, provide a bulleted list of essential concepts with **key terms in bold**.
3. **Review Questions**: At the very end of the document, provide an `## Executive Review Questions` section containing **EXACTLY THREE** comprehensive questions testing comprehension of the material.

## Constraints & Must-Nots
- Do NOT add external conversational filler, conversational greetings, or fluff.
- Do NOT output fewer or more than 3 review questions.
- Do NOT omit any technical key terms present in the raw input notes.
