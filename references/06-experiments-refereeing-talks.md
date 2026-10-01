# Hypotheses & experiments, refereeing, and short talks

## Hypotheses and experiments

### Stating hypotheses
- Specify hypotheses clearly, precisely, and unambiguously; state what is *not*
  proposed and where the conclusions stop.
- Limit scope to a domain that can feasibly be explored; make the claim
  falsifiable — the more vulnerable to disproof, the more convincing a
  successful demonstration.
  - Bad: "Q-lists are superior to P-lists." (would have to hold everywhere,
    always)
  - Good: "As an in-memory search structure for large data sets, Q-lists are
    faster and more compact than P-lists. We assume a skew access pattern — the
    majority of accesses are to a small proportion of the data."
  - Bad: "Our proposed query language is relatively easy to learn." (vague,
    unfalsifiable)
- Distinguish a mere observation ("the algorithm worked on our data") from a
  tested hypothesis ("the algorithm was predicted to work on any data of this
  class, and this prediction has been confirmed on our data").

### Developing hypotheses
- Refine hypotheses as testing proceeds; expect evolution alongside experimental
  refinement.
- Never let the hypothesis follow the experiments: keep tests as blind as
  possible. Fine-tuning hypothesis and experiment on the same data yields
  observations, not confirmation.
- Apply Occam's razor: where two hypotheses fit equally well, choose the simpler.
- Reject a hypothesis if it yields improbable consequences, contradicts a belief
  that could only have been held out of stupidity, or explains no more than the
  current belief.
- Test your own hypothesis hardest when you like it most — try to disprove it
  rather than twisting results.

### Defending hypotheses
- Build an explicit argument linking evidence to hypothesis; evidence alone is
  unconvincing.
- Play inquisitor: raise objections, rebut the rebuttable, concede what cannot
  be rebutted, admit uncertainty — and include this reasoning in the paper.
- Actively hunt counter-examples; if an objection cannot be refuted, raise it
  yourself; it may force you to reconsider your results.

### Evidence
- Choose among four kinds — analysis/proof, modelling, simulation, experiment —
  by persuasiveness, not minimal effort.
- Treat proofs as fallible; do not assume all hypotheses are amenable to formal
  analysis, or that complexity analysis suffices.
- Keep model, simulation, and experiment distinct: computing a model's
  predictions is *not* a test of the algorithm; a simulation is an artificial
  test; an experiment is a full test on real or realistic data.
- Design the experiment in light of model predictions, and let methods
  corroborate each other.

### Designing fair experiments
- Make tests fair, not built to support the hypothesis; design the environment
  to seem reasonable to supporters of the competing idea.
- Test the cases where the hypothesis is *least* likely to hold — those are the
  interesting cases. Verify that what you test is what you intended.
- Seek alternative interpretations of results and design further tests to
  eliminate them (e.g., is the speed gain from fewer cycles or faster
  compressed-file fetch?).
- Handle failure carefully: proving impossibility invites doubt; be rigorous.
- Sanity-check via conservation rules, boundary behaviour, and rough expected
  values; avoid overstating — success in a special case proves nothing general.

### Designing robust experiments
- Minimize extraneous factors; aim for results independent of system
  characteristics and constant-factor overheads.
- Choose test data carefully: use standard benchmarks/corpora where they exist;
  otherwise ensure data is representative.
- Describe performance in terms of commonly available hardware (clock speed,
  disk access time) so others can relate results to their system.
- Prefer unambiguous Boolean outcomes; where impossible, demonstrate a trend.
- Do not over-generalize from implementation comparisons.
- Guard against luck: run many times; report minimum, average, median, or
  maximum as appropriate and justify the choice.
- Explain anomalies rather than silently discarding them ("the algorithm was
  much slower on two of the data sets; we are still investigating").

### Describing experiments
- Interpret results — do not merely compile figures; analyze significance,
  explain why typical results are typical, theorize about anomalies, and show
  how results confirm or refute the hypothesis.
- Make experiments verifiable and reproducible; give enough detail for
  replication; consider releasing code.
- Report results fairly: never conceal failures; state failure as prominently as
  success; avoid reporting a lone success that looks like a fluke.
- Keep detailed experiment logs for yourself; sketch irrelevant or preliminary
  experiments only briefly.

## Refereeing

### Responsibilities
- Author: ensure correctness, presentation standard, and originality — this is
  the author's responsibility, not the editor's or referees'.
- Referee: be fair, objective, confidential, free of conflict of interest;
  review promptly; declare your limitations; recommend acceptance only when
  confident.
- Editor: choose referees, ensure prompt adequate reviewing, arbitrate
  disagreements and appeals, decide acceptance.
- Expect to referee roughly two to three times as many papers as you submit;
  decline only with good reason.

### Contribution
- Judge contribution (the main criterion) as originality + validity; it is
  defined by peer review.
- Weigh originality by likely effect — from breakthrough to tinkering or
  survey. Do not reject for obviousness: obvious-in-retrospect ideas can be
  excellent, and asking the right question counts.
- Require validity: intuition alone is not valid; require proof, analysis,
  modelling, simulation, or experiment (preferably several), with comparison to
  existing work.

### Evaluation of papers
- Confirm accuracy, originality, and proper credit; do not recommend acceptance
  without a caveat if you cannot assure quality.
- Ask: Is there a contribution? Is it significant, interesting, timely,
  relevant? Are results correct and critically analyzed? Are conclusions
  warranted? What is missing or unnecessary? Who is the audience? Is it clear
  and well presented?
- Identify the explicit or implicit hypothesis; if you cannot, something is
  likely wrong. Check whether all material is pertinent.
- Inspect the bibliography: too few references can signal bad scholarship; be
  suspicious of no major-venue citations; cite the refereed version over
  technical reports.
- Perform elementary nitpicking: spelling, syntax, English, bibliography errors,
  undefined terms, formula/math errors, inconsistencies. A few typos are
  expected; mixed-up subscripts suggest unchecked results.
- Distinguish rejection from "resubmit after major changes"; never use the
  latter as a "soft reject" with impossible demands.

### Referees' reports
- Serve the explicit purpose (editor's decision) and the implicit purpose
  (sharing expertise to help authors).
- Make a convincing case: for positive reviews give a clear statement of the
  contribution (not a summary); for negative reviews give a clear, evidenced
  explanation of faults.
- Give guidance: state changes needed to fix residual faults; for rejection,
  indicate how authors can proceed and which core (if any) is worthwhile.
- Check detail on acceptance — the referee is the last expert to see the paper.
- Be willing to change your mind as reading deepens; keep reviews constructive —
  positives matter as much as negatives; every paper has something to commend.
- Offer accessible, essential references; be polite, never patronizing or
  sarcastic; do not add secret criticisms invisible to authors.

### Ethics
- Refuse to referee where there is a real or apparent conflict of interest (same
  department; recent supervisor/student/co-author; close interaction;
  competition); return the paper promptly with an alternative suggestion.
- Base evaluation on the paper alone — not author or institution stature.
- Treat submitted papers as confidential: do not show them to colleagues or use
  them as a basis for your own research.

## Presentation of short talks

### Content
- Choose the single main goal — the one idea the audience should learn — then
  work out what must precede it; prune aggressively to essentials.
- Use "uncritical brainstorming, critical selection": first list everything
  (time-box it), then judge harshly.
- Ask what the audience *needs* to know, not what you want to tell. Keep it lean
  and leisurely, never crowded and hasty. Cut internals, full proofs, and
  implementation details unless they are the point.
- Never exceed the allotted time.

### Organization
- Design for linearity: the audience cannot skip back or pause; use backward and
  forward references and summaries at topic changes.
- Follow a logical sequence — subject, necessary background, experiments/results,
  conclusions — and make the structure apparent, keeping background visibly
  relevant.
- Distinguish essential from incidental material; say so when you skip important
  detail. Build in skippable end material to absorb timing variance.

### Introduction
- Begin well; first impressions form fast. Grab attention with a surprising
  claim, a challenge to intuition, or a practical consequence.
- State the goal before the structure; do not open by outlining the structure.
  - Bad: "This talk is about new graph data structures. I'll begin by explaining
    graph theory and show some data structures …"
  - Good: "This talk is about new graph data structures. There are many
    practical problems … such as the travelling salesman problem … But even
    these solutions are slow if the wrong data structures are used. I'll begin
    by explaining approximate solutions …"
- Always show title, your name, co-authors, and affiliation. Tell a story only
  if it motivates the problem and is certain to land.

### Conclusion
- End cleanly and signal the end; do not let it fade away.
  - Bad: "So the output of the algorithm is always positive. Yes, that's about
    all I wanted to say…"
- Revise the main points, outline future work, and consider an emphatic,
  logically-grounded statement (a prediction, recommendation, or judgement).

### Preparation
- Do not write the talk out in full or memorize it as a script; written English
  sounds stilted and reading prevents eye contact.
- Use large-print point-form prompts; rehearse enough that the right words come
  at the right time.
- Time the talk; note expected progress at 5, 10, … minutes. Rehearse to a
  mirror or tape, anticipate questions, learn the equipment, seek critical
  feedback.

### Overheads
- Use overheads as a focus of attention; aim for about one per minute.
- Make each self-contained with a heading; avoid rapid switching; repeat crucial
  information and notation; consider an evolving diagram or the whiteboard.
- Keep hardcopy sheets ordered, with paper between them; prefer landscape
  orientation.

### Text overheads
- Write point-form, brief summaries in short sentences; every point will be
  discussed.
- Never read overheads aloud — the audience reads faster and stops listening.
  - Bad: "Coding technique log-based, integer codes."
  - Good: "The coding technique is logarithmic but yields integer codes."
- Define all variables and simplify formulas; state variable types (crucial in
  talks). Never display a page from a paper. Use large fonts (uppercase ≥ 4 mm
  high), generous white space, an uneven right margin, and minimal clutter.

### Figures
- Make figures simple and uncluttered; avoid tables unless necessary.
- Exploit colour (orderings, entity types, routes to outcomes); shades of grey
  can be lost in reproduction.
- Label everything meaningful, horizontally, characters ≥ 4 mm; omit labels for
  material omitted from the talk.
- For each figure ask: does it illustrate a major point unambiguously? Is it
  self-contained, uncluttered, and fully legible?

### Delivery
- Speak clearly at a natural tone and volume; pace about 500 words per 3
  minutes; overemphasize consonants; keep your head up and face the audience.
- Avoid monotony; pause rather than fill gaps with "um". Be relaxed, vivid, even
  amusing, but never false or showy.
- Avoid distracting mannerisms: pacing, gesticulating, masking overheads,
  standing behind the projector, mumbling, laughing at your own jokes.
- Make frequent eye contact; vary activity; never diminish your achievements or
  announce the talk will be dull. Expect nerves — adrenaline helps.
- Point at the overhead, not the screen; remove your watch to check time
  discreetly; do not change overheads before the audience can read them.

### Audience and questions
- Treat silence as attention; the audience starts with goodwill — capitalise on
  it with a strong opening. Handle distractions tactfully; offer persistent
  interrupters a private conversation afterwards.
- Keep answers brief; do not debate one questioner at the expense of others.
- Never bluff — admit ignorance frankly; respond positively and honestly; never
  be rude or dismissive.
