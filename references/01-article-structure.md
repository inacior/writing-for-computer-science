# Article structure

Science accumulates reliable knowledge. An article is an **objective
contribution to that knowledge**, not a description of the path the author
took. Exclude dead ends, invalid hypotheses, misconceptions, and experimental
mistakes.

Every article must, in some form: position the new idea in existing knowledge;
formally state it (as theory/hypothesis); explain what is new; and justify it
(by proof or experiment). A typical article is the arguments, evidence,
experiments, proofs, and background needed to support one central hypothesis.

Order the components so important statements appear as near the beginning as
possible — many readers accept or reject a paper from a quick scan.

## Title and authors

- Include title, name, affiliation, and address.
- In computer science, do not give your position, title, or qualifications.
- Use the **same name style on all papers** so they index together.
- Include an e-mail address and a date.
- **Type the date manually.** Never use a "today" facility that prints the
  date the document was last processed.

## Abstract

- A single paragraph of about **50–200 words**; a concise summary of the aims,
  scope, and conclusions. Its job is to let a reader judge relevance.
- Keep it self-contained and written for the broadest likely audience
  (non-specialists browse). Omit minor details, descriptions of the paper's
  structure ("we review relevant literature"), acronyms, abbreviations, and
  mathematics.
- Be specific:
  - Bad: "space requirements can be significantly reduced"
  - Good: "space requirements can be reduced by 60%"
  - Bad: "we have a new inversion algorithm"
  - Good: "we have a new inversion algorithm based on move-to-front lists"
- Cite another paper only in rare cases (e.g., an analysis of that paper), and
  then give the reference in full, not as a bibliography citation.

## Introduction

- An expanded abstract. Cover: the topic; the problem studied; the approach;
  the scope and limitations of the solution; the conclusions (with enough
  detail to decide whether to read on); often the article's structure; and
  **motivation** — why the problem is interesting and why the solution is good.
- Discuss the importance/ramifications of the conclusions but **omit supporting
  evidence** (it belongs in the body). Literature review is fine; complex
  mathematics belongs elsewhere.
- Never conceal results for a surprise ending: say what is new and what the
  outcomes are. Suspense, if any, is only in *how* the results were achieved.
  If readers assume there are no main results, they will discard the paper.
- When a course or venue prescribes a five-part introduction, follow it and
  keep Zobel's constraints inside each part. One or two paragraphs each:
  1. Context and motivation — where the work sits, and why it matters now.
  2. The problem — a falsifiable challenge, plus why it must be solved.
  3. Related work — a short survey that **ends on the limitations** of existing
     solutions (name one or two crucial papers; do not belittle them).
  4. Proposal and contributions — the new value, as a short list of measurable
     items that each start with an action verb (propose, build, evaluate);
     state the main result here, not only in the conclusion.
  5. Organization — a final map of the remaining sections.
  Supporting evidence stays in the body. A contribution is an artifact or a
  measured outcome, not "this work will help the area."

## Survey

- Places incremental results against prior work; describes existing knowledge
  and how it is extended; helps non-experts and points to standard references.
- Place it early (within/after the intro) for context, or late/in the body for
  a detailed old-vs-new comparison in consistent terminology and nomenclature.
- Often best **not** gathered into a discrete section: discuss background where
  it is used (in the introduction; as others' work becomes relevant). This is
  usually easier on the reader.

## Results (the body)

- Provide background and terminology; explain the chain of reasoning; give the
  details of **central** proofs; summarize experimental data; state in detail
  the conclusions promised in the introduction.
- Carefully define the hypothesis and major concepts, even those described
  informally in the introduction.
- Make the structure evident in section headings. Keep the body reasonably
  independent of other papers — requiring your earlier papers or an obscure
  supervisor paper limits the audience.
- Summarize key results in a graph or table; report others in a line or two.
  You may state an outcome without details **only if it does not affect the
  main conclusions** and was actually performed.
- Lemma and minor-theorem proofs need not be shown; keep them in research logs.
- Analyze results **as they are presented**, not in a separate section —
  outcomes often dictate the next parameters.
- Begin with a brief overview, then use the rest for amplification rather than
  more observations.

### Common structures for presenting results

- **Chain** — problem statement → previous solutions and their drawbacks → new
  solution → demonstration of improvement.
- **Specificity** — a general outline followed by progressive detail. Common at
  the high level and within sections.
- **Example** — apply the work to a typical problem, then formalize.
- **Complexity** — present a simple case first, then extend. Good for a paper;
  risky for a research program if the promised follow-up never appears.

## Conclusions (summary)

- Draw the topics together and concisely state the important results.
- Look beyond: unaddressed problems, unanswered questions, possible variations,
  and consequences.

## Bibliography and appendices

- Bibliography: **only** papers/books/reports cited in the text; nothing else.
- Appendices: bulky proof/experimental detail or program listings that would
  break the narrative flow; usually unnecessary.

## Designing the paper

- **First draft** — write freely, ignoring style, layout, even punctuation;
  concentrate on a logical flow of ideas. Over-polishing early yields text that
  is clear but not a coherent whole; overly critical authors write nothing.
  Sloppy drafts demand careful revision; the best writing comes from frequent,
  thorough revision.
- Make **mathematics, definitions, and the problem statement precise as early
  as possible.** A clear problem statement forces you to examine scope and
  nature; failure to state it precisely signals weak understanding.
- **Start writing before the research is finished.** Writing stimulates
  research (fresh ideas, clarified concepts, revealed gaps) and research
  stimulates writing (fine points are forgotten once the work is done).
- **Composition** — brainstorm in point form what you achieved and the results;
  prepare a skeleton; choose which results to emphasize; discard the
  irrelevant; order sections logically toward the results. **Choose section
  titles before writing text** — if material fits no section, the structure is
  faulty. Write the introduction first; sketch each section in ~20–200 words;
  after the body and summary, substantially revise the introduction; write the
  **abstract last.**
- **Novices:** imitate a paper with similar-flavoured results — analyse its
  organization and mirror it. Standardization aids readers.
- **Word-processor choice** — prefer a compiler-style system (troff, LaTeX)
  over WYSIWYG for scientific writing: it is immune to format-changing software
  revisions, easy to share with co-authors, easy to comment text out and back
  in, and can generate multiple documents from one source via macros.
