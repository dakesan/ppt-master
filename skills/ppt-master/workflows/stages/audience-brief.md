---
description: Fork addition (dakesan). Audience brief gate that must pass before any Generate PPTX planning or authoring.
---

# Audience Brief

> Runs once per Generate run (Default and Quick), after source content is read and before planning: Default enters it after Step 1, Quick after §2 source preparation and before the roster. Beautify, Image to PPTX, Create Template, and Edit Native PPTX skip it.

A deck is built for one reader and one goal. Before planning a single page, the agent states — in its own words, not copied from the request — who reads the deck, what the deck must achieve, and how that dictates the way it speaks. A deck planned without this brief drifts into the generic, everything-on-one-page "AI deck".

## 1. Write the brief

Write three items, each as concrete sentences.

**1. Reader** — pick one reader pattern and name the actual people.

| Pattern | Reader | What the reader needs |
|---|---|---|
| P1 data summary | Researchers and 相澤先生 — domain experts who know the project | Raw results with conditions, n, replicates, and statistics; full axes and units; method details on demand; dense pages are fine; no simplification of the science |
| P2 non-specialist | Readers outside the field — an investor/partner deck, material that 石倉さん reads | Conclusion first; every term of art explained or replaced; one message per slide; numbers only where they carry the point, always with a comparison; background before data |
| Other | Anyone else | Describe the reader's background, what they already know, and what they lack, in the same shape as the rows above |

**2. Goal** — what the reader knows, decides, or does after the deck that they did not before. One sentence naming a decision, action, or changed understanding ("相澤先生 agrees to move clone B to the in vivo test"), never a topic ("explain the C9orf72 results").

**3. How to convey** — derived from 1 and 2: the core message, the order (conclusion-first or evidence-first), the depth of each part, what is left out or moved to backup, and the vocabulary level. Each choice cites the reader need or goal it serves.

**Completion criterion**: every item rests on evidence — the user's words, the sources, or this conversation — and another agent given only this brief would build the same outline. An item that rests on a guess is unresolved.

## 2. Resolve gaps

- All three items resolved → print the brief to the user as a short block (Reader / Goal / How to convey) and continue. Default seeds Stage 1 from it (§3); Quick proceeds without a stop.
- Any item unresolved → ask the user 2–3 questions covering only the unresolved items, each with a recommended answer and the reason, then stop until the user answers. Rewrite the brief from the answers and recheck the completion criterion. This stop applies to Quick as well.

## 3. Handoff

The confirmed brief is the source for Stage 1's communication contract ([`strategist.md`](../../references/strategist.md) §c):

| Brief | Stage 1 field |
|---|---|
| Reader (pattern + people) | `audience` |
| Goal | `audience_outcome` |
| How to convey: core message | `core_message` |
| How to convey: order, depth, vocabulary | `communication_intent` |

Quick keeps the brief in context and uses it as the core-message anchor. Both routes read [`slide-clarity.md`](../../references/slide-clarity.md) before the first SVG; the reader pattern sets its density row.
