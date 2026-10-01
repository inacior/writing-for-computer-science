# Graphs, figures, tables, and algorithms

## Illustrations (overview)
- Use illustrations only for matter central to the paper; they attract
  attention, so do not dilute with marginal figures.
- Number every figure and give a descriptive caption so it is as self-contained
  as possible.
- Introduce and discuss each illustration, just before or on the page where it
  appears. Omit any illustration you have nothing to say about.
- Obtain permission and credit the original author, source, and copyright when
  reusing a figure.

## Graphs
- Present numerical results with graphs, not number dumps; use numbers
  sparingly. Select data because it is evidence for a hypothesis, not because a
  program emitted it.
- Limit to about three or four graphs; ten is almost certainly too many. Push
  detailed tables to an appendix or omit transient numbers.
- Keep graphs simple: few lines, minimal clutter. Put the varied parameter/input
  on the x-axis; the function/output on the y-axis.
- Mark discrete data points with distinctive symbols (circles, boxes, triangles);
  do not use ticks or crosses.
- Keep lines, axes, and elements of similar thickness; do not pair a bold font
  with lightly drawn lines. Make axis ticks slightly lighter.
- Use sufficiently distinct grey shades; lighter lines may need to be thicker.
- Use logarithmic axes to show behaviour across orders of magnitude and for
  problem-size-vs-time plots (different growth rates become straight lines of
  different slope).
- For more than two interacting parameters: if A and B both depend on C, plot C
  on x with two y-axes. For three-dimensional relationships, hold one variable
  fixed and choose a representative value.
- Data that seems tabular may still suit a graph; for unordered items use a bar
  graph — do not join points with lines (implies a functional relation).
- To compare methods, keep separate graphs consistent and directly comparable.
- Put white space between values and units (`11.2 Kbytes`); hyphenate a
  number+unit used as an adjective (`the 2.7-Kb input`).

## Diagrams (schematics)
- Use diagrams to show a structure, a process, or a state — do not mix these
  purposes (e.g., data flow and control flow) in one diagram.
- Develop with preliminary hand sketches; balance proportion (about half again
  as wide as high); use space well; avoid bunching.
- Never submit hand-drawn diagrams unless professionally prepared.
- Keep the diagram open, not too dark; it need not be faithful to every detail.
- Label horizontally, at a size similar to body text; use at most two or three
  fonts/sizes; lines no heavier than a little thicker than the text font.
- Be consistent: same arrow/line kind = same meaning. Distinguish arrow types
  with dashed vs solid lines.

## Tables
- Use tables for data unsuitable for graphs: dataset properties, or where exact
  values matter. Do not use a table to show function values across points (a
  graph is better), except for a function with only two or three values.
- Design hierarchically: simple tables have column headings and row stubs;
  complex tables partition columns/rows, span headings, and share labels.
- Indicate hierarchy with double lines, single lines, or white space — not dense
  rules.
- Keep items below a column head of the same kind; items right of a row label
  must all be properties of that label.
- Leave the top-left corner blank if the label column has no heading.
- Do not rule between every row/column; do rule between groups of rows.
- Do not make tables too dense. Avoid blank positions (use a dash for "not
  applicable" and explain it).
- Align numbers on the decimal point; values with different units need not align
  or share precision.
- State units in labels: `Size (bytes)`, not `Size`.
- Small tables may sit in running text like displayed math; larger tables are
  labelled and placed at the top or bottom of a page.
- Do not rely on a table to convey essential information; graphs or text are
  preferable.

Typical bad table: all elements at one level, case used to separate headings
from content, inconsistent units and precision, units not factored out,
unnecessary first-column heading, too many horizontal lines.
Typical good table: no vertical lines, like rows adjacent for comparison, units
factored out, different units not aligned or forced to shared precision.

## Captions and labels
- Make captions informative; prefer more descriptive captions that explain the
  major elements. Use minimum capitalization for descriptions.
- Use the caption for self-contained detail: parameter values, expansions of
  abbreviations and notation used in headings.
  - Bad: `Figure 5. Fan data structure.`
  - Good: `Figure 5. Fan data structure, of lists with a common tail. The
    crossed node is a sentinel. Solid lines are within-list pointers. Dotted
    lines are inter-list pointers.`
- Expand abbreviated terms naturally in the discussing text rather than listing
  what each abbreviation stands for.

## Algorithms

### Presentation and content
- Demonstrate the algorithm is worthwhile: show correctness (given appropriate
  input it terminates with appropriate results) and that it meets its claimed
  performance bound — by proof, experiment, or both.
- Clarify the scope of any "better" claim (worst vs average case; time vs space;
  asymptotic vs practical constant factors) — "better" is vague.
- Be explicit about the kind of contribution: new/better computation (complexity
  analysis expected); explanation of a complex process (argue the steps are
  effective); or feasibility/decidability (formal correctness essential).
- State, where applicable: the steps; input/output and internal data structures;
  scope and limitations; correctness properties (preconditions, postconditions,
  loop invariants); a correctness demonstration; a complexity analysis (space
  and time); experiments confirming the theory.
- When a formal demonstration is absent, make the reason clear.
- Do not use flowcharts — poor modularity, encourage goto, no room for
  explanatory text or complex conditions.

### Formalisms
- **List style:** numbered/named steps with "go to step X" loops. Allows full
  discussion, but control structure becomes obscure.
- **Pseudocode:** block-structured, each line numbered. Structure is obvious,
  but statements are terse and comments are hard.
- **Prosecode (preferred):** number each step, never break a loop over several
  steps, subnumber step parts, include explanatory text. Describe input/output
  in the preamble; mix statements and text.
- **Literate code:** introduce detail gradually, intermingled with ideas,
  analysis, and correctness proof — most verbose but usually clearest.
- Use `←` for assignment (unambiguous, unlike `=`).
- Discuss the key ideas before giving the algorithm; most worthwhile algorithms
  need substantial explanation beyond a page or two.

Bad (over-specified loop): step-by-step expansion of a summation with nested
loops and index arithmetic.
Good: state the summation with `Σ` and `Π` and assume readers know how to
implement sums and products.

### Notation
- Prefer mathematical notation to programming notation: write `xᵢ`, not `x[i]`.
- Do not use `*` or `x` for multiplication; use `×` or `·`, or implicit
  multiplication.
- Avoid language-specific constructs (`a <<= 0`, `a++`, `for(i=0;i<n;i++)`) —
  unclear or wrong to unfamiliar readers.
- Omit `begin`/`end`; show nesting by indentation or numbering.
- Use set notation, subscripts/superscripts, `Σ`, `Π`, but respect their formal
  meanings.
- Take care with multi-character variable names (`pq` may read as `p × q`).
- Do not include full program text; provide code separately if needed.
- Use English when it is sufficiently clear.
  - Bad: `for 1 ≤ i ≤ |s|: set c ← s[i]; set A_c ← A_c + 1`
  - Good: `For each character c in string s, increment A_c.`

### Level of detail and figures
- Specify in enough detail to allow implementation "without undue inventiveness",
  but no more.
- Make explicit any step whose implementation greatly affects behaviour, but do
  not over-specify.
- Use figures to convey the intricacies of data structures.

### Environment
- Describe the algorithm's environment: data structures, input/output types,
  and sometimes OS/hardware properties (e.g., disk characteristics).
- Keep hardware assumptions realistic. Specify all variable types except trivial
  counters. Describe expected input and output without assuming correctness;
  state limitations and unhandled errors; most importantly, say what the
  algorithm does.
- Describe data structures with simple mathematical notation (e.g., "each
  element is a triple (string, length, positions)").
- When presenting several algorithms for the same task, define them over the
  same input/output where possible; make capability differences explicit.

### Performance
- State the basis of evaluation explicitly: which criteria — functionality or
  speed? asymptotic or typical data? real or synthetic data?
- Compare new techniques to a well-known standard; ensure the basis does not
  appear to favour your algorithm.
- Justify non-trivial simplifying assumptions. Give some absolute indication of
  time; label model-based vs experimental times.
- Treat measured CPU time as an estimate (fixed quantum fractions, allocated by
  heuristics). Specify memory use; consider time/memory trades.
- For disk/network traffic, account for first-bit (seek/latency) and transfer-rate
  components separately; consider caching and repeat accesses.
- Do not compare resource requirements of algorithms that perform subtly
  different tasks.

### Asymptotic complexity
- Explain how the algorithm behaves as problem scale changes.
- Define terms precisely: f(n) is O(g(n)) if f(n) ≤ c·g(n) for all n > k;
  o(g(n)) if f(n) < c·g(n); Ω for lower bounds, Θ for tight bounds. Define your
  usage, as authors differ. Informal big-O is acceptable but avoid ambiguity —
  state which complexity you mean.
- Include construction cost for static data structures (binary search is
  O(log n), but sorting first is O(n log n)).
- Make the analysis domain clear and analyze the right component. For integer
  arithmetic, choose a cost model (unit cost, or cost in bits).
- Watch that the dominant cost may change with scale, and that the theoretical
  dominant cost may never dominate in practice (O(n log n) comparisons vs O(n)
  disk accesses).
- Recognize when formal analysis is inappropriate: for rarely-large inputs,
  typical-case behaviour may matter more than the limit.
- Analysis is no more reliable than its assumptions and says nothing about
  constant factors or practical CPU/cache/bus/disk interactions — experiments
  are needed to confirm, and analysis cannot replace them (nor they it).
