# Punctuation and mathematics

## Punctuation

### Fonts and formatting
- Use at most three fonts (plain, italic, bold), or four with a fixed-width
  font for program text; use non-plain fonts sparingly.
- Prefer italic to bold for emphasis; bold is distracting. Never underline for
  emphasis (obsolete).
- Eliminate visual clutter: boxes, icons, excessive parentheses/quotes/italics/
  uppercase.
- Use indentation to mark paragraphs and to offset quotes, programs, and
  displayed math; do not substitute blank lines (meaning is lost at page breaks).
- Signal topic changes with headings, not blank lines.
- For submissions: wide margins, decent font size, page numbers, a running
  header, and follow the journal's "Information for Authors".

### Stops (periods)
- End sentences with stops; use other marks for variety — stops alone read
  telegrammatically.
- Omit the sentence's stop when an abbreviation ending in a stop ends the
  sentence.
- Do not put a stop at the end of a heading.
  - Bad: `3. Neural Nets for Image Classification.`
  - Good: `3. Neural Nets for Image Classification`

### Commas
- Use commas to mark pauses, aid parsing, form lists, and mark parenthetical
  (comment) phrases rather than qualifiers.
- Distinguish restrictive from parenthetical with paired commas:
  - `the four processes that use the network are almost never idle` = of the
    processes, only the four that use the network are idle.
  - `the four processes, which use the network, are almost never idle` = all
    four use the network and are idle.
- Include both commas of a parenthetical pair; omitting the first is a common
  error.
  - Bad: `The process may be waiting for a signal, or even if processing input,
    may be delayed by network interrupts.`
  - Good: `The process may be waiting for a signal, or, even if processing
    input, may be delayed by network interrupts.`
- Use the minimum commas for disambiguation, but never so few as to create
  ambiguity.
  - Bad: `Using disk tree algorithms were found to be particularly poor.`
  - Good: `Using disk, tree algorithms were found to be particularly poor.`
  - Bad: `One node was allocated for each state, but of the nine seven were not
    used.`
  - Good: `One node was allocated for each state, but, of the nine, seven were
    not used.`
- Keep the serial (Oxford) comma in lists; omitting the last comma rarely adds
  clarity and often damages it.
- Rewrite comma-heavy ("strangulated") sentences; split them.
  - Bad: `The process required less than a second (except when the machine was
    heavily loaded, the network was saturated, etc.).`
  - Good: `The process required less than a second (unless, for example, the
    machine was heavily loaded or the network was saturated).`

### Colons and semi-colons
- Use colons to join related statements and to introduce lists.
  - Good: `These small additional structures allow a large saving: costs are
    reduced from O(n) to O(log n).`
- Use semi-colons to separate list elements that themselves contain commas.
  - Good: `There are three phases: accumulation of distinct symbols in a hash
    table; construction of the tree, using a temporary array to hold the symbols
    for sorting; and the compression itself.`
- Use a semi-colon to divide a long sentence or set off emphasis. Do not overuse
  either mark.

### Apostrophes
- Singular possessives: apostrophe + s (`student's algorithm`, `Gowers's book`).
- Plural possessives: apostrophe only (`students' passwords`).
- Pronoun possessives: no apostrophe (`its speed`, `hers`).
- Contractions take an apostrophe (`it's`, `can't`), but avoid contractions in
  technical writing. `it's` = "it is"; `its` = possessive.

### Exclamations
- Avoid exclamation marks; never use more than one. Prefer restructuring for
  emphasis.
  - Acceptable: `Performance deteriorated after addition of resources!`
  - Better: `Remarkably, performance deteriorated after addition of resources.`

### Hyphenation
- Be consistent among transitional forms (`bit slice`/`bit-slice`/`bitslice`).
- Use hyphens to override right associativity and disambiguate:
  - `randomized data structure` parses as randomized data-structure.
  - `skew-data hashing` needs the hyphen (or rewrite: "hashing for skew data").
  - Write `hash-based data structure`; rewrite `binary tree based data
    structure` as `data structure based on binary trees`.
- If no correct hyphenation exists, rewrite the sentence.
- Check automatic end-of-line hyphenation: break at syllables, not near a word's
  end.
- Distinguish three dashes: hyphen `-` (joining), en-dash `–` (minus/ranges,
  e.g. `pages 101–127`), em-dash `—` (parenthetical break).

### Capitalization
- Capitalize only proper names; use lower case for common-use names.
- Follow programming-language conventions: `FORTRAN`, `Prolog`, `APL`; `lisp`
  and `pascal` are incorrect.
- Capitalize technical object labels: `Theorem 3.1`, `Figure 4`, `Section 11`.
- Choose maximum or minimum heading capitalization and be consistent; never mix
  maximal sections with minimal subsections.
  - Minimal: `The use of jump statements: Advice for Prolog programmers`
  - Maximal: `The Use of Jump Statements: Advice for Prolog Programmers`
- Apply the same rules to captions and reference titles.

### Quotations
- Place punctuation inside quotation marks only if it belonged to the original;
  otherwise put it outside.
  - Good: `Crosley [14] argues that "open sets are of insufficient power", but
    Davies [22] disagrees.`
- For literal strings, especially code, keep punctuation outside:
  - Bad: `One of the reserved words in C is "for."`
  - Good: `One of the reserved words in C is "for".`
- Use typographic quotes, not ASCII double quotes.

### Parentheses
- Punctuate a sentence containing a parenthetical exactly as if the
  parenthetical were removed; punctuate the parenthetical independently.
  - Bad: `Most quantities are small (but there are exceptions.)`
  - Good: `Most quantities are small (but there are exceptions).`
- Keep parentheticals to true asides; never bury important text there. At most
  one per paragraph, a couple per page. Never nest parentheses. Avoid `(s)` for
  optional plurals.

### Citations
- Punctuate citations as parenthetical remarks.
  - Bad: `In [2] such cases are shown to be rare.`
  - Good: `Such cases have been shown to be rare [2].` / `Wilson [2] has shown
    that such cases are rare.`
- Never treat a bracketed expression as a word (never produce `In2`).
- Place the citation close to the material it supports.

## Mathematics

### Clarity and precision
- Be precise, especially in fundamental definitions; ambiguity in a theorem
  makes its proof incomprehensible.
- Do not misuse terms with fixed mathematical meanings; prefer `usual` to
  `normal`. Use `definite`, `strict`, `proper` only mathematically; be careful
  with `all` and `some`.
- Restrict `intractable` to NP-hard. Distinguish `formula` from `equation` (the
  latter involves equality). Use `equivalent` only for indistinguishability;
  otherwise `similar`. Use `element` only for a member of a set/list/array.
- `Partitioned` subsets are disjoint and union to the original set. Use
  `average` formally (arithmetic mean) or say `mean`.
- English-specified orderings are nonstrict: `A is a subset of B` means A ⊆ B;
  use `strict subset` for A ⊂ B.

### Theorems and proofs
- Write theorems to be as independent of surrounding text as possible; readers
  skim and may quote them verbatim.
- Number definitions, theorems, lemmas, and propositions; reference by number,
  not by location.
- For complex proofs, state the main theorem first, then state and prove lemmas
  before the main proof — or use heavy motivation and examples.
- Explain a long proof's structure before its details, and relate each part to
  that structure. Omit mechanical algebra the reader will not value.
- Keep logical gaps completable mechanically, without invention.
- Mark the end of a proof/example/definition with a symbol such as a box.

### Readability
- Set variables in italic; write function names (`log`, `sin`) upright.
- Delimit expressions with parentheses or brackets; avoid braces (confused with
  sets). Size parentheses a little taller than their contents.
- Structure sentences with embedded math as if each formula were a phrase; do
  not start a sentence with a formula.
  - Bad: `P ⊢ q₁ ∧ … ∧ qₙ is a condition`
  - Good: `The dependency P ⊢ q₁ ∧ … ∧ qₙ is conditional.`
- Give the type of each variable at every use.
  - Bad: `The values are represented as a list of numbers L.`
  - Good: `The values are represented as a list L of numbers.`
- Avoid ambiguous forms like `a/b + c`. Break down expressions to enlarge small
  symbols.
  - Bad: `For each xᵢ, 1 ≤ i ≤ n, xᵢ is positive.`
  - Good: `Each xᵢ, where 1 ≤ i ≤ n, is positive.`
- Do not let math replace text; readers get lost in a stream of expressions.

### Notation
- Use symbols the reader will know; do not substitute symbols (`∀`, `∃`, `⇒`)
  for words, and do not verbalize simple symbols (`a ≤ b`).
- Do not confuse `≈`, `≅`, `~` with `=`.
- Never reuse notation; keep meanings consistent. Adopt conventions (`i`, `j`
  for integer subscripts; uppercase for sets) and keep them.
- Vertically align equality signs; display important formulas consistently
  (centred or indented). Display positive results, not counter-examples, so
  skimmers are not misled. Number important formulas.
- Keep math symbols the same font size as text. Avoid unnecessary or piled
  subscripts (`x_{k_i}`) and mixed sub/superscripts (`x_i^k`).
- Prefer set notation: `Σ_{w∈W} f_w` over `Σ_{i=1}^n f_{w_i}`.
- Avoid multiple accents and piled primes; never use handwritten symbols.

### Alphabets
- Greek letters add clarity because they cannot form English words; do not
  overuse. Minimize unfamiliar letters and new notation.
- Prefer letters whose names are known (so readers do not invent names).
- Watch superficially similar symbols (ζ/e, ξ/n, μ/u, ρ/p, υ/v, ω/w, α/a,
  φ/¢, ∅).

### Ranges and sequences
- Closed range `[a, b]`; open `(a, b)`; half-open `[a, b)` and `(a, b]`.
- Use ellipsis for integer sequences: `m, …, n`. For infinite sequences, list
  initial values and state the pattern. Always give both bounds. Replace
  `1 ≤ i ≤ 6` with `i = 1, …, 6` when integrality is not obvious.

### Line breaks
- Do not let a number, symbol, or abbreviation start a line.
  - Bad: `… in about 12` [newline] `ms using our techniques.`
  - Good: `… in about 12 ms` [newline] `using our techniques.`
- Use a non-breaking space; rewrite surrounding text when a formula cannot break
  cleanly.

### Numbers
- Write numbers as figures, except: approximate numbers; numbers up to twenty
  unless a literal value or measurement; and numbers starting a sentence (recast
  instead). Always write percentages in figures. Do not mix modes.
  - Bad: `There were between four and 32 processors in each machine.`
  - Good: `There were between 4 and 32 processors in each machine.`
- Group long digits with thin spaces (`1 897 600`), not commas.
- Never omit a leading 0 (`0.3 Kb`, not `.3 Kb`).
- Avoid "orders of magnitude"; state explicit factors.
  - Bad: `at least two orders of magnitude faster`
  - Good: `at least a hundred times faster`
- Give values of the same units to the same precision. Do not imply false
  accuracy; flag approximations with "roughly", "nearly", "approximately",
  "over". Write fractions as words.

### Percentages
- Use percentages with caution; avoid ambiguous ones.
  - Bad: `The error rate grew by 4%, from 52% to 54%.`
  - Good: `The error rate grew by 2%, from 52% to 54%.`
- State what a percentage is of. Prefer percentages to odds for probabilities.
- Do not describe small samples as percentages; that overstates authority.

### Units of measurement
- Time: second (sec), minute (min), hour (hr); abbreviated forms are unusual in
  running text. Spell out ambiguous sub-second units at least once (ms/msec,
  µs/µsec, ns/nsec). Separate hours/minutes with a colon.
- Space: bit and byte; larger units scale in powers of 2 (Kb 2¹⁰, Mb 2²⁰, Gb
  2³⁰, Tb 2⁴⁰, Pb 2⁵⁰, Eb 2⁶⁰).
- If `Mb` could read as megabit, write `Mbyte` or `megabyte`; spell out large
  units at least once. Prefer explicit rates (`18 Mb/sec`).
- Prefer seconds over minutes (avoids `1.50 minutes` ambiguity; eases
  comparison). Avoid ill-defined units like MIPS.
- Use plural units for quantities greater than 1, singular below: `1.3 seconds`
  but `0.8 second`. Typeset units in the text font, even inside math.
