# Writing style

## General guidelines

### Economy
- Make text taut: every sentence must be necessary; length must reflect content.
- Delete superfluous words, simplify sentence structure, establish logical flow.
- Revise frequently and critically; be egoless and ready to dislike your own
  prior text.
- Ask "what did I write that led the reader astray?" rather than "the referee
  is wrong."
- Do not over-condense — keep words that aid understanding.

Bad: "Bit-stream interpretation requires external description of stored
structures. Stored descriptions are encoded, not external."
Good: "Interpretation of bit-streams requires external information such as
descriptions of stored structures. Such descriptions are themselves data, and
if stored with the bit-stream become part of it so that further external
information is required."

### Tone
- Be objective, accurate, austere — not pompous, turgid, or convoluted.
- One idea per sentence/paragraph; one topic per section. Short words, short
  sentences, simple structure, short paragraphs.
- Avoid buzzwords, clichés, excess. Be specific, not vague or abstract.
- Use direct statements and active voice ("we"/"I") to distinguish new results.
- Casual/conversational is fine; slang and idioms are not.

Bad: "The system should be developed with the end users clearly in view. It
must therefore run the gamut from simplicity to sophistication, robustness to
flexibility…"
Bad: "The results show that, for the given data, less memory is likely to be
required by the new structure, depending on the magnitude of the numbers to be
stored and the access pattern."
Good: "The results show that less memory was required by the new structure.
Whether this result holds for other data sets will depend on the magnitude of
the numbers and the access pattern, but we expect that the new structure will
usually require less memory than the old."
Never use idioms: "crop up", "lose track", "it turned out that", "play up".

### Examples
- Use an example whenever it adds clarification, especially for fundamental
  concepts. Each example must illustrate one concept; if you cannot say what it
  illustrates, change it.
Good: "In a semi-static model, each symbol has an associated probability
representing its likelihood of occurrence. For example, if the symbols are
characters in text then a common character such as 'e' might have an associated
probability of 12%."

### Motivation
- Order the parts logically, and communicate that logic: add brief summaries at
  section start/end and linking sentences between sections.
- Never assume a series of definitions, theorems, or algorithms is
  self-explanatory — explain how each is used, why it is interesting, how it fits.
- Explain everything not common knowledge to the audience; decide what to teach
  the reader. Link text like a narrative.
Good: "Together these results show that the hypothesis holds for linear
coefficients. The difficulties presented by non-linear coefficients are
considered in the next section."

### The upper hand
- Write for the dullest of your readers, as an equal — never swagger.
- Cut egotistical showing off.
- Watch for: name-dropping philosophers; "the argument proceeds on Voltairian
  principles"; "analysis of this method is of course a straightforward
  application of tensor calculus"; unnecessary difficult mathematics; obscure
  citations.

### Obfuscation
- Be specific; avoid vague or convoluted terms that hide meaning.
- Do not exaggerate, omit relevant information, or state bold conclusions from
  flimsy evidence. Avoid stilted text and unnecessary formality.

Bad: "The status of the system is such that a number of components are now able
to be operated." → Good: "Several of the system's components are working."
Bad: "In respect to the relative costs, the features of memory mean that with
regard to systems today disk has greater associated expense…" → Good: "Memory
can be accessed more quickly than disk."
Bad: "there may be exceptions in some circumstances"; "data was transmitted
fast."

### Analogies
- Include an analogy only if it significantly reduces the work of understanding.
- Beware: analogies can take reasoning astray by masking fundamental
  differences; in computing papers there are more bad ones than good.

### Straw men
- Do not pose indefensible hypotheses just to demolish them. Contrast the new
  with the current, not the fictitious or impossibly bad.
- Do not attack the ancient — later work has probably improved on it.

Bad: "it can be argued that databases do not require indexes."
Bad: "Before then data was kept in filing cabinets… queries were verbal, which
led to many mistakes… Such mistakes are impossible with new query languages."

### Reference and citation
- Relate new work to existing work; show how it builds on and differs from
  prior results.
- Include a reference only if it serves the reader: relevant, up to date,
  reasonably accessible, necessary. Prefer the original to a secondary source;
  good over bad; journal over conference; conference over technical report or
  manuscript (unrefereed).
- Avoid private communications and talks; if unavoidable, use a footnote or the
  acknowledgements, not a bibliography entry.
- Do not cite common knowledge. Substantiate claims and prior-work discussion.
- Avoid gratuitous self-reference.
- Describe others' results fairly and accurately; neither belittle nor overstate.

Bad: "Robinson's theory suggests that fast access is possible, but he did not
perform experiments to confirm his results [22]."
Good: "Robinson's theory suggests that fast access is possible [22], but as yet
there is no experimental confirmation."
Bad: "Most users prefer the graphical style of interface."
Good: "We believe that most users prefer the graphical style of interface."

### Citation style
- Name references that are discussed; never leave them anonymous, especially
  self-references.
- Prefer ordinal-number style; name-and-date or superscript are also common.
  Avoid uppercase codes like "[MAR91]".
- Use "et al." for more than three authors in text; give all authors in the
  reference list.
- Format fields of the same type consistently, and give complete details:
  - Journal: full name, authors, title, year, volume, number, pages, month.
  - Conference: full name, authors, title, year, pages.
  - Book: title, authors, publisher, address, year, edition, volume, pages.
  - Tech report: title, authors, year, report number, publisher address,
    electronic address.

Bad: "Other work [16] has used an approach in which…"
Good: "Marsden [16] has used an approach in which…"
Bad: "Rowers, Mann, Thompson, and Wills [9] provide another example."
Good: "Rowers et al. [9] provide another example."

## Specifics

### Titles and headings
- Be concise, informative, specific; accurately describe the content. Brevity
  is not vagueness. Accuracy over catchiness — the title is what most people see.
- Titles and headings need not be complete sentences. Reflect logical structure;
  make sibling subsections parallel.
- Use only two heading levels; number major headings only. Do not over-split
  (three headings per page is too many) or use too few sections.

Bad: "A New Signature File Scheme based on Multiple-Block Descriptor Files for
Indexing Very Large Data Bases" → Good: "Signature File Indexes Based on
Multiple-Block Descriptor Files"
Bad: "Duplication of Data Leads to Reduction in Network Traffic" → Good:
"Duplicating Data to Reduce Network Traffic"

### The opening paragraphs
- Write the abstract especially well; make the opening sentence direct.
- Make first paragraphs intelligible to any likely reader — describe what you
  did, not how. Provide context before stating the contribution.
- Distinguish description of existing knowledge from the paper's contribution.
- The paper must stand complete without the abstract; do not let the
  introduction read as a continuation of it.

Bad: "This paper does not describe a general algorithm for transactions."
Good: "General-purpose transaction algorithms guarantee freedom from deadlock
but can be inefficient. In this paper we describe a new transaction algorithm
that is particularly efficient for a special case, the class of linear queries."
Bad: "Underutilization of main memory impairs the performance of operating
systems."
Good: "Operating systems are traditionally designed to use the least possible
amount of main memory, but such design impairs their performance."

### Variation
- Vary organization, structure, sentence/paragraph length, and word choice to
  hold attention.

### Paragraphing
- One topic per paragraph; capture the gist in the opening sentence, then
  amplify. Keep every sentence related to the announced topic.
- Break long paragraphs; vary length — do not chop into uniform blocks.
- Restate references across paragraph boundaries ("The fast sorting
  algorithm…", not "This algorithm…").
- Link paragraphs by reusing key words and connective expressions.
- Use lists sparingly, for important material that needs enumeration; use tags,
  numbers only when order matters. Avoid childish symbols.

### Sentence structure
- Keep sentences simple — no more than a line or two; do not say too much at once.
- Avoid nested sentences; move parenthetical content to a separate sentence.
  Keep "if" conditions together. Beware misplaced modifiers and double negatives.
- Replace "and"/semicolon with a period if there is no reason to join.

Bad: "We collated the responses from the users, which were usually short, into
the following table."
Good: "The users' responses, most of which were short, were collated into the
following table."
Bad: "If the machine is lightly loaded then speed is acceptable whenever the
data is on local disks."
Good: "If the machine is lightly loaded and data is on local disks then speed
is acceptable."

### Repetition and parallelism
- Avoid monotonous repeated sentence forms; watch sequences beginning
  "however", "moreover", "therefore", "hence", "thus", "and", "but", "then",
  "so", "nevertheless", "nonetheless". Do not overuse "First,… Second,… Last,…".
- Explain complementary concepts as parallels. Match flags ("on the one hand" ↔
  "on the other hand"; "One…" ↔ "Another…"). Use parallel structure in lists;
  move longer clauses to the end of a list.

Bad: "To achieve good performance there should be sufficient memory, parallel
disk arrays should be used, and caching."
Good: "Achievement of good performance requires sufficient memory, parallel
disk arrays, and caching."

### Direct statements
- Avoid excessive passive/indirect voice, especially with no actor.
- Use active voice and "we" to distinguish contributions and simplify. Do not
  imply a paper is sentient ("this paper shows"). Replace artificial verbs.

Bad: "The following theorem can now be proved."
Good: "We can now prove the following theorem."
Bad: "Tree structures can be utilized for dynamic storage of terms."
Good: "Terms can be stored in dynamic tree structures."
Watch for: perform, utilize, achieve, carry out, conduct, done, occurred,
effected. Prefer "we show" over "in this paper it is shown that".

### Ambiguity
- Check carefully; you cannot detect ambiguity in your own text because you know
  the intent. A clumsy sentence is preferable to an ambiguous one.
- Give pronouns ("it", "this", "they") clear referents. Distinguish speed from
  time — "increasing speed" can read as increasing time.

Bad: "The compiler did not accept the program because it contained errors."
Good: "The program did not compile because it contained errors."
Bad: "In addition to skiplists we have also tried trees. They are superior…"
Good: "In addition to skiplists we have also tried trees. Skiplists are
superior because…"

### Emphasis
- Sentence structure places implicit stress; reorganize to put stress where the
  meaning is. Do not italicize unnecessarily or use capitals for emphasis.
- Explain new terms at first use, by structure or a one-word italic.

Bad: "Additional memory can lead to faster response, but user surveys have
indicated that it is not required."
Good: "Faster response is possible with additional memory, but user surveys
have indicated that it is not required."

### Definitions
- Define or explain terminology, variables, abbreviations, and acronyms at
  first appearance, in a consistent format; emphasize/italicize first use.
- Use a discursion or negative examples to motivate a definition.

### Choice of words
- Prefer short, direct words; use an exact long word over an approximate short
  one. Be precise ("difficult to compute" = slow? memory-hungry?).
- Do not cycle synonyms to avoid repetition — technical terms must stay
  consistent. Use a word only if you know its meaning. Avoid slang and
  contractions ("cannot", not "can't").
- Avoid superlatives and excessive claims ("our method is an ideal solution").

Use: "begin" not "initiate"; "first" not "firstly"; "part" not "component";
"use" not "utilize".

### Qualifiers
- At most one of might/may/perhaps/possibly/likely/could per sentence.
- Avoid "very" and "quite" entirely; delete "simply"; avoid double negatives.

Bad: "It is perhaps possible that the algorithm might fail on unusual input."
Good: "The algorithm might fail on unusual input."
Bad: "There is very little advantage to the networked approach."
Good: "There is little advantage to the networked approach."

### Padding
- Delete pedantic phrases. Watch for: "the fact that", "in general", "it can be
  seen that", "it is a fact that", "of course" (patronizing), phrases with
  "case". "note that" is acceptable only to introduce a deductive consequence.

### Misused words
- that (defining) vs which; can (capability) vs may (permission/possibility);
  less (continuous) vs fewer (discrete); affect (verb) vs effect (noun);
  conversely (only true opposites); similarly/likewise (only strong parallels);
  optimize = find the optimum, not merely improve; alternate vs alternative;
  basic (elementary) vs fundamental; conflate vs merge; continual (ceaseless)
  vs continuous (unbroken); fast/quickly (speed) vs timely (opportune);
  presently (soon) vs currently (at present).

Bad: "There is one method which is acceptable." → Good: "There is one method
that is acceptable."
Good: "Users can access this facility, but may not wish to do so."

### Spelling conventions
- Be consistent in "-ise"/"-ize" and follow the target journal's standard.
- "disk"/"disc": both common — pick one. "enquire"/"inquire",
  "biased"/"biassed", "dispatch"/"despatch" are unstable.
- Commonly misspelt: apparent, argument, consistent, definite, existence,
  foreign, grammar, heterogeneous, homogeneous, independent, occurred,
  participate, preceding, primitive, propagate, referred, separate, supersede,
  transparent.

### Jargon
- Use specialised vocabulary for specialists, but know it shrinks the audience.
- Be cautious when common words are given new meanings ("record", "function").
  Use new terminology consistently; avoid ridiculous modifier stacks.

Bad: "The transaction log is a record of changes to the database."
Good: "The transaction log is a history of changes to the database."

### Foreign words
- Prefer an English equivalent. Use the appropriate characters for foreign names.

### Overuse of words
- Eliminate repetition that makes the reader feel they have read the same
  phrase twice. Do not use the same word in different senses, or a word plus its
  synonym together. Watch tics: "so", "also", "hence", "note that", "thus",
  "this", "very".
- Repetition is fine for technical terms — always describe a concept the same way.

### Redundancy and wordiness
- Use the minimum number of shortest words.
- "added together" → "added"; "after the end of" → "after"; "in the region of"
  → "approximately"; "cancel out" → "cancel"; "currently…today" → "currently";
  "divided up" → "divided"; "give a description of" → "describe"; "during the
  course of" → "during"; "first of all" → "first"; "for the purpose of" → "for";
  "joined up" → "joined"; "of large size" → "large"; "merged together" →
  "merged"; "the vast majority of" → "most"; "completely optimized" →
  "optimized"; "separate into partitions" → "partition"; "reason why" →
  "reason"; "a number of" → "several"; "completely unique" → "unique"; "in the
  majority of cases" → "usually"; "whether or not" → "whether"; "the fact that"
  → delete.

### Tense
- Present for eternal truths ("the algorithm has complexity O(n)") and statements
  about the text ("related issues are discussed below").
- Past for describing the work and its outcomes.
- Either tense for discussing references (present preferred); future rarely,
  except in conclusions.

Good: "Although the algorithm has worst-case complexity O(n²), in our
experiments the worst case observed was O(n log n)."

### Plurals
- Convert plurals to singulars where reasonable; excessive plurals confuse.
- Prefer modern forms: schemas, indexes, formulas (but radii, matrices persist).
- "data" serves as both singular and plural.

Bad: "Packets that contain an error are automatically corrected."
Good: "A packet that contains an error is automatically corrected."

### Abbreviations
- Expand "no.", "i.e.", "e.g.", "c.f.", "w.r.t." to "number", "that is", "for
  example", "compared with"/"in contrast to", "with respect to".
- Expand "Fig.", "Alg."; write "first", not "1st"; do not abbreviate months.
- Explain every abbreviation/acronym at first use. Avoid "etc."; use an ellipsis
  only in quotations. Do not use slashes ("and/or", "list/tree") — they are
  ambiguous.

### Acronyms
- Use acronyms for long names (DNA) and frequently-used sequences (CPU).
- Do not introduce one unless it will be used frequently.
- No stops in acronyms ("CPU" correct; "C.P.U." pedantic; "CPU." incorrect).
- Plurals take no apostrophe ("CPUs", not "CPU's").

### Sexist language
- Avoid expressions that unnecessarily specify gender. Never use "s/he" or
  reverse sexism ("she"); recast the sentence.

Bad: "A user may be disconnected when he makes a mistake."
Good: "A user who makes a mistake may be disconnected." (Singular "they" is
acceptable but jarring.)
