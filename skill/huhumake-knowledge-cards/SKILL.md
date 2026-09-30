---
name: huhumake-knowledge-cards
description: Use when converting pasted articles or local Markdown/TXT files into a concise series of visual knowledge cards, especially when facts may need verification or source attribution. Do not use for PDF, Anki, or GUI requests.
---

# HUHUmake Knowledge Cards

## Overview

Turn one article into 6–10 self-contained knowledge cards. Preserve the source's meaning, select only knowledge worth remembering, and make every card teach exactly one point.

## Inputs and boundaries

- Accept pasted text or local `.md`, `.markdown`, and `.txt` files. Read local files before drafting.
- If the input is a PDF, Anki deck, or GUI request, state that the format is unsupported and ask for pasted text or a Markdown/TXT export.
- Use the user's requested language; otherwise follow the input language.
- Do not count a cover, contents page, or closing page among the 6–10 knowledge cards. Create those only when requested.

## Workflow

1. Identify the article's purpose, claims, reasoning, examples, and limits. Ignore promotional filler and repeated phrasing.
2. Build a candidate list of atomic knowledge points. Merge duplicates and remove points that are merely transitions, slogans, or unsupported repetition.
3. Rank candidates by importance to understanding and reuse. Keep 6–10. If the source supports fewer than six honest cards and external research is allowed, fill only the missing concepts with relevant, sourced extensions. If research is forbidden or unavailable, explain the shortfall and ask whether to deliver fewer cards; never split one idea merely to reach six.
4. Verify claims when the user requests verification, the article lacks enough support, or a claim is scientific, medical, legal, financial, statistical, controversial, or time-sensitive. Prefer primary or authoritative sources. Clearly label any extension beyond the source and cite it; never present an inference as a source claim.
5. Draft every card with the required contract below. Then compare cards pairwise: each title must answer a different question, and removing one card must remove a distinct idea.
6. Give the series a coherent impressionist visual system. If image generation is available and finished visuals are requested, generate text-free backgrounds first; keep all card copy outside generated images so wording remains accurate and editable.

## Card contract

Return 6–10 numbered cards. Every card must contain all five fields:

```markdown
### Card N — [short title]
- Core knowledge: [one precise, standalone sentence]
- Plain explanation: [2–4 concise sentences explaining meaning, mechanism, or boundary]
- Example / self-check: [one concrete example or one answerable question]
- Impressionist background: [subject, palette, light, brushwork, and quiet text area]
- Evidence: [Original: section/paragraph] or [Extension: S1]
```

Translate the field labels into the output language while preserving this structure.

Use either an example or a self-check, whichever teaches the point better. Do not combine two concepts to fill space. Keep examples illustrative rather than pretending they are evidence.

## Visual direction

Treat the cards as one series: 3:4 portrait composition, visible painterly brushstrokes, atmospheric light, softened edges, and a restrained shared palette. Vary the scene to match each concept while preserving a low-detail, low-contrast area for readable text. Avoid busy focal points behind copy, photorealism, watermarks, logos, and text baked into the background.

## Sources and delivery

After the cards, add `## Sources` only when external material was used. List each source once as `S1`, `S2`, and so on, with title, publisher or author, date when available, and direct URL. Keep original-source material distinguishable from externally added context.

Finish with a short quality note stating the card count, whether external research was used, and any uncertainty the user should review. Do not claim to have generated image files unless they actually exist.

## Quality checks

- 6–10 knowledge cards, excluding optional cover and closing pages
- one distinct knowledge point per card; no repeated conclusions
- every card includes title, core knowledge, explanation, example/self-check, background, and evidence
- important caveats survive compression
- extensions are useful, labeled, and sourced
- all citations are traceable; no invented facts or URLs
- impressionist backgrounds remain visually coherent and leave copy readable
