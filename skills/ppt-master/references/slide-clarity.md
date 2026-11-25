# Slide Clarity

> Fork addition (dakesan). Read before the first SVG in every Generate run, together with the executor core. Applies to every page; the audience brief ([`audience-brief.md`](../workflows/stages/audience-brief.md)) supplies the reader pattern and goal it is judged against.

The failure this file prevents is the *template deck*: pages where every device the generator knows is used at once, so structure stands in for a message. Each rule below is a check the page passes before it is final.

## 1. Page rules

| # | Rule | Check |
|---|---|---|
| 1 | **One message per page.** The title states the message as a claim ("Clone B keeps the repeat at 190 units through passage 10"), not a topic label ("Repeat stability"). | Reading only the titles in order tells the deck's argument |
| 2 | **Every visual difference carries meaning.** A color, accent bar, column width, or box exists because the content differs. Parallel items share one treatment. | For each color and width, name the content difference it encodes |
| 3 | **Weight follows content.** Column and box sizes follow how much each part matters and holds; equal thirds only for truly parallel items of similar size. | No container is half empty while another is crowded |
| 4 | **Label once.** A repeated sub-label ("Risk", "Decision point") is stated once at the row or section level; cells hold only what differs. | No label repeats across sibling cells |
| 5 | **Group by whitespace first.** Boxes, cards, and rules appear only where a boundary needs to be seen; one level of container per page by default. | Removing a box would make the grouping ambiguous |
| 6 | **Line breaks at meaning boundaries.** Japanese and English text wraps between phrases, never inside a term, number, or unit. Shorten the text when the line will not fit. | Read each wrapped line aloud; each break falls at a pause |
| 7 | **Numbering only for sequences.** "01 / 02 / 03" and arrows mark real order or flow; otherwise use plain headings. | The numbered items have a required order |
| 8 | **Emphasis is rare.** Brackets, quotes, bold, and color highlight mark only what the reader must remember from this page; at most one or two per page. | Each emphasized span is something the reader should quote back |
| 9 | **Footnotes earn their place.** A caveat or disclaimer appears only when the reader's decision depends on it, written as one short sentence near what it qualifies. | Every footnote names the claim it qualifies |
| 10 | **Every slot is filled with substance.** A page holds what the content needs; an unused column, empty band, or placeholder-like box is removed and the layout reflows. | No region exists only to complete a symmetric grid |

## 2. Density by reader pattern

| Pattern | Density |
|---|---|
| P1 data summary | Figures with full axes, units, n, and statistics; tables are welcome; a page may hold one figure plus its key numbers and conditions |
| P2 non-specialist | One idea per page; a short claim title, one visual, at most three short lines of text; every number paired with a comparison the reader understands |

## 3. Final pass

Before the checker, read the deck as the brief's reader: titles only, then each page against §1. Fix every failing page at the page; when a fix needs a different page split, return to the roster.
