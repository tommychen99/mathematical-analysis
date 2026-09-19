# Lecture Notes on Mathematical Analysis

Repository: <https://github.com/tommychen99/mathematical-analysis>

## Single and Multivariable Calculus

**Author:** Tommy Chen

**Current version:** Version 3.29.0

**Revision date:** September 19, 2026

**Status:** Focused pedagogical and organizational revision of the authoritative
Version 3.28.0 working tree. Chapter 8 now separates Taylor theory, the
exponential/logarithmic development, and trigonometry. Part II retains its
architecture, with the requested Chapter 10 compactness clarification.
Appendices A–I remain optional.

These notes give a rigorous introduction to real analysis and rebuild the
central ideas of calculus from modern foundations. Part I develops the real
numbers, sequences, limits, continuity, series, differentiation, and Riemann
integration. Part II develops the finite-dimensional topology and linear
algebra needed for multivariable analysis, followed by multivariable
integration, classical line and surface integrals, Green and patch Stokes,
differential forms, manifolds, and the general Stokes theorem.

## Version 3.29.0 — September 19, 2026

This revision preserves the current sources, figures, exercises, labels, and
prior revision history, including the uncommitted Version 3.28.0 work. It does
not undertake the deferred broad Part II revision.

- Chapter 4 reuses monotone convergence in Bolzano–Weierstrass and adds three
  elementary variants of the sequential definition of e.
- Chapter 5 distinguishes equation roots from principal radicals, motivates
  rational exponents through exponent laws, explains the negative-base
  representation obstruction, and keeps root continuity near construction.
- Chapter 8 has nine numbered sections: derivatives; chain and mean value
  theorems; differentiating limits and series; higher derivatives and Taylor;
  exponential, logarithm, and real powers; trigonometry and inverse branches;
  curves and polar coordinates; smooth cutoff; convexity and nondifferentiability.
  Taylor order zero is explicitly linked to the MVT, with rigorous error and
  asymptotic examples after the relevant functions are constructed.
- The exponential development preserves the proof that exp(1) equals the
  sequential e and rational-power compatibility, then develops a worked
  family of hidden exponential limits. Geometric trigonometry motivates the
  analytic construction without being used as an unproved premise.
- Chapter 10 defines compact subsets using containment in ambient open covers
  and proves equivalence with subspace compactness, simplifying two proofs.
- Appendix A corrects the Hartogs relation coding and makes stopping in the
  transfinite recursions precise. Appendix B adds concrete category, functor,
  opposite-arrow, and diagram examples within its existing narrow scope.
- Appendix F synthesizes slices, graphs, and regular levels, and compares
  immersions with embeddings. Appendix G linearizes multiplication and
  inversion, consolidates its example Lie algebras, and uses exp(A) as the
  primary matrix-exponential notation.
- Appendix H adds a geometric first-reading route, the radial one-form
  prototype, an exact-sequence prototype, a two-arc Mayer–Vietoris figure,
  and the de Rham naturality square. Cubical integration is explicitly
  distinguished from the later simplicial model.
- Appendix I extends selected strategic hints to A–H, with higher density in
  F–H. A superscript asterisk continues to mean “hint available,” not difficulty.
- A selective typography pass extracts related formulas from dense prose;
  substantive Part II architecture and the optional status of the appendices
  are preserved.

### Foundations status

Appendix A states the recursion and transfinite-recursion principles without
proof, proves Hartogs’s lemma, and proves the equivalence of AC, the
Well-Ordering Theorem, and Zorn’s Lemma using those foundations.

### Validation

The final `main.pdf` contains 508 pages. Repeated pdfLaTeX builds stabilized
`main.aux`, `main.toc`, and `main.out`; the final log contains no LaTeX
warnings or overfull/underfull boxes. The rendered revised pages were
visually inspected, including the contents, Taylor and inverse-function
displays, category and exact-sequence diagrams, Lie-group matrices, the
Mayer–Vietoris figure, and selected-hint pages.

Automated checks verified 689 unique explicit source labels, preservation of
all prior labels and per-chapter exercise counts, 1,335 resolved internal
PDF links, and 304 valid bookmarks. All 68 exercise–hint pairs have working
links in both directions, including 35 newly selected appendix hints.
There are no unresolved printed references. Chapters 11–13 are unchanged
from the authoritative pre-revision working-tree snapshot. `git diff --check`
passes. No Git tag or release was created.

## Version 3.28.0 — September 18, 2026

This substantive revision starts from the current authoritative Version
3.27.1 working tree, including all uncommitted sources, figures, appendices,
and revision history. It strengthens the construction-first narrative for the
elementary functions and expands the two foundational appendices without
undertaking the deferred broad Part II pedagogical revision.

- Chapter 3 repairs the endpoint case in rational density when the least
  natural number selected by well-ordering is \(1\).
- Chapter 4 constructs
  \(e=\lim_{n\to\infty}(1+1/n)^n\) from a strictly increasing, uniformly
  bounded sequence, as an immediate application of monotone convergence.
- Chapter 5 develops general real roots, root laws, well-defined positive
  rational powers, the standard rational-exponent laws, monotonicity, and the
  qualification for negative bases. Its terminology now names Lipschitz
  continuity as the property and records the implication hierarchy.
- Chapter 7 no longer interrupts the series tests to construct rational
  powers; it recalls the Chapter 5 theory and proceeds directly to root tests
  and rational \(p\)-series.
- Chapter 8 now places power-series differentiation and Taylor machinery
  before the elementary-function construction. Familiar exponential and
  unit-circle properties motivate the series, after which the chapter proves
  the derivative and addition laws, identifies \(\exp(1)=e\), defines \(e^x\),
  constructs logarithms and real powers, and proves compatibility with the
  Chapter 5 rational powers.
- The trigonometric development distinguishes motivation from construction,
  proves the zero sets and special-angle table, defines tangent on its actual
  domain, distinguishes domains, codomains, and ranges, and develops principal
  inverse branches, composition identities, special values, and derivatives
  before returning to curves and polar coordinates.
- Chapter 9 adds worked inverse-trigonometric antiderivatives, including the
  scaled arcsine and arctangent forms with their domain restrictions.
- Appendix A now types recursion explicitly, derives induction on
  \(\mathbb N_0\), constructs addition as a binary operation, proves its basic
  laws, distinguishes maximal from greatest elements, and proves the cycle
  AC \(\Rightarrow\) Well-Ordering \(\Rightarrow\) Zorn
  \(\Rightarrow\) AC using localized transfinite recursion and Hartogs's
  lemma. The vector-space basis theorem is consequently an application of a
  proved equivalent principle.
- Appendix B is expanded at a first-reader pace while retaining narrow scope:
  categories, the divisibility/poset examples, isomorphisms, covariant and
  contravariant functors, opposite categories only after arrow reversal,
  commutative diagrams, natural transformations, differential-form pullback,
  the exterior derivative, and the de Rham forward pointer.
- A second manuscript-wide typography and dependency pass preserves compact
  prose while preferring stacked fractions and aligned displays where they
  materially improve readability. Cross-references now follow the Chapter
  4--5--7--8--9 construction order. Part II's architecture and advanced
  content remain intact.

### Validation

Two consecutive final pdfLaTeX passes produce a **498-page** PDF and a clean
log: no LaTeX/package warnings, unresolved references or citations, duplicate
labels, or overfull/underfull boxes. Extracted text contains no printed `??`.
All **1,245 internal links** resolve to document pages, and all **295
bookmarks** resolve. Visual review covers all **38 targeted pages** across the
Chapter 4--9 dependency sequence, every substantially revised Appendix A--B
page, the cover, and representative typography pages in Chapters 1, 10, 12,
and 13; corrected running heads were rendered and rechecked separately. The
prior Version 3.27.1 record is preserved below. No commit, tag, release, push,
or remote publication was made.

## Version 3.27.1 — September 18, 2026

This focused finishing revision starts from the current authoritative 3.27.0
source and README, including their uncommitted material. It is a
styling/definition/dependency patch, not a broader Part II pedagogical revision.

- A manuscript-wide mathematical-presentation pass prefers stacked fractions
  in displays, retains compact slash notation where it reads better in prose,
  selectively extracts dense inline mathematics, and uses aligned displays for
  related multistep calculations. Representative repairs span Chapters 4–9
  and other touched material without mechanically converting every expression.
- Appendix A is simplified using Kenneth A. Ross's *Elementary Analysis: The
  Theory of Calculus* selectively as a pedagogical benchmark, while retaining
  the manuscript's notation, organization, and independently checked claims.
  It fixes the conventions
  `N = {1,2,...}` and `N_0 = N union {0}`, presents Peano axioms rather than
  Peano structures, and writes the successor as `n+1` without a separate map.
- Addition is the first recursion example, making explicit that successor
  notation precedes binary addition and illustrating “recursion defines;
  induction proves.” Ordinary induction now has a practical workflow and
  distinct sum, inequality, and addition examples.
- Shifted, strong, and two-step induction are stated. Strong induction is
  proved equivalent to ordinary induction through a strengthened proposition;
  prime-factorization existence is its main worked example. A recurrence-based
  exercise gives a natural use of two-step induction.
- Binomial coefficients use the zero-outside-range convention. Pascal's
  identity precedes an induction proof of the binomial theorem. Natural-number
  well-ordering then closes the arithmetic discussion before a sharper
  transition from finite recursion to the Axiom of Choice.
- Chapter 3 formally defines an Archimedean field, proves the equivalence of
  the large-scale and reciprocal-smallness forms, recasts the completeness
  theorem as “every complete ordered field is Archimedean,” and synchronizes
  the constructed real field. Chapter 4 now uses the defined, nonredundant
  term “Archimedean field.”
- Chapter 10 defines an open cover through an index set `I` and a finite
  subcover through a finite subset `J` of `I`, retaining the empty-space and
  empty-index-set convention.
- Chapters 10–13 receive no Part-I-style scaffolding, new application sets,
  Taylor or mean-value workflows, asymptotic-notation expansion, or general
  restructuring in this patch.

### Validation

The final pdfLaTeX build produces **490 pages**. Consecutive passes have
identical auxiliary, contents, and bookmark-file hashes, and the final log has
no LaTeX/package warnings, unresolved references or citations, duplicate
labels, or overfull/underfull boxes. Extracted PDF text contains no printed
`??`. All **1,227 internal links** resolve, including both directions of all
**33 exercise-hint pairs**; the PDF has **295 bookmarks**, including the nine
correctly titled appendix bookmarks. Visual review covers every revised
Appendix A page, the Chapter 3–4 Archimedean sequence, Chapter 10 compactness,
the affected contents page, and representative fraction/display changes.
Release evidence is kept under `tmp/revision3271/`; the revision record remains
in this README.

## Version 3.27.0 — September 18, 2026

This substantive Part I elementary-analysis pedagogical revision starts from
the current 3.26.0 manuscript and README, including their uncommitted material.
No historical checkout or exported PDF was substituted for that baseline.

- Chapters 4–5 distinguish backward proof discovery from forward verification,
  teach error budgets, and name the thresholds in foundational limit proofs.
  Sequence algebra, denominator control, order, squeeze, completeness,
  Bolzano–Weierstrass, and limsup/liminf receive explicit estimates.
- Ordinary limits include integer powers, geometric sequences, rationalization,
  and polynomial quotients. Chapter 4 treats formal expressions evaluated at
  natural inputs `k`; Chapter 5 treats genuine rational-function limits,
  including infinity, denominator control, and parity at negative infinity.
- Continuity and uniform-continuity workflows include direct delta choices,
  piecewise/removable behavior, sequence-pair failures, root continuity,
  Lipschitz sensitivity, and IVT existence applications.
- Chapter 6 teaches pointwise case analysis, input-independent error estimates,
  sup norms, moving witnesses, and the role of bounded and unbounded domains.
  Bernstein approximation and equicontinuity theory remain intact.
- Chapter 7 strengthens test selection, comparison, ratio/root/alternating
  examples, growth/root limits, and power-series radius plus endpoint analysis.
  Its explicitly informal p-series/Integral-Test calculus preview recalls
  truncation and improper evaluation; the independent rational-p condensation
  proof remains. Chapter 9 explicitly closes the preview with the formal
  Integral Test and analytic rederivation for real p.
- Chapter 8 adds direct difference quotients, ordinary derivative calculations,
  familiar elementary-function limits after their construction, rate/sensitivity
  examples, and optimization with a justified domain and global extremum.
- Chapter 9 adds Darboux-gap practice, integrability decisions, FTC evaluations,
  oriented bounds, splitting and symmetry, substitution, and improper-integral
  workflows. Existing integration-by-parts examples and the deeper FTC,
  Dirichlet/Thomae, Lebesgue-criterion, and Riemann-theory developments remain.
- Selected ordinary applications explicitly translate assumptions into a
  sequence, function, derivative, or integral and interpret the conclusion.
  Exercises include verbal descriptions where students must formulate the model.
- Expanded exercise sets preserve all previous theoretical exercises. New
  optional Appendix I gives selected hints, with a superscript asterisk linking
  from each hinted exercise and a labeled return link. The front matter explains
  that the asterisk means “hint available,” not difficulty, and that scaffolding
  intentionally decreases after Part I.
- Dependency repairs distinguish Chapter 3 square roots from Chapter 5 general
  roots and Chapter 7 rational powers. Chapter 3 cites the integer-part lemma;
  Appendix A states finite choice precisely; Appendix B identifies both
  contravariant functors in the exterior-derivative natural transformation.
- Chapters 10–13, all figure sources, and Appendices C–H remain unchanged from
  the saved current baseline. All existing theoretical content and the
  analysis-to-Stokes route are preserved.

### Validation

The final pdfLaTeX build produces **491 pages**. Consecutive passes have
identical auxiliary, TOC, and bookmark-file hashes. The final log contains
no LaTeX/package warnings, unresolved references or citations, duplicate
labels, or overfull/underfull boxes; extracted PDF text contains no `??`.
All **1,220 internal links** and **295 bookmarks** have valid destinations.
The nine appendix bookmarks use the established “Appendix X: Title” format.

There are **40 new exercises** across Chapters 4–9, in addition to every
existing exercise. All **33 starred exercises** have exactly one matching
hint entry. Source counter order agrees with each printed exercise number;
the actual PDF annotations provide a forward link on the exercise page
and a return link on its hint page. The Chapter 8 Taylor hint is attached
to the Taylor exercise, including the chapter's earlier in-text exercise
in its numbering. Hints are more frequent in Chapters 2–5 and selective
in Chapters 6–9; Part II is unchanged.

The dependency and proof audit checks the Chapter 3 square-root construction,
Chapter 5 general roots, Chapter 7 rational powers, and Chapter 8 real powers.
The premature rational-power notation in Chapters 5–6 is replaced with root
notation. The oscillating differentiability example is retained after the
trigonometric construction, where its bound is proved. New dominant-power
examples distinguish polynomial degrees from sequence inputs, control
denominators, and treat signed infinite limits separately. The Chapter 7
calculus preview is explicitly informal and not used in its condensation
proof; Chapter 9 explicitly closes the promise. Application assumptions,
units, finite versus infinite totals, and error interpretations were reviewed.

Visual review covered **127 rendered pages**, including all of Chapters 4–9,
front matter, early starred-exercise pages, the complete new Appendix I,
and the local Chapter 3 and Appendix A/B repairs. Final layout checks include
the corrected Chapter 8 hint placement and keeping appendix chapter headings
with their first hint. All pre-existing source labels and exercise bodies
are preserved (apart from the requested root-notation correction).
Chapters 10–13 and Appendices C–H compare byte-for-byte with the saved current
3.26.0 source baseline; no figure sources were edited. Local build, link,
numbering, and rendering evidence is retained under `tmp/revision327/`.
Release history and validation remain in this README; no separate revision
or audit document was added.

## Version 3.26.0 — September 18, 2026

This minor version preserves the authoritative 3.25.0 manuscript and its
developed appendices. No Git reset or earlier exported baseline was used.
The main Chapters 1–13 analysis-to-Stokes route remains unchanged in scope.

- Adds a compact Notation and Conventions page before Chapter 1, preserving
  the natural-number convention and the Euclidean/intrinsic D/d distinction.
- Chapter 3 explains decimals through finite truncations and nested intervals,
  endpoint ambiguity, and the motivation for the Cauchy construction.
  Chapter 4 explicitly revisits this material through sequence convergence;
  Chapter 2's forward pointer reflects the revised progression.
- Chapter 10 introduces neighborhood limits, sequential continuity and
  closedness, first-countability tests, and a concrete counterexample to
  unrestricted sequential tests. It retains the I-adic and Zariski examples
  and makes Hausdorff uniqueness explicit.
- Preserves Chapter 13's figures, degree ladder, worked 1-forms, graded signs,
  and local-to-global architecture; appendix pointers now use labels.
- Adds Appendix A: Foundations: Natural Numbers, Induction, and Choice,
  and Appendix B: Categories and Functors.
- Reletters the existing appendices as Appendix C: Permutations and
  Determinants over a Field; Appendix D: Tensor Products and Exterior Powers;
  Appendix E: Quotient Spaces, Gluing, and Classical Manifolds;
  Appendix F: Submanifolds; Appendix G: Lie Groups and Lie Algebras;
  Appendix H: de Rham Cohomology. TOC and PDF outline entries use
  “Appendix X: Title”.
- Expands Appendix H in place with chain/cochain complexes, induced maps,
  exactness, Snake and Five Lemmas, connecting maps, long exact sequences,
  Mayer–Vietoris, and the smooth/continuous singular comparison. Existing
  Poincaré, circle, torus, and period arguments remain intact. External
  structural theorems are explicitly marked as unproved.
- Appendix G gains a worked nonzero bracket and an explicit link between
  the SO(2) generator, circle tangent, and exponential.

### Validation and dependency audit

The final pdfLaTeX build stabilizes the auxiliary, TOC, and bookmark files
and produces a 477-page PDF. The log contains no LaTeX/package
warnings or overfull/underfull boxes. Checks find no duplicate labels,
unresolved references or citations, printed `??`, missing baseline labels,
or broken internal destinations. All 1125 internal links and
286 bookmarks have valid destinations. The eight appendix
bookmarks use “Appendix X: Title” and match the A–H chapter labels and pages.

Visual inspection covers 106 selected pages continuously through the
revised Chapter 3 and Chapter 4 decimal passages, the Chapter 10 topology
sequence, affected Chapter 13 portions and outlook, all of new Appendices A
and B, and the complete F/G/H appendices. Front matter, TOC, representative
C/D/E openings, diagrams, long exact sequences, and bibliography were also
reviewed. Final layout repairs keep the notation reference on one page,
correct front-matter running headers, and prevent orphaned Appendix A headings.
All existing figure source files and every existing appendix exercise are
preserved. Chapter 13 still has 17 numbered sections, and its general Stokes
statement and proof are unchanged from the saved 3.25.0 baseline.

The dependency audit confirms:

- Chapter 3 uses finite decimal truncations and nested intervals, without
  importing series or completion theory. Chapter 4 revisits those results
  using sequence convergence; its tail estimate uses only finite sums.
- Chapter 10 defines neighborhood limits and first countability before their
  tests, retains the infinite-field hypothesis in the Zariski example, and
  confines the compactness/sequential-compactness equivalence to metric spaces.
  Hausdorff uniqueness is stated only in the valid direction.
- Chapter 13 retains tangent spaces before intrinsic differentials and
  pullbacks, forms before integration, orientation and partitions of unity
  before global integration, and global integration before Stokes. Its
  less-familiar definitions and optional-appendix pointers are cross-referenced.
- Appendix A separates Peano induction from recursion and distinguishes
  natural-number well-ordering from the general Well-Ordering Theorem;
  the unproved choice equivalences do not conceal an ordinal construction.
- Appendix B orders categories, functors, contravariance, and natural
  transformations before its forward pointer to cohomology.
- Appendix H places complexes and cochain maps before quotient/induced maps,
  exactness before the Snake/Five statements, and long exact sequences before
  Mayer–Vietoris. Singular terminology precedes the de Rham theorem, and
  integration is restricted to smooth chains in the comparison discussion.
  Unproved structural results are identified locally; the appendices do not
  become prerequisites for Chapters 1–13.

The historical Version 3.25.0 record below is preserved verbatim.


## Version 3.25.0 — September 17, 2026

This revision works from the authoritative 3.24.0 working source and PDF,
including existing uncommitted material. No historical Git reset was used.

- Appendix A shortens field-structure digressions and the second Laplace
  bookkeeping proof while retaining cycles, Vandermonde parity, inversions,
  and the characteristic-two distinction between alternation and symmetry.
- Appendix B uses universal properties for associativity, finite products,
  induced maps, and structural identities; distributivity is proved once
  and reused. The binary construction and detector basis proof remain
  detailed. Exterior wedge arithmetic and determinant detectors are explicit,
  the nontrivial multiplication and duality constructions remain, and the
  exercise collection contains twelve distinct tasks.
- Appendix C uses one separated-isometry metric proposition for strip,
  Klein-bottle, and antipodal quotients, preserving the seam/corner charts
  and the complete classical manifold gallery.
- New **Appendix D — Submanifolds** develops local straightening, graphs,
  embeddings versus immersions, manifold rank and regular-level theorems,
  tangent kernels, matrix constraints, and intrinsic multipliers.
- New **Appendix E — Lie Groups and Lie Algebras** develops matrix groups,
  left-invariant fields, the bracket, tangent Lie algebras, and matrix
  exponentials with the explicit SO(2) calculation.
- New **Appendix F — de Rham Cohomology** develops the quotient and induced
  pullbacks, degree zero, the star-shaped Poincaré lemma, angular obstruction,
  circle and degree-one torus calculations, and integration on cycles.
- Section 13.17 now navigates from topology through smooth geometry to
  analysis, with concise, connected directions for **differential topology,
  geometric topology, and geometric analysis**, plus separate Lie theory
  and a shortened de Rham preview pointing to the developed appendices.
- Chapter 11 points to D for manifold rank notions. The visual §13.5 tour
  gains a small pullback preview. Euclidean derivatives use `Df(p)` and
  exact-form values use `(df)_p`; intrinsic differentials retain `df_p`.
  All appendices now start with an unnumbered **Introduction**.

### Reference comparison and mathematical scope

Tu, *An Introduction to Manifolds*, second edition (2011), and Lee,
*Introduction to Smooth Manifolds*, second edition (2013), are the primary
comparisons. Their actual texts were consulted, rather than relying on
secondary summaries. Source texts and baseline snapshots are retained under
`tmp/refinement-3.25/`; no additional maintained audit document was created.

| Material | Comparison and chosen mechanism |
|---|---|
| D: slices, graphs, embedded images, smooth maps into subsets | Tu §§9, 11.3–11.4; Lee Chapter 5. The induced slice atlas and subspace topology are checked directly. |
| D: constant rank, regular values, tangent kernels, extrema | Tu §§9–11, including Theorems 9.9 and 11.1; Lee Theorem 4.12 and Corollary 5.14. Chart reduction reuses Chapter 11; the kernel and multiplier conclusions use rank–nullity and linear factorization. |
| D: Whitney perspective | Lee Theorem 6.19 is stated without proof for positive-dimensional manifolds without boundary. Tu §11.3 supplies the contrasting local image/embedding discussion, not a claimed proof of Whitney. |
| E: group examples and tangent matrices | Tu §§15–16; Lee Chapters 7–8. The symmetric target for `AᵀA` removes redundant constraints; determinant differentiation gives the special-linear kernel. |
| E: invariant fields and brackets | Tu Propositions 16.8–16.11; Lee Propositions 8.33 and Theorem 8.37. Smoothness uses translated coordinate curves; cancellation of second derivatives gives the bracket before transport to the identity. |
| E: matrix exponentials | Tu §15; Lee Chapter 20. Compact-uniform power-series estimates and the Cauchy product prove the matrix results without assuming general flow existence. |
| F: quotient, degree zero, pullback | Tu §24; Lee Chapter 17. The representative check is explicit; infinitely many components give a product of copies of R. |
| F: local exactness | Tu §29's coefficient integration and Lee Lemma 17.9/Theorem 17.14. The proof specializes to straight segments and derives the sign identity directly, avoiding Lie derivatives and general homotopy machinery. |
| F: periods and examples | Tu §§24, 26.2, 28.1; Lee Chapters 17–18. Periodic primitives replace Mayer–Vietoris for the circle and degree-one torus calculation; Stokes gives the cycle obstruction. |
| F: de Rham comparison | Lee Theorem 18.14, with Tu's §§24–29 as the introductory cohomological route. The comparison theorem is explicitly unproved. |

The new arguments are reconstructed in the manuscript's notation and checked
independently. D assumes manifolds without boundary; E assumes D; F starts
from Chapter 13 and may use C's examples. The main torus is still `S¹ × S¹`,
Chapter 13 still constructs forms directly from alternating covectors, and
General Stokes acquires no appendix prerequisite. Whitney and de Rham are
the only major unproved perspective theorems in D–F; the general Lie-group
exponential is described only as a later construction.

### Validation

The final PDF has **463 pages**. The last two pdfLaTeX passes stabilized
the auxiliary, TOC, and bookmark files. The final log has no LaTeX/package
warnings or overfull/underfull boxes. All 617 labels are unique; all original
labels survive; citations and references resolve, and the extracted PDF
contains no printed `??`. All 1,020 internal link destinations and 267
bookmark destinations resolve. No appendix title retains the old optional prefix.

Visual review covered 116 distinct PDF pages: the title/contents/reading
guide, Chapter 11 notation and forward references, Chapter 13's preview,
Euclidean and intrinsic differential passages, all of §13.17, every page of
Appendices A–F, and the bibliography. Orphan headings in A, B, and F were
corrected and the affected pages re-rendered and reinspected.

Against the saved authoritative working baseline, Chapters 1–10 and 12
are byte-for-byte unchanged. Chapter 13 retains all seventeen numbered
sections, its early sequence, and the unchanged General Stokes statement
and proof. Appendix B has twelve exercises; D, E, and F have seven each.
The reference-comparison table above records the actual Tu/Lee checks and
the scope of the independently reconstructed arguments.

## Version 3.24.0 — September 17, 2026

This release expands proof detail while preserving the manuscript's overall
architecture, original labels, examples, and exercises. It starts from the
existing 3.23.0 working source, not a reset to an earlier repository commit.

- Chapter 10 adds total boundedness and proves compactness ⇔ sequential
  compactness ⇔ completeness plus total boundedness. The finite-subcover
  separation margin is now available for later compact-support arguments.
  Heine–Borel retains and expands its coordinate/subsequence proof, followed
  by the completeness/total-boundedness viewpoint and comparison examples.
- Connectedness now includes clopen sets, locally constant functions,
  intermediate values, the fully proved topologist's sine curve, connected
  components, total disconnectedness versus discreteness, and polygonal
  paths in open connected Euclidean sets. The I-adic example begins with
  integer congruence neighborhoods before the optional algebraic generalization.
- Section 13.5 is a visual manifold vocabulary tour; §13.6 develops algebra
  at one vector space; §13.7 starts with “Why differential forms?” and the
  retained exact/general 1-form and curve-pullback material before flux
  2-forms and general forms. All 17 numbered Chapter 13 sections remain.
- Determinant proofs display the surviving permutation, cancellation pairs,
  product columns, triangular stages, transpose reindexing, and the form
  underlying the Laplace minor. Appendix A retains its Vandermonde-first
  parity argument and expands its separate combinatorial Laplace proof.
- Appendix B constructs exterior maps directly by the exterior universal
  property, then verifies tensor-quotient compatibility. Exterior bases,
  minors, composition, the top-degree determinant action, and duality show
  their intermediate calculations. The existing tensor and exterior-product
  architecture is preserved. Dummit–Foote is used selectively as a comparison.
- Appendix C receives a localized audit of fibers, descent, metrics, and
  small quotient neighborhoods; its existing gluing gallery is retained.
- Ten new TikZ figures explain compactness, connectedness, charts, tangent
  directions, and smooth weights. The intrinsic-boundary figure moves into
  the preview. Existing diagrams now distinguish a scalar component from
  its projected vector and coordinate transitions from their derivatives.
- Later uses of finite ball covers, connected components, locally constant
  signs, and compact-support separation have explicit references. The main
  torus remains `T² = S¹ × S¹`, and the cusp distinction is preserved.

The separate Algebra manuscript was not modified. Deferred suggestions,
scope details, and the dependency review are recorded in
[REVISION-3.24.0.md](REVISION-3.24.0.md).

### Validation

The 444-page PDF compiles with pdfLaTeX and stable auxiliary, contents, and
bookmark files, with no LaTeX warnings or unresolved references/citations.
Checks cover 581 labels, 955 internal links, and 249 bookmarks; all original
labels survive. Visual review covers 99 rendered pages, including the revised
topology, early Chapter 13, and all Appendix A/B/C pages. Verification records
are in `tmp/refinement-3.24/`; the release report describes their scope.

## Version 3.23.0 — September 17, 2026

This controlled revision preserves the existing chapter/section architecture,
Riemann/Jordan foundation, direct alternating-covector construction, and proof
strategies. The formal torus remains `T^2 = S^1 × S^1`; §13.17 remains a preview.

- Chapter 10 adds the I-adic basis example with both basis checks, quantitative
  rational-coordinate approximation with countability references, closed
  singletons and finite sets in Hausdorff spaces, and the Zariski affine line
  over an infinite field as the substantive converse counterexample.
- The reading guide states a selective global cross-reference convention.
  Local reminders now connect countable bases, Hausdorff separation, support,
  local finiteness, precompactness, dual bases, and form operations to their
  definitions. Appendix C receives corresponding topology reminders.
- Generic manifold maps use `f,g`, their intrinsic differentials use `df,dg`,
  Euclidean representatives use a separately named `h`, and surface
  parametrizations use lowercase symbols. Statements, proofs, exercises, and
  diagrams are synchronized; conventional vector-field `F` remains distinct.
- “Why differential forms?” now opens the forms sequence. Numerical covector
  evaluations, type distinctions, degree-one curve pullback derivation, exact
  versus general forms, and the circulation obstruction precede general forms.
  Flux motivates two inputs before the abstract exterior-power construction.
- Exterior algebra gains a geometric degree ladder, explicit basis-proof
  questions, a separate equivalent full-permutation remark, a six-swap block
  example, the parity table and odd-degree square consequence, and a complete
  three-dimensional degree table before the graded direct sum. Appendix B is
  explicitly recommended as a structural alternative with precise
  references to its constructions and canonical-agreement proposition.
- The manifold route has a compact local-to-global roadmap and first-reading
  guidance; second countability is recalled at the definition. Manifold
  1-forms and a worked coordinate-change evaluation precede general forms.
  Pullback starts with one direction; manifold exterior differentiation states
  its Euclidean/overlap strategy before the formal construction.
- Integration is introduced through one-chart integration, coordinate
  invariance, then smooth localization. A two-chart circle preview and a
  common-refinement roadmap prepare the retained rigorous infrastructure.
  General Stokes closes the story through localization, local Euclidean
  Stokes, cancellation of weight derivatives, and reassembly.
- Eleven original TikZ figures explain work projection, reversal, surface
  area, flux, patch Stokes, alternating measurements, tangent representatives,
  the differential, intrinsic boundary, chartwise integration, and global
  Stokes. The surface-reparametrization hypothesis now names the ambient
  diffeomorphism and its restriction explicitly.

### Validation and dependency review

The complete 430-page manuscript compiles with pdfLaTeX; repeated passes
stabilize the auxiliary, contents, and outline files. The final checks find
556 unique source labels, no unresolved references or citations, no extracted
`??` placeholders, and no LaTeX/package or overfull/underfull-box warnings.
All 914 internal links and 246 bookmarks resolve to valid destinations.
All original labels and all 17 numbered Chapter 13 sections are retained,
including its 42 proofs and 32 exercises.

Visual review covers all 87 Chapter 13 pages (printed pages 281–367), the
affected Chapter 10 and related pages, and enlarged views of all eleven new
figures. Corrections include separating diagram labels, removing redundant
sketches, placing tangent representatives after their construction, and
keeping first-reading and exercise headings with their following text.

The dependency audit checks chart independence before the tangent-space
operations, the differential before intrinsic pullback, and Euclidean
pullback compatibility before manifold exterior differentiation. Boundary
invariance precedes induced orientation; support, local finiteness, and
partitions of unity precede integration independence and global Stokes.
Early geometric examples are explicitly previews, not proof prerequisites.
Appendices B and C and the further-directions section remain outside the main dependency route.
Detailed audit evidence and baseline snapshots are in
`tmp/refinement-3.23/`, including `dependency-audit.md`, `checks.json`,
`source-audit.json`, and rendered-page review files.

## Version 3.22.0 — September 17, 2026

Targeted refinement of the authoritative 3.21.0 manuscript and README,
preserving the chapter/section architecture and section-based numbering.

- Chapter 10 formally connects open neighborhoods, topological bases, the
  basis criterion, rational Euclidean bases, product bases, and second
  countability. Subspace and finite-product inheritance are proved and cited
  in the manifold and optional quotient constructions.
- Covectors remain Definition 10.16.1. A separate dual-basis definition
  introduces the Kronecker delta, coordinate extraction, and the parallel
  vector/covector expansions. Exchange and coordinate-conversion mechanisms
  are clarified; multilinear finite-dimensionality hypotheses are explicit.
  The existing detailed determinant expansion is retained.
- Four structural Chapter 10 figures show a basic product neighborhood,
  internal direct sums (with a three-line counterexample), one vector in two
  coordinate systems, and reversal of determinant orientation.
- Section 13.5 introduces Euclidean 1-forms and curve evaluation before
  general exterior powers. Section 13.6 gives explicit object types,
  determinant-defined elementary wedges, their identities, the three-dimensional
  degree-two example, and a detector-based spanning/independence proof.
  Separate propositions prove shuffle multilinearity and alternation, then
  compatibility with elementary concatenation via Leibniz permutations before
  deriving the exterior-algebra laws.
- Section 13.7 explains pointwise wedge products and pullback smoothness,
  motivates degree-raising differentiation from Green and Stokes, and retains
  the distinction between the Hessian and exterior differentiation. First-reading
  guidance keeps Appendix B's tensor/universal-property route independent of the main route.
- Classical proofs now establish cross-product bilinearity, admissibility of
  reparametrized Jordan regions, null boundary arcs under finite subdivision,
  and the chain/product-rule steps of patch Stokes. Local finishing edits in
  §§13.14 and 13.17 clarify equal-dimensional substitution, the three-stage
  Riemann comparison, and the projective filtration, and remove drafting prose.
- Existing Munkres, Tu, Lee, and Spivak references are retained; Hubbard and
  Hubbard is added as a selective geometric companion. Tu's coordinate-form
  distinction is cross-checked against the author-supplied ICTP excerpt.
  Proofs and figures are written in the manuscript's own notation.

No additional general-topology course or tensor prerequisites are introduced.
The optional I-adic aside and lower-priority figures are omitted to keep the
pass focused. New numbered definitions/propositions shift later numbers only
within their sections; four inserted figures shift later Chapter 10 figure
numbers. Existing labels remain the reference mechanism.

### Version 3.22.0 validation

The final PDF contains 421 pages (seven more than Version 3.21.0). Compilation
stabilized with no LaTeX warnings or overfull/underfull boxes. Automated checks
verified 533 unique labels, 879 internal links, and 246 bookmarks, with no
unresolved references/citations, invalid destinations, or printed `??` markers.
Visual review covered 63 selected pages, including all four new figures and
the continuous exposition in §§13.5–13.7. A further 425 exact arithmetic checks
confirmed representative shuffle, determinant, sign, and coordinate-detector
identities as a supplement to the written proofs. Local numbering changes
were audited; the earlier README version history is preserved unchanged.

## Version 3.21.0 — September 16, 2026

Focused refinement of the current 3.20.0 manuscript, preserving the chapter
architecture, existing numbered statements, and optional quotient-topology route.

- Chapter 11 distinguishes operational calculus notation from geometric
  differentials, makes the two-variable curve chain rule explicit, and explains
  implicit differentiation as vanishing on level-curve directions.
- Chapter 13 motivates tangent lines, planes, and cotangent measurements; connects
  dual bases and `df` with curve pullbacks and regular-level-set kernels; and makes
  the Euclidean integral, line integral, signed Jacobian, and general Stokes
  connections explicit. Sections 13.12–13.14 use clearer paragraph structure,
  proof strategies, and displayed overlap, orientation, and localization formulas.
- Existing illustrations follow their constructions more closely, with local
  float barriers and one fixed torus-sequence figure. The sphere illustrations
  follow the chart and transition steps separately. Appendix C's Klein figure
  now follows its gluing definition; the two Klein figures consequently exchange
  numbers C.6/C.7, with labels and cross-references retained.
- Section C.3 is **Circles and Spheres as Quotients**. The projective line is a
  distinct unnumbered example following the antipodal construction, and the torus
  square distinguishes dashed and solid edge pairs. No new topology material or
  figures were added. The two unrecovered historical path literals remain
  explicitly unavailable; no paths were guessed.

### Version 3.21.0 validation

The full **414-page PDF** compiles with pdfLaTeX (three pages more than 3.20.0).
A repeat pass leaves `main.aux`, `main.toc`, and `main.out` unchanged; the final
log has no warnings, unresolved references/citations, or overfull/underfull boxes.
All **511 source labels** are unique, all checked source references and cited
bibliography keys resolve, extracted text contains no `??`, and all **828
internal links** have valid destinations. Existing labeled statement numbers
are unchanged; only the two relocated Klein figures exchange numbers.

Rendered review covered **72 selected pages of the final PDF**, including the affected Chapter 11
passages, classical diagrams, all Chapter 13 and Appendix C numbered figures,
the tangent/cotangent discussion, all of §§13.12–13.14, and Stokes. The gallery
was rechecked after the final page-break adjustment. Mathematical checks cover
the heuristic/pullback distinction, regular-level kernels, dual-basis notation,
orientation signs versus absolute Jacobians, and local-to-global support and
sum identities. No new prerequisite on Appendix C or algebraic topology was
introduced. The preceding version history is preserved verbatim.

## Version 3.20.0 — September 16, 2026

Focused finishing revision of the authoritative Version 3.19.0 working
manuscript. The main analysis-to-Stokes route and independence of Appendix C
and §13.17 are preserved.

- Appendix C uses triangular quotient-factorization diagrams and tilde notation
  for induced maps. Appendix B aligns quotient notation while retaining standard
  tensor and exterior-power structural names.
- The projective-space construction now starts from nonzero scaling, identifies
  the antipodal sphere model by two inverse induced maps, and proves affine-chart
  continuity, smooth transitions, Hausdorff separation, second countability, and
  compactness directly. The projection-matrix and trace detour is removed.
- Compact quotient figures explain sphere boundary collapse, torus and Möbius
  edge rules, Klein gluing, and projective antipodal pairs and disk models.
  The Chapter 13 Klein sequence explicitly moves an open tube end toward its
  partner before gluing. Existing torus/Möbius sequences and local charts remain.
- §13.17 adds the maps-to-invariants viewpoint, induced fundamental-group and
  homology maps, explicit CW characteristic maps and disjoint-union topology,
  quotient-figure connections, and the two-dimensional formula χ = V − E + F.
  Real coefficients and the unproved-preview scope are retained.
- The bibliography destination follows its heading's page break; local prose
  defects are corrected. Historical literal paths are restored by exact
  surrounding-text comparison with the intact preceding README at
  `tmp/revision-current/baseline/README.md` (formerly numbered 3.10.0, now 3.18.0).
  This restores 149 occurrences. Two path literals in the subsequently deleted
  standalone audit are explicitly marked unavailable rather than reconstructed
  from corruption suffixes; restoring them requires the intact audit source.
  Historical paths retain their original spelling even when the files are obsolete.
- The supplied topology notes are acknowledged by their verified title and
  author. The Chinese smooth-manifolds notes are acknowledged by romanized
  author/title and the specific projective-space example; no publication
  date or venue is invented. The source's swapped Hausdorff-case coordinates
  are corrected in the adapted argument.
- All release and validation records are maintained here. `ERRATA.md` is the
  single errata entry point; redundant copy files and obsolete documentation
  snapshots are removed after their records are checked for preservation.

### Version 3.20.0 validation

The complete **411-page PDF** builds with pdfLaTeX; a final repeat pass
leaves `main.aux`, `main.toc`, and `main.out` unchanged. The final log contains
no LaTeX/package warnings, overfull/underfull boxes, or unresolved references.

- All **511 source labels** are unique and **536 reference occurrences** resolve.
  Extracted PDF text contains no unresolved `??`. All **821 internal named links**
  resolve, and all **425 numbered statement/exercise destinations** contain
  the expected number on their destination page. All **31 historical README
  links** resolve to preserved anchors.
- The bibliography contents entry on physical PDF page **6** and its outline
  bookmark share the heading destination on physical PDF page **409** (printed
  page **401**), at the top of the page (PDF destination y = 720 points).
  The rendered destination page begins with “References and Further Reading”;
  the preceding exercise page is no longer the target.
- Visual inspection covers **33 pages**, including the complete revised §13.17,
  the complete Appendix C, the cover, affected Appendix B diagrams, the Klein
  sequence, and bibliography. All seven new/revised figure pages were also
  inspected at enlarged scale. Figure-label overlaps, a stranded section heading,
  and a figure interrupting the exercises were corrected before the final build.
- Comparison with the supplied 3.19.0 working baseline preserves all **39
  Chapter 13 proof bodies** verbatim, the full partitions-of-unity through Stokes
  and exercises block, all earlier chapters and Appendix A, the existing torus
  and Möbius sequences, and all three retained local quotient figures. Appendix B
  changes only canonical quotient-map and induced-map notation. Existing Appendix C
  proof bodies preceding projective space are preserved except the requested
  universal-property notation refinement.
- Mathematical checks cover exact quotient fibers versus unjustified injectivity,
  the two inverse scaling/sphere factors, open restricted quotient maps,
  representative-independent affine ratios and inverses, ordered transition
  coordinates and domains, both Hausdorff cases, countable chart bases,
  compactness, and the explicit projective-circle map. CW cells, skeleta,
  attachment domains and the torus word, real chain/cochain indices, induced
  maps, and the surface Euler specialization agree. No active source retains
  the deleted projective matrix/trace argument or depends on it in an exercise.
- Documentation cleanup removes **262 Copy-named files**, **six duplicate errata
  files**, and **37 obsolete README/OUTLINE snapshots**. The repository now has
  one README and one ERRATA file. Three additional historical errata paragraphs
  were preserved below. Older source/PDF snapshots remain as historical evidence;
  this cleanup does not delete entire snapshot directories.

The 149 recoverable historical literal paths were compared with the intact
preceding README before removing its redundant documentation snapshot. Two
path literals from the deleted standalone audit remain explicitly marked as
unavailable; they were not guessed. This is the remaining documentation limitation.
The bibliography has 23 entries, including both supplied lecture-note sources.
Current metadata agrees on **3.20.0**, **September 16, 2026**. No commit, tag,
push, publication, standalone release-note file, or standalone audit was created.


## Version 3.19.0 — September 16, 2026

This substantive revision continues the authoritative working manuscript formerly
numbered **3.10.0**, now **3.18.0** under the corrected history below. It does not
restart from Git HEAD or an earlier draft.

- Appendix C separates motivation, definitions, metric arguments, topology
  comparisons, and local-chart proofs. Canonical projections use π; general
  quotient maps use q. Coset quotients connect to Appendix B, and Z² is explicitly
  a subgroup rather than a real vector subspace. Trace and its invariance now
  precede the projective-space projection argument. Six focused exercises close
  the appendix.
- Chapter 13 distinguishes the generating identity chart, its maximal standard
  smooth atlas, and the resulting manifold. Torus gluing includes a bent cylinder
  with separate ends and consistent θ/φ directions. Möbius markers, depth cues,
  and the boundary itinerary clarify the half-twist. Five Klein-bottle stages
  distinguish its actual seam from the incidental crossing in R³. Appendix C
  adds compact seam and corner charts; the circle, cylinder, annulus, and original
  embedded-torus figures are preserved.
- §13.17 gives Algebraic Topology its own topic after General Topology: homotopy,
  based loops, fundamental groups, CW complexes, Euler characteristic, and real
  singular chains and cochains. Landmark results are explicitly unproved
  previews. De Rham Theory remains after Differential Geometry, retains the
  punctured-plane example, and refers to the new cohomology definition.
- Front matter distinguishes optional algebraic and topological quotients.
  The bibliography adds Hatcher as further reading, not an adaptation claim.
  Current and historical validation summaries live in this README; the immediately
  preceding standalone audit is consolidated below and removed without discarding
  its content. No new audit or release-note file is created.

### Version 3.19.0 validation

The complete **407-page PDF** builds with pdfLaTeX. Repeated passes produce
identical `main.aux`, `main.toc`, and `main.out` hashes. The final log has no
LaTeX/package warnings, overfull/underfull boxes, or unresolved references.

- All **504 source labels** are unique; **527 reference occurrences** resolve.
  Extracted PDF text contains no unresolved `??`. All **811 internal links**
  have destinations, and **425 labeled numbered statement/exercise destinations**
  land on pages containing their correct numbers. All 31 historical README links
  resolve to their consolidated records.
- Direct comparison with the supplied working baseline preserves all **39
  existing Chapter 13 proof bodies** verbatim. The complete source block from
  partitions of unity through manifold integration, General Stokes, classical
  recovery, and the exercises is unchanged. No earlier chapter or Appendix A/B
  is edited in this pass. The circle, cylinder, annulus, and embedded-torus
  figure sources are byte-for-byte unchanged.
- The mathematical review checks representative independence, attainment of
  quotient-distance minima, metric/quotient topology agreement, seam domains,
  all four Klein corner representatives, boundary-component counts, and countable
  bases. Projective trace, rank, normalization, chart inverses, and transition
  denominators are justified locally. Based homotopy fixes endpoints, loop
  concatenation is consistently left-to-right, sphere/projective/torus cell
  counts agree with the examples, and chain/cochain indices include degree zero.
  Real coefficients match the de Rham comparison. None of these optional
  constructions enters the Stokes prerequisite chain.
- Rendered review covers **47 selected pages**, including the cover and contents,
  affected manifold and gallery pages, the full revised Further Directions
  sequence, every Appendix C page, and the bibliography. Every changed/new figure
  is checked at reading scale and enlarged scale. The torus's initial blue-edge
  gluing keeps θ along the tube and φ around it; its ends remain visibly separate
  before closure. The Möbius trace uses increasing x on both original edges.
  The Klein representation distinguishes the actual glued seam from its crossing.
  Appendix seam and corner diagrams match the displayed coordinate maps.
- Figure-label collisions and an overfull paragraph were repaired; section openings
  stay with their constructions, and the references entry no longer occupies a
  separate contents page. All three metadata locations agree on **3.19.0** and
  **September 16, 2026**. The bibliography has 21 entries, with Hatcher explicitly
  used for further reading. Optional extra projective, lattice, and CW figures
  were omitted to keep the appendix and preview restrained.

All release notes and validation summaries remain in this README. No standalone
revision audit, Git commit, tag, push, or release was created.

### Version-numbering policy and corrected history

Use **MAJOR.MINOR.PATCH**. A substantive addition, broad pedagogical restructuring,
or major proof redevelopment increments MINOR and resets PATCH to zero. Local
corrections, notation repairs, finishing edits, and maintenance increment PATCH.
A wholesale architectural break may increment MAJOR. Lack of new theorem scope
alone does not make a broad revision a maintenance patch.

The review covers all documented releases. Versions through 3.4.1 already fit
this rule and retain their numbers, including the local 3.1.1 and 3.4.1 patches.
The substantive revisions formerly called 3.4.2–3.4.8 and 3.5.1 require minor
increments. Their successors are renumbered to preserve chronological order;
local finishing/dependency repairs remain patches. Here is the complete mapping
of changed historical identifiers (left column intentionally preserves old names):

| Original identifier | Corrected identifier | Classification |
|---|---|---|
| 3.4.2 | 3.5.0 | Substantive revision |
| 3.4.3 | 3.6.0 | Substantive revision |
| 3.4.4 | 3.7.0 | Substantive revision |
| 3.4.5 | 3.8.0 | Substantive revision |
| 3.4.6 | 3.9.0 | Substantive revision |
| 3.4.7 | 3.10.0 | Substantive revision |
| 3.4.8 | 3.11.0 | Substantive revision |
| 3.5.0 | 3.12.0 | Substantive revision |
| 3.5.1 | 3.13.0 | Substantive revision |
| 3.5.2 | 3.13.1 | Maintenance / local repair |
| 3.6.0 | 3.14.0 | Substantive revision |
| 3.6.1 | 3.14.1 | Maintenance / local repair |
| 3.7.0 | 3.15.0 | Substantive revision |
| 3.8.0 | 3.16.0 | Substantive revision |
| 3.9.0 | 3.17.0 | Substantive revision |
| 3.10.0 | 3.18.0 | Substantive revision |

At that release, **3.19.0** followed corrected **3.18.0**; the current
revision is **3.20.0**. Its projective-space redevelopment and new quotient
figures warrant a MINOR increment under the same policy. Release headings,
historical prose references, and their internal README anchors use the corrected
numbers. Literal paths to existing historical scratch artifacts retain their
original filenames; the mapping resolves those names. Historical artifact paths retain the filenames used when produced; redundant
working snapshots are removed under the single-record policy. No Git history, commit,
tag, or published release is rewritten or created.

## Version 3.18.0 — September 16, 2026

This focused revision starts from the authoritative Version 3.17.0 working
manuscript. Chapter 10 motivates Hausdorffness and proves the closed-diagonal
criterion before the compact-subset theorem; it does not develop quotient topology.
New Darboux and subspace figures explain oscillation and relative openness.

Chapter 13 preserves the formal product torus and the original embedded-torus
figure. The parameter square now develops through a cylinder into the torus.
Staged cylinder, Möbius-strip, and Klein-bottle diagrams explain matching arrows,
a half-twist, boundary components, and the representational self-intersection
of the Klein-bottle drawing. The gallery previews orientability, then §13.13
returns to determinant signs and the global sign reversal around closed loops.
A standard annulus illustrates outward-first boundary orientation. The torus
also receives an explicit nowhere-vanishing form from its product-circle model.

Appendix C develops the quotient topology and universal property,
compact-to-Hausdorff arguments, circle and torus quotient models, explicit
cylinder/Möbius seam and boundary charts, Klein-bottle edge and corner charts,
and projective spaces via projection matrices and affine charts. Separation
and second countability are checked, rather than inferred from local pictures.
Its seven sections remain outside the main prerequisite chain. An endpoint-gluing
figure complements the circle construction. No general quotient-manifold,
covering-space, or group-action theory is introduced.

All prior proof bodies in Chapters 9, 10, and 13 are retained verbatim; the
other existing chapters and both earlier appendices are untouched. All earlier
standalone figures are unchanged except the requested parameter-square upgrade.
The General Topology perspective now points to Appendix C instead of duplicating
its quotient definition and circle proof. Version metadata, contents, numbering,
and cross-references are regenerated. No Git commit, tag, or release is created.

Validation details are preserved in the [consolidated validation record](#historical-revision-3.18.0-audit) below.

## Version 3.17.0 — September 16, 2026

Version 3.17.0 replaces several elaborate proofs with more transparent
constructions while preserving the established dependency structure. Part I
now uses peak indices for monotone subsequences and Bolzano–Weierstrass,
a single completeness-equivalence cycle, reciprocal inverse difference
quotients, nested open sets for Dini, and local Darboux derivative bounds
for countable-exception Newton–Leibniz. Integral linearity, rearrangements,
alternating remainders, and Thomae's function receive shorter arguments.

Part II uses a finite-cover compactness argument, a telescoping finite
partition of unity, common Darboux bounds for continuous Fubini, and
translated fibers for shear volume after proving Jordan measurability.
The manifold partition of unity retains positive-sum normalization.
The existing quantitative inversion remainder, sequential uniform-continuity
arguments, and source-side change-of-variables localization are retained.

Ten original TikZ figures in `figures/` support affine hyperplanes, conics,
implicit surfaces, local Jacobian distortion, spherical coordinates, sphere
charts and overlaps, and the torus. Existing graph/tangent, gradient, and
oblique-coordinate figures remain. Spherical coordinates include the Jacobian,
ball volume, and explicit control of axis, origin, and seam exceptions.

Chapter 10 is titled **Topology and Linear Algebra** and explicitly defines
an open neighborhood. Chapter 13's locally Euclidean condition uses an open
neighborhood of each point and a homeomorphism onto an open Euclidean subset.
Definitions prefer “if”; characterization theorems retain equivalences.
Generic open sets prioritize U, V, W, with distinct ambient extension domains
and other meaningful local notation retained.

The scope of §13.17 is preserved. No Git tag or GitHub release is created.

Validation: the final PDF has **386 pages**. Repeated pdfLaTeX passes stabilized
`main.aux`, `main.toc`, and `main.out`. Checks found no duplicate labels,
unresolved references, extracted-text `??`, LaTeX warnings, or overfull/underfull
boxes. All **753 internal links** and **421 numbered destinations** passed.
The Chapter 10 bookmark and contents title were verified. All ten new figures
were inspected at page scale and enlarged scale; revised theorem pages and
preview citations were also reviewed. All 39 existing Chapter 13 proof bodies
remain unchanged from the Version 3.16.0 working baseline.

## Version 3.16.0 — September 16, 2026

Version 3.16.0 substantially refines Chapter 13's manifold exposition without
enlarging the developed differential-geometric scope. Core manifold definitions
are recast around formal symbolic statements followed by shorter explanations,
standard and inherited smooth structures are made explicit, transition maps
handle empty overlaps transparently, and a sphere atlas plus original diagrams
strengthen the first examples. The Further Directions section is expanded into
concise mathematical previews of measure theory, topology, functional and complex
analysis, differential geometry, de Rham theory, PDE, and probability. The
established partition-of-unity, manifold-integration, and Stokes proofs remain intact.

- Definitions display their maps, domains, quantifiers, and equivalence relations.
  Identity charts generate maximal standard atlases; restricted charts define
  inherited structures; a proposition proves each chart is a diffeomorphism.
- The examples progress from Euclidean spaces and open subsets through graphs,
  the circle, a six-chart sphere atlas with a worked transition, and products.
  Original diagrams show coordinate changes, smooth maps, the half-space model,
  and localization; two compact diagrams summarize the definition dependencies.
- The seven-page further-directions section introduces actual mathematical objects
  and explicitly marks unproved theorems as previews. None becomes a prerequisite
  for the developed manifold, integration, or Stokes theory.
- Chapter 12's closing Fubini wording now attributes the general theorem's bounds
  to product Riemann integrability. The partition theorem statement and the
  computational-practice heading are kept with their associated content.

### Version 3.16.0 validation

- The final PDF has **381 pages**. Repeated pdfLaTeX passes completed with
  identical final `main.aux`, `main.toc`, and `main.out` hashes. There are no
  LaTeX/package warnings, overfull/underfull boxes, undefined references,
  duplicate labels, broken internal links, or extracted-text `??`.
- Checked **465 labels**, **488 reference uses**, **416 labeled statement
  destinations**, and **750 internal links**. Every audited numeric statement
  destination lands on a page containing its correct result number.
- Direct source comparisons preserve Chapter 13's opening through local Stokes,
  the tangent vector-space and intrinsic differential proofs, the external
  refinement theorem, the partition theorem statement and proof, the top-form
  converse, compact boundary extension, manifold integration and its
  common-refinement proof, and the entire general Stokes section. Classical
  recovery and exercises differ only by the computational-heading page guard.
  Chapters 1–11, both appendices, and the bibliography were not edited in this pass.
- The mathematical review checked the sphere chart domains, inverse maps, and
  overlap formula; vacuous smoothness of empty transitions; maximal extension
  and inherited structures; the signed-boundary-chart convention; and the
  partition-dependent direction of the orientation/top-form theorem. Tangents
  remain chart-vector equivalence classes and exterior algebra remains based
  on alternating covectors in the main text.
- Further-direction statements have their required hypotheses: measurable
  dominated convergence, continuous Hilbert-space duals, the disk form of
  Cauchy's integral formula, and the integrable i.i.d. strong law. The de Rham
  isomorphism is explicitly with real singular cohomology. The PDE weak-form
  discussion is motivational. None of these previews is used by the developed
  theory. The Chapter 12 cleanup adds no measure-theoretic prerequisite.
- Visually reviewed the cover and contents, physical pages **304–341** covering
  the full revised §§13.9–13.17 sequence, the Chapter 12 cleanup, and the three
  bibliography pages. The six new diagrams were also inspected at enlarged
  scale. The partition statement remains on one page, and computational practice
  stays with its first exercise. Version and date agree between cover and README.
- The bibliography retains its existing 20 entries and attribution architecture.
  No Git tag or GitHub release was created.


## Version 3.15.0 — September 16, 2026

Version 3.15.0 strengthens Chapter 12's classical Riemann–Fubini theory through
lower and upper section integrals and exceptional-section examples, while
substantially expanding Chapter 13's manifold foundations into a gentler
sequence of charts, atlases, boundary models, tangent and cotangent spaces,
differentials, forms, and orientation. The existing partition-of-unity,
manifold-integration, and Stokes proofs are preserved. Chapter 11 simplifies
the inverse/implicit theorem titles while retaining their `C^k` hypotheses
and conclusions, and the optional local-volume argument gains its missing
maximum-norm estimate.

- Continuous Fubini remains first. The new general theorem proves outer
  integrability directly from product Darboux bounds without assuming section
  integrability. Thomae times Dirichlet supplies dense exceptional sections
  and shows why arbitrary replacement values can destroy outer integrability.
- Sections 13.9–13.17 separate the manifold foundations and later integration
  theory. Tangent equivalence precedes the tangent-space definition; forms
  and orientation have independent definitions. The orientation/top-form
  equivalence defers its partition-dependent direction until after that theorem.
- Tu is the primary pedagogical benchmark; Lee is the supplementary technical
  reference. The external refinement citation identifies Theorem 1.15 and
  the coordinate refinement in the proof of Theorem 2.23 (pp. 43–44), with
  Exercise 2.24 for boundary adaptation. No review lecture notes were added.
- Release notes and historical validation records are consolidated in this
  README. Standalone audit files are removed. No Git tag or GitHub release
  is created.

### Version 3.15.0 validation

- The final PDF has **372 pages**. pdfLaTeX completed successfully and the
  final two passes produced identical `main.aux`, `main.toc`, and `main.out`
  hashes. No LaTeX/package warnings, overfull/underfull boxes, undefined
  references or citations, duplicate labels, or extracted-text `??` remain.
- Checked **462 labels**, **488 reference uses**, **413 labeled statement
  destinations**, and **749 internal links**. Every statement destination
  lands on a page containing the correct result number; every internal
  link has an existing destination. Contents and cross-references reflect
  the new Chapter 13 numbering.
- Direct source comparisons confirm that continuous Riemann–Fubini,
  Chapter 13's classical opening, the partition-of-unity proof, the
  compact-boundary-extension and manifold-integration development, and
  the general Stokes section are unchanged. The inverse and implicit
  theorem statements retain their exact regularity hypotheses and
  conclusions, including `k = infinity`; only their names and relevant
  prose changed. Chapters 1–10 and both appendices were not edited.
- The new Darboux proof establishes boundedness and integrability of all
  four section functions through explicit finite-sum inequalities. It
  assumes product integrability, not section integrability. The exceptional
  example cites Chapter 9's Thomae function and gives its product-cell
  sums, section analysis, and arbitrary-assignment warning. No new measure
  theorem is used. The maximum-norm argument precedes its local-volume use.
- The manifold dependency check confirms local boundary designations precede
  chart-independence, tangent equivalence is proved before forming the tangent
  space, vector operations descend through linear transition maps, coordinate
  covectors are explicitly dual, and the intrinsic differential is introduced
  before its coordinate matrix. Forms and orientation are separate; orientation
  uses charts rather than undefined frames. Paracompactness first appears where
  partitions are needed. The top-form converse follows that partition theorem.
- The imported refinement retains its explicit external status and verified
  Lee citation. The common-refinement sum is finite on compact support;
  Stokes retains local finiteness, derivative-term cancellation, genuine-boundary
  extensions, artificial-edge zero extensions, and orientation signs.
- Visually inspected the contents, theorem-title changes, all new Chapter 12
  material, the maximum-norm estimate, the complete manifold-foundations
  sequence, partitions, integration, Stokes, and bibliography. The final
  review covers physical pages 1–9, 220, 225, 247–250, 268–269, 304–326,
  329–330 (including the new exercises), and 370–372. An isolated subsection heading was moved with its following
  text, and affected pages were inspected again.
- All 20 bibliography keys are unchanged; no review lecture-note attribution
  was introduced. Twenty-four historical audit documents and the correction
  history were preserved below. All 55 files with audit names, including
  obsolete scratch audit scripts and outputs, were removed. Historical
  README links now target the preserved records within this file.

## Version 3.14.1 — September 15, 2026

Version 3.14.1 replaces the matrix-pivot proof of local primitive factorization
by a successive-coordinate argument, closes the rank–minor and
differentiating-limits dependency gaps, clarifies primitive substitution and
inverse patching, and completes selected proof-prose and documentation cleanup
while preserving the Version 3.14.0 architecture. The Lagrange inversion example
now proves convergence by a coefficient bound and a geometric series.

Validation details are recorded in [historical validation record](#historical-revision-3.14.1-audit).
No Git tag or release was created.

## Version 3.14.0 — September 15, 2026

Chapter 11's local differential structure now leads to Chapter 12's structural
change of variables and Chapter 13's global manifold localization.

- Linear implicit function theorem and the nonlinear graph formula.
- Rank, nonzero-minor persistence, and the full Euclidean Constant Rank Theorem.
- Immersions, submersions, regular level sets, and dimension consequences;
  Chapter 12 supplies the lower-dimensional image covering argument.
- Optional analytic Lagrange inversion, explicitly distinguished from smooth IFT.
- Primitive local diffeomorphisms, explicit factorization, and finite Euclidean
  cutoffs and partitions of unity.
- Main change-of-variables proof by one-variable substitution, Fubini,
  composition, and finite smooth localization; Jordan boundary control is separate.
- Optional direct local-volume comparison using the inverse map, a Schwartz
  1954 perspective, and an unproved Lebesgue measure preview.
- Chapter 13 reuses Euclidean cutoffs and highlights the genuinely new locally
  finite manifold refinement. The complete-ball inverse-function proof is preserved.

Validation details are recorded in [historical validation record](#historical-revision-3.14.0-audit).
No Git tag or release was created.

## Version 3.13.1 — September 15, 2026

This finishing pass preserves the mathematical architecture of Version 3.13.0
while tightening its dependencies and proof presentation.

1. **Cumulative definitions:** Open and closed balls are introduced before
   topology and proved open/closed together after those notions are defined.
   Convex subsets and convex normed-space balls now precede the multivariable
   mean-value theory.
2. **Linear and affine notation:** `L(V,W)` and the convention
   `L(V) = L(V,V)` now appear with the first general linear maps. Affine maps,
   their base-point form, and invertible affine changes of coordinates are
   defined before the derivative's affine approximation.
3. **Proof naturalization:** Formulaic strategy labels and proof-auditor prose
   were selectively rewritten throughout Chapters 2--13 and the appendices.
   The inverse- and implicit-function arguments retain their quantitative
   architecture but now read as textbook proofs.
4. **Hidden mechanisms:** The revision exposes representative segment,
   finite-radius, operator-perturbation, compactness, exceptional-region, and
   little-o scale estimates where the earlier prose compressed real work.
5. **Finishing checks:** Chapter 9 wording, attribution sections, theorem
   anchor placement, and local page structure were synchronized and reviewed.

Build, reference, hyperlink, and visual-validation details are recorded in
[historical validation record](#historical-revision-3.13.1-audit). No Git tag or release was
created.

## Version 3.13.0 — September 15, 2026

This substantive revision rebuilds the metric dependency sequence and the
inverse-function proof while retaining the manuscript's scope.

1. **Chapter 10 dependency chain:** Euclidean norm notation now begins with
   Euclidean distance. Closure, boundary, limit points, isolated points, and
   all metric closed-set characterizations are consolidated, including their
   sequential forms. Closed balls, interior closed-ball containment, closed
   subsets of complete spaces, and finite-product convergence now provide the
   reusable metric machinery needed later.
2. **Operator norms:** A single characterization theorem identifies the
   operator norm through the unit ball, unit sphere, nonzero-vector ratios,
   optimal linear bound, and optimal Lipschitz constant. The standard
   bounded-linear-map equivalences and finite-dimensional maximum formula are
   made explicit.
3. **Chapter 11 specialization and inverse theorem:** The chapter now cites
   Chapter 10 for general metric limits and sequences, explains why the
   differentiability domain is open, and retains only the genuinely
   finite-dimensional limit techniques. The inverse function theorem is
   rebuilt around a fixed contraction constant $1/2$, an invariant complete
   closed ball, a checked segment hypothesis, a direct inverse-differentiation
   argument, and an explicit reversal of the normalization.
4. **Residual cleanup:** Chapter 9 distinguishes exceptional derivative
   identities from exceptional differentiability, sharpens the
   Dirichlet--Thomae discussion, and locally cites the unproved FTC/Cantor
   previews. The attribution note now identifies these previews accurately,
   and repetition in the higher-derivative discussion is reduced.

Build, reference, and visual-validation details are recorded in
[historical validation record](#historical-revision-3.13.0-audit). No Git tag or release was
created.

## Version 3.12.0 — September 14, 2026

This minor revision has three coordinated components:

1. **Chapters 8–9:** Darboux's theorem follows the Mean Value Theorem in
   §8.2. After the Lebesgue criterion and Dirichlet–Thomae discussion,
   §9.6 proves finite- and countable-exception Newton–Leibniz theorems,
   states the Lipschitz/almost-everywhere form, and gives the Cantor-function
   warning. Section 9.7 defines absolute continuity and previews both
   directions of the Lebesgue FTC. Proposition 9.4.12 and the elementary
   organization of §9.4 are preserved.
2. **Chapter 11:** The existing higher-derivative exposition now explicitly
   identifies operator-valued derivatives with multilinear maps, displays
   permutation symmetry, and distinguishes the second differential, its
   Hessian matrix, and evaluations on directions. Scalar and vector examples
   clarify the types. The second-order chain rule, line-restricted Taylor
   formula, multi-index expansion, and `C^k` inverse/implicit regularity are
   connected without duplicating the existing theory or changing the 3.11.0
   inverse/implicit proof architecture.
3. **Whole manuscript:** More than 80 individually considered prose edits
   across all thirteen chapters, both appendices, the preface, and reference
   annotations reduce repetitive transitions, generic praise, canned
   contrasts, and unnecessary proof narration. Mathematical scope and
   pedagogically significant distinctions are preserved.

Validation: the complete **348-page PDF** compiles to stable auxiliary files
with no LaTeX/package warnings, unresolved references, duplicate labels, or
overfull/underfull boxes. All **412 labels** are unique and all **438 reference
uses** resolve. The mathematical expressions in all **348 pre-existing proof
bodies** are preserved. Visual review covers **118 pages** containing changed
passages and surrounding context, including the cover and contents, with
enlarged inspection of the FTC and higher-derivative additions. Fifteen
selected theorem/example links land on their statement pages.

See [historical validation record](#historical-revision-3.12.0-audit) for exact locations,
the countable-exception proof audit, the Chapter 11 change inventory,
representative prose revisions, and build/visual-review results.
No Git tag or release was created.

## Previous revision: Version 3.11.0 — September 14, 2026

Chapter 11 now passes from the contraction theorem to a Euclidean open-ball
corollary, perturbation of invertible operators, smooth inversion on
`GL(R^n)`, and normalized inverse and implicit function theorems with `C^k` regularity of the inverse/implicit solution. The
inverse proof separates its `C^1` fixed-point core, regularity bootstrap, and
explicit undoing of the normalization. The implicit proof constructs its
graph from the inverse of `H(x,y)=(x,F(x,y))` before shrinking neighborhoods
or differentiating the graph equation.

Local repairs explain the Cauchy–Schwarz parameter choice and the secant-line
mechanism in the mean value theorem, display the exponential Cauchy product,
move the tagged-sum and polar previews into their logical settings, expose the
finite Darboux grouping in sectionwise Fubini, and distinguish intrinsic `df`
from its coordinate formulas. Anthony W. Knapp’s *Basic Real Analysis* is
added as a supplementary reference. Appendix B and its full Tensor–Hom
coverage remain unchanged.

Validation: the 342-page PDF builds without LaTeX warnings or layout-box
warnings; 399 unique labels and all reference uses pass the checks. Extracted
text has no unresolved `??`. Hyperlink destinations for the revised theorem
sequence and Theorem 9.3.1 land on the pages containing their statements.
The rendered pages containing every edit were inspected at full-page and
enlarged resolution.

See [historical validation record](#historical-pedagogy-3.11.0-audit) for the proof
architecture, preservation checks, hyperlink audit, and visual review.
No Git tag or release was created.

## Previous revision: Version 3.10.0 — September 14, 2026

Numbering convention: theorem-style environments share a counter within
each section (for example, Theorem 8.4.1). Subsections are unnumbered but
remain in the contents. Every chapter and appendix has an unnumbered Exercises
heading; exercises use a separate sequence, Exercise 1, 2, …, restarting
with each chapter or appendix, including any exercises embedded in its text.
References to unnumbered subsections use their linked titles.

Reviewed all 192 section/subsection openings and revised 31; reviewed all
349 proof bodies and expanded 12. The revision strengthens motivation before
definitions, explains theorem hypotheses and hidden proof estimates, and
adds three focused hypothesis examples. Analyticity now opens Chapter 8's
smooth-cutoff section after the elementary curves and polar material.
Appendix B gains transitions while retaining every proof and the complete
Tensor–Hom correspondence, with its existing vector-space and finite-sum scope.

Validation: the 343-page PDF builds without LaTeX warnings or layout-box
warnings; 399 unique labels and 434 reference uses pass the checks. Extracted
text has no unresolved `??`. Visual review covers 89 pages containing edited
passages and their surrounding context, including the cover and contents.

See [historical validation record](#historical-pedagogy-3.10.0-audit) for the complete opening
inventory, proof mechanisms, preservation checks, and validation details.
No Git tag or release was created.

## Previous revision: Version 3.9.0 — September 14, 2026

Elementary curves, velocity, speed, polar coordinates, and polar motion now
begin in Chapter 8 using only one-variable calculus. Chapter 10 collects the
standard coordinate norms and establishes the default Euclidean norm. Chapter
11 recalls curves in its first-order section, distinguishes differentiation
of a changing base point from differentiation of a fixed linear map, proves
the bilinear differentiation rule, and includes differential-evaluation and
curved-path examples. Chapter 9 translates integration-by-parts shorthand.
Chapter 13 adds polar pullback and circulation, explains arc length versus
coordinate differentials, and completes cotangent and coordinate-differential
notation. Appendix B is unchanged.

Validation: the 337-page PDF builds without LaTeX warnings or overfull/underfull
boxes; 399 labels and 432 reference uses pass the reference checks. Visual
review covers 63 pages containing edited passages and surrounding context.

See [historical validation record](#historical-pedagogy-3.9.0-audit) for the dependency,
preservation, and PDF checks. No Git tag or release is created.

## Previous revision: Version 3.8.0 — September 13, 2026

This focused revision makes covectors and coordinate differentials cumulative
across Chapters 10–13. Chapter 10 formally defines covectors and the dual space;
Chapter 11 derives coordinate differentials from coordinate projections,
explains the scalar differential, and applies the chain rule to parametrized
curves. Polar geometry now precedes its first use in limits, with its Jacobian
revisited after partial derivatives. Chapter 13 connects the same covectors to
wedges, forms, curve pullbacks, and oriented volume. Chapters 9 and 12 clarify
scalar integration notation. Local fixes cover candidate Jacobians, exterior
derivative regularity, surface-area notation, Taylor factorials, and the
analytic-series majorant. Appendix B changes only a page-break hint.

See [historical validation record](#historical-pedagogy-3.8.0-audit) for preservation,
definition-order checks, and PDF validation. No Git tag or release is created.

Validation: 330 PDF pages, 388 unique labels, 418 reference uses, and all 345
existing proof bodies preserved. The final build has no warnings or unresolved
references; 54 pages containing edited passages and their context were visually
reviewed, including the cover and contents.

## Previous revision: Version 3.7.0 — September 13, 2026

Chapter 8 develops repeated differentiation, derivative matching and uniqueness
of the Taylor polynomial, explicit error bounds, and the Taylor–Peano formula.
It distinguishes smooth finite-order approximation from analytic reconstruction.
Chapter 11 teaches coordinate-slice differentiation, candidate versus justified
Jacobians, Hessian computation, vector-valued second derivatives, and higher
symmetric multilinear derivatives. A modest multi-index introduction explains
analytic Taylor expansions and reuses the smooth cutoff as a counterexample.
Chapter 13 links symmetric derivatives to alternating forms and distinguishes
the Hessian D²f from the exterior identity d²f = 0.

Appendix B now derives finite tensor theory from a fixed recursive binary
realization. The direct quotient represents the same universal problem;
parenthesizations and finite bases are consequences, with induced maps built
recursively. Its quotient prelude, binary construction, Tensor–Hom treatment,
and exterior constructions remain. Finite direct sums only; no scalar changes
or exactness. Chapter 12 receives only Jacobian-determinant terminology fixes.

See [historical validation record](#historical-pedagogy-3.7.0-audit) for the focused revision,
dependency checks and PDF validation. No Git tag or release is created.

Validation: 326 PDF pages, 380 unique labels, 402 reference uses, no LaTeX
warnings or unresolved references, and visual review of 74 selected pages,
including the revised passages and the complete Appendix B.

## Previous revision: Version 3.6.0 — September 13, 2026

Chapter 10 adds Gaussian and Gauss–Jordan elimination, augmented matrices,
elementary matrices, inverse computation, and determinant calculations after
the structural determinant laws. Chapter 11 develops practical workflows for
joint limits and function sequences, and derives Jacobian columns from the
derivative's basis images. Local Taylor–Peano and Lagrange-multiplier references
are made precise. Chapter 12 uses Latin cell indices and identifies the exact
Chapter 9 mechanisms inherited by its integration and convergence proofs.

Appendix B is substantially reorganized and rewritten to follow Chapter 8 of
the author's current Algebra notes, specialized throughout to vector spaces.
It develops finite direct sums, finite multilinear products, induced maps,
exterior powers and alternating forms in that order. The full
previous Tensor–Hom discussion is retained verbatim, with compatibility added.
Exactness and restriction or extension of scalars are excluded. Chapters 9 and 13 and Appendix A are unchanged.

See [historical validation record](#historical-pedagogy-3.6.0-audit) for source alignment,
preservation, build, and visual-review evidence. No Git tag or release is created.

Validation: 322 PDF pages, 367 unique labels, no LaTeX warnings or unresolved
references, and visual review of 94 pages including the complete Appendix B.

## Previous revision: Version 3.5.0 — September 13, 2026

Chapter 10 now proves the required permutation signs in the main text, builds
linear continuity from basis-image estimates, explains operator norms and vector
series, and factors invertible maps geometrically into permutations, scalings,
and shears. Chapter 11 opens with limits and families of maps, including the
finite-dimensional Arzelà–Ascoli theorem, and adds differentiating limits,
second-order chain rules, Taylor error estimates, convexity, and local geometric
consequences of the inverse and implicit function theorems.

Chapter 12 now starts with concrete grids and Darboux approximation, teaching
common refinement before using it and postponing owned-cell step functions until
after continuous integrability. Coordinatewise FTC and integration by parts gain
worked computations. Multivariable Arzelà bounded convergence is proved using
elementary box content; Dini remains in Chapter 12. Chapter 9 and the appendices
receive only focused computational and notation changes.

See [historical validation record](#historical-pedagogy-3.5.0-audit) for preservation,
cross-reference, build, and visual-review evidence. No Git tag or release is created.

Validation: the rebuilt PDF has 316 pages. The final LaTeX log has no warnings,
undefined references, or overfull/underfull boxes; all 364 labels resolve, and
the extracted PDF text has no unresolved `??`. Focused visual review covers
81 pages, including the full revised Chapter 11 and the touched appendix pages.

## Previous revision: Version 3.4.1 — September 12, 2026

This finishing patch expands Chapter 12's volume examples into fully worked
cross-sectional derivations and completes Chapter 13's scalar surface and flux
computations. It improves the Chapter 11 affine-approximation figure and places
the circle picture with its implicit-function example. Appendix B displays its
central maps and separates the proof stages more clearly, following the available
Algebra Chapter 8 while preserving coverage. Small notation, exercise duplication,
cross-reference wording, and page-layout issues are repaired. No major theorem
scope or chapter architecture is added or changed.

See [historical validation record](#historical-polish-3.4.1-audit) for the focused change record,
preservation checks, and build/visual-review results. No Git tag or release is
created for this revision draft.

Validation: the stabilized PDF has 307 pages, with no LaTeX warnings,
undefined references, or overfull/underfull boxes. Visual review covered
80 distinct pages, including the complete Appendix B and references.

## Previous revision: Version 3.4.0 — September 12, 2026


Appendix B follows the editorial organization and pedagogical style of the
available Algebra Chapter 8 sources more closely, while remaining specialized
to vector spaces over a field. Its shorter quotient preparation leads into
construction, calculation, working rules, and structural consequences.
Chapters 11–12 gain concrete computations and explanatory TikZ figures.
Chapter 12 adds geometric volume calculations, worked substitutions,
visualization strategy, and a final integration problem-solving guide.
Chapter 13 adds routine line and surface integral calculations. No major
theorem scope is added; the Riemann/Jordan and manifold proof dependencies remain.

See [historical validation record](#historical-computational-3.4.0-audit) for the
preservation record and build/visual-review results. No Git tag or release
is created for this revision draft.

Validation: the stabilized PDF has 305 pages. The final LaTeX log has no warnings,
undefined references, duplicate labels, or overfull/underfull boxes. Visual review
covered 74 selected pages, including the complete rewritten Appendix B.

## Previous revision: Version 3.3.0 — September 12, 2026


This revision repairs rectangular integration dependencies, restores the informal
manifold preview immediately after classical patch Stokes, and develops exterior
algebra through low-degree examples. Appendix A explains field coefficients and
determinant normalization. Appendix B now places binary structural laws before
finite multilinear products, proves equivalence for every finite parenthesization,
and develops exterior maps, minors, and top determinant action before multiplication
and duality. Both appendices remain outside the main dependency route.

The detailed coverage matrix, source provenance, preservation checks, and actual
build/visual-review results are in
[historical validation record](#historical-consolidated-3.3.0-audit).
Version and date are synchronized through the preamble macros used by the title
page. No Git tag or release was created.

Validation performed: `latexmk -pdf main.tex` completed successfully, producing
295 pages with stable references, contents, numbering, and bibliography. The final
LaTeX log contains no warnings, undefined references, or overfull/underfull boxes.
Visual review covered every changed location and both appendices in full (84
distinct PDF pages including title, contents, and bibliography). The build launcher
reported a harmless Perl locale fallback; the document build succeeded.

## Previous revision: Version 3.2.0 — September 12, 2026

This minor revision explains object types and first-use mechanisms throughout
Chapters 11–13. Chapter 12 now begins with scalar rectangular step functions,
then Darboux integration, vector integration, and the multiple/iterated distinction.
Dependency repairs establish the extremum condition, half-space derivatives,
boundary structure, support under differentiation and boundary pullback, compact
cutoffs, continuous-form regularity, and zero-dimensional integration before use.
The existing chapter order and substantial proofs are preserved. Small supporting
changes address Chapter 8 regularity notation and Appendix B terminology.
See [historical validation record](#historical-pedagogical-dependency-3.2.0-audit)
for the item-by-item record, build results, and visual review. No tag or release
is created for this revision draft.

## Audience and prerequisites

The intended reader knows ordinary single-variable calculus and high-school
algebra and is beginning proof-based mathematics. The notes develop the
logical, set-theoretic, topological, and finite-dimensional linear-algebraic
language needed for their arguments. They do not attempt to develop measure
theory, Lebesgue integration, complex analysis, functional analysis, PDE, or
advanced differential geometry; these are discussed only as later directions.

## Reading the notes

The compiled document is [`main.pdf`](main.pdf). The chapters are intended to
be read in order. Formal definitions and proved results are distinguished from
examples and explicitly labelled informal previews. The core development is
proved internally except for the cited manifold-refinement theorem used in
Chapter 13. Optional topics are explicitly stated without proof:
analytic Lagrange inversion in Chapter 11; Lebesgue change of variables and
transformation of measure in Chapter 12; and stronger FTC results and the
Cantor function in Chapter 9. These optional previews carry local references
and are not prerequisites for the later internally proved development.
Section 13.17 also contains explicitly unproved previews, including dominated
convergence, Hilbert-space Riesz representation, Cauchy’s integral formula,
the de Rham theorem, and the maximum principle.

## Build

The project is designed for **pdfLaTeX**. From the repository root, run:

```text
latexmk -pdf main.tex
```

Alternatively, run `pdflatex main.tex` repeatedly until the table of contents,
cross-references, and bibliography stabilize. The project uses standard AMS
packages, `hyperref`, `cleveref`, `enumitem`, `xcolor`, TikZ (including `tikz-cd`),
`needspace`, and Latin Modern fonts.
The bibliography is written directly in LaTeX; no BibTeX or Biber step is
required. No absolute local paths, external figure-generation tools, or downloads
are required to build the PDF.

## References and external dependencies

The document contains a short bibliography. The core development is proved
internally except for the explicitly cited manifold-refinement theorem used
in Chapter 13. The stated-but-unproved optional results are analytic Lagrange
inversion (Chapter 11), Lebesgue change of variables / transformation of
measure (Chapter 12), and the Lipschitz/a.e. and Lebesgue FTC extensions and
Cantor function (Chapter 9), together with the additional explicitly unproved
preview theorems in §13.17. None of these optional
previews is a prerequisite for the later internally proved development.
Appendix A states ordinary and transfinite recursion without proof, proves
Hartogs’s lemma, and proves the equivalence of AC, Well-Ordering, and Zorn;
Appendix H marks the homological structural theorems and de Rham comparison
as unproved. These appendices remain optional.
The remaining entries are supplementary benchmark and
further-reading references. Specific acknowledgments to the author's algebra
notes cover the determinant expansion, influence on the permutation
exposition, and Appendix D's proof architecture; they do not describe the
origin of the entire manuscript.

## AI-assisted preparation

OpenAI Codex was used extensively in drafting, revising, proofreading, and
preparing the LaTeX source for these notes. The author determined the scope
and mathematical organization, made the final decisions about retained
content, and is responsible for approving and verifying the correctness of the
published version. Codex is not listed as a coauthor.

Before publication, the author should verify any AI-authorship or disclosure
policy imposed by the intended university, repository, publisher, or platform.

## License and copyright

Copyright \(\copyright\) 2026 Tommy Chen. This work is licensed under the
[Creative Commons Attribution 4.0 International License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).
You may share and adapt the notes under the terms of that license, with
appropriate attribution.

## Errors and errata

The notes may contain errors. Please report them through
[GitHub Issues](https://github.com/tommychen99/mathematical-analysis/issues)
or record them in [`ERRATA.md`](ERRATA.md).

## Revision notes

### Focused proof-and-dependency patch — version 3.1.1 (September 12, 2026)

Closes the early continuity-composition dependency, gives finite-threshold
proofs for infinite L'Hôpital variants, and makes local integrability and
linear-image measurability explicit. Chapter 13 now constructs a single
extension near compact boundary-chart supports and proves agreement of
manifold integration with the earlier Riemann/Jordan integral before the
classical corollaries. Small domain, title, grammar, and exercise-presentation
repairs preserve the existing architecture and Appendix B.

See [historical validation record](#historical-patch-3.1.1-audit) for the focused audit and
build/visual validation.

### Focused dependency-and-exposition revision — version 3.1.0 (September 12, 2026)

This pass preserves the architecture of 3.0.0. Chapter 13 now defines smooth
maps locally with explicit chart domains and constructs manifold pullback,
wedge product, and the chart-independent exterior derivative before global
integration. Surface definitions are separated, and general-dimensional flux
is defined before the divergence theorem.

Chapter 12 makes the grid-face values in lower/upper step functions explicit,
repairs the remainder-strip description in the exact-grid case, and proves
elementary Jordan-set algebra. The correct closed sequence tails and
compact-closure derivative maximum are verified and preserved. Convergence
remarks distinguish uniform convergence from the one-dimensional Arzelà
theorem with its separately assumed integrable limit.

Chapter 10 adds a positive direct-sum calculation, defines matrix-space
operations, consolidates repeated examples, and compares exact operator norms
with different values. Appendix B adds concrete finite-distributivity and
three-factor applications and proves compatibility with Chapter 13's shuffle
product. Exercises, specific cross-references, and attribution are updated.

See [historical validation record](#historical-focused-dependency-audit) for the request
map, preservation checks, compilation, and visual review.

### Major proof-architecture revision — version 3.0.0 (September 12, 2026)

Chapter 10 now has eighteen sections. Its topology introduction begins with
distance, balls, ambient-space examples, convergence, and metric continuity;
then develops abstract topology, finite products, separate compactness proofs,
finite nets, Lebesgue numbers, and connectedness. The linear-algebra introduction
adds displayed axioms, coefficient calculations, explicit coordinate inverses,
internal and external direct sums, basis-value map construction, and a two-part
rank–nullity proof. Matrices remain derived from basis images and composition.

Appendix B has thirteen sections, beginning with quotient vector spaces and
universal factorization. It separates formal-basis extension from quotient
factorization and develops tensor uniqueness, basis detectors, the scalar
isomorphism, symmetry, finite distributivity, multivariable products,
associativity, Tensor–Hom maps, alternating quotients, exterior multiplication,
duality, and the top exterior power. Canonical isomorphisms have constructed
forward and reverse maps with both composites checked. The scope remains
vector spaces over fields.

Targeted proofs in Chapters 2–9 now expose representative independence,
subsequence choices, finite-sum comparisons, and the order of parameter choices.
The interval open-cover proof precedes its use in Arzelà's argument. Chapters
11–13 add higher inverse regularity, a staged compact-Jordan-region proof,
noncircular polar error bounds, tangent transition and differential constructions,
local finiteness, explicit Stokes signs, and common-refinement integration.
A two-chart partition-of-unity calculation recovers the circle integral 2π.
The trigonometric-series example now asserts only the continuity established
by its supplied proof, rather than an uncited nowhere-differentiability theorem.

See [historical validation record](#historical-proof-architecture-audit) for the request
coverage, preserved arguments, dependency audit, and compilation/visual record.

### Earlier major pedagogical revision — version 2.0.0 (September 12, 2026)

Version 2.0.0 was the preceding local revision draft. Chapter 10 was reorganized into
twelve sections, separating metric and topological foundations, vector spaces,
linear transformations, matrix representations, composition, coordinate changes,
inner products and norms, operator estimates, duality and multilinearity,
determinants and orientation, and the transition to differentiation. Worked
coordinate and determinant calculations accompany the structural proofs.

Appendix A develops permutations through bijections, cycles, swaps, inversions,
and parity without group-theory prerequisites. Appendix B expands quotient
constructions, tensor and exterior universal properties, canonical isomorphisms,
coordinate detectors, induced maps, exterior multiplication, and duality over
fields only. The determinant proof uses the elementary parity facts stated in
Chapter 10 and proved in Appendix A; no further appendix machinery is needed
for Chapters 11–13.

Part I adds examples, proof explanations, and exercises, strengthens the
equicontinuous pointwise-limit result, and proves Arzelà bounded convergence
internally with pointwise convergence and an integrable limit. It repairs the
power-series radius argument and makes the continuous FTC a corollary of the
accumulation-function result. Chapter 12 repairs the rectangle example and
boundary-cover arguments. Chapter 13 separates geometric objects from their
coordinates and uses intrinsic tangent orientations with explicit boundary
chart signs. Bartle has been added as an analysis companion.

See [historical validation record](#historical-major-pedagogical-audit) for the change map,
source-consultation scope, dependency checks, and validation record.

### Earlier 1.3.0 revision draft


The 1.3.0 draft revises the real-number construction and decimal foundations,
repairs reciprocal and boundedness arguments, and adds tagged sums and the
smooth cutoff. Part II adds linear-algebra preparation, worked derivatives,
graph-region and compact-support change of variables, and a classical
curve/surface bridge to forms. Boundary tangent spaces and chart integration
are treated explicitly. See [historical validation record](#historical-revision-audit) for the
correction map, dependencies, and validation record.

### Focused foundations revision (September 11, 2026)

Chapter 5 expands limit points, isolated-point continuity, and precise O/o
estimates. At that revision, Chapter 10 had seven sections: topology; products and
compactness; vector spaces and linear maps; norms; duality and multilinearity;
determinants and orientation; and transition to differentiation. Matrices
are derived from basis images and composition. The determinant proof adapts
the slot-by-slot expansion of Theorem 5.12.3 in the author's algebra notes.
Chapter 11 connects higher derivatives to symmetric multilinear maps;
Chapter 13 starts exterior algebra from elementary wedges and their basis.
Two structural appendices cover permutation parity and determinants over a
field, and tensor products and exterior powers. They are not prerequisites
for the analysis chapters. See [historical validation record](#historical-focused-revision-audit).

### Previous version

Version 1.2.0 expands Chapter 9's proofs of the Darboux criterion, basic
integral properties, additivity, absolute-value estimates, and integrability
of monotone functions. It also corrects the wording in Theorem 9.7(b): the
oscillation of $f$ is described as the supremum of the possible differences
$|f(x)-f(y)|$, without assuming that the supremum or infimum is attained.

## Release preparation

**Release-note policy:** Keep all current and future release notes and their
validation summaries in this README. Do not create separate release-note or
audit files. Historical records below describe their original versions; old
result numbers and validation counts are not claims about the current build.

This is a local revision draft. No Git tag or GitHub release has been created. Keep the version and revision date synchronized between
`preamble.tex`, the title page, and this README. Use a patch release (for
example, `1.1.2`) for minor corrections, a minor release (for example, `1.2.0`)
for meaningful additions or improvements, and a major release (for example,
`2.0.0`) for substantial restructuring.

## Historical revision and validation records

The following records were moved from the former standalone audit files.
They preserve historical findings, including issues subsequently corrected.

<a id="historical-computational-3.4.0-audit"></a>
<details>
<summary>COMPUTATIONAL 3.4.0 AUDIT</summary>

# Computational and editorial audit — Version 3.4.0 (revision draft)

Revision date: September 12, 2026. Local revision draft; no Git tag or GitHub release.

## Baseline and editorial source

The baseline is the actual Version 3.3.0 working tree, preserved with its PDF
under `tmp/revision-340-baseline/`. Existing uncommitted work and the files named
“Copy” were preserved. Git HEAD was not substituted for that baseline.
The available sibling Algebra Chapter 8 sources, `chapters/tensor-products.tex`
and its exterior-algebra input, supplied the editorial benchmark. No claim is
made about a newer remote edition. The analysis appendix retains vector spaces
over a field and does not import the algebra chapter's module-theoretic scope.

## Coverage and organization

| Target | Revision |
|---|---|
| 11: differentiability workflow | Visible numbered box; ordinary vector-valued continuous-partials calculation; continuous-with-partials counterexample; existing strict hierarchy retained. |
| 11: geometry | Quadratic surface and affine tangent plane with exact and numerical remainder; elliptical levels with gradient and three unit directional derivatives; circle graph choices; ellipse tangent/normal and brief two-component hyperbola. |
| 11: practice | Classification of continuity/partials/directions/differentiability, direct remainder estimate, conic tangent and normal. |
| 12: foundations visualized | Lower/upper Darboux columns beside the retained four-cell computation; 20-cell sum grouped in two orders; short accurately scoped Riemann–Fubini versus Fubini–Tonelli remark. |
| 12: region descriptions | Parabolic region in both orders, representative slices, area and nonconstant integral; retained triangles with a diagram explaining the split at x=1. |
| 12: volumes | Cylinder, cone, ball by cross-sections; projection workflow for all three coordinate planes; ellipse and ellipsoid by linear scaling. |
| 12: substitutions | Ellipse with a nonconstant integrand and two successive substitutions; x+y and x−y coordinates; nonlinear square-to-trapezoid map; radial fourth-power integral; cylindrical cone with explicit derivative and controlled exceptions. |
| 12: figures and strategy | Source/target disk–ellipse, square–diamond, square–trapezoid, polar rectangle–sector; cylinder/cone and ball slices; boxed substitution warnings; final eight-step strategy and method-comparison exercise. |
| 13: computation | Line and surface workflows; wire mass, segment work, helix length/density; plane area and cylinder side area/flux. Helix and plane illustrations. |
| 13: local repairs | Displayed Alt definition; term-by-term first wedge computation; associativity by existing trilinear maps and spanning; stable k/N parametrized-integration notation; explicit north-pole disk chart; roadmap under patch-Stokes heading. |
| B: quotient preparation | Shorter coset/operation proofs, first isomorphism theorem as an application, retained factorization/basis/complement mechanism. General universal-property discussion moved into the tensor encounter. |
| B: tensor pacing | Universal problem → explicit construction → working rule and calculation → canonical uniqueness; arithmetic as working facts; shortened analogous symmetry/distributivity/induced-map proofs. |
| B: exterior pacing | Early two-dimensional wedge calculation, exterior working rule, basis/minor expansion/nonvanishing, structural induced-map proof followed by short proof, determinant-line payoff, intended product before well-definedness construction, complete F^3 degree table and mixed-degree products. |
| B: local repairs | Named associativity maps in direct three-factor comparison, explicit linear T in assembled exterior homomorphism, explicit endomorphism hypothesis for top-covector scaling. |

The optional inverse-function grid deformation was omitted: the existing inverse
theorem application remains, while the three requested Chapter 11 figure types
are supplied. Cylindrical geometry uses the cone slices and polar sector together;
no spherical-coordinate section was added. The existing plane-area exercise was
adapted to scalar density and flux, avoiding repetition of the promoted calculation.

Appendix B now has twelve sections: quotients; bilinear problem and construction;
tensor bases; binary laws; binary induced maps; finite products; Tensor–Hom;
exterior powers; exterior maps/minors/determinants; multiplication; exterior
algebra; duality. README, OUTLINE, and the architectural-audit entry point reflect
the new arrangement. Historical version audit files retain their historical records.

## Preservation and mathematical checks

Only Chapters 11, 12, 13, and Appendix B differ from their baseline chapter files.
Chapter 10, Appendix A, Chapters 1–9, preface, and references are byte-identical
to the saved baseline. Main manuscript inputs and the classical-to-intrinsic
sequence are unchanged. Appendix B remains outside the main dependency route.

All 22 Chapter 11 and all 29 Chapter 12 proof bodies are unchanged. In Chapter 13,
33 of 35 are unchanged; the two modifications are the requested gentler
wedge-associativity proof and the parameter-dimension notation correction.
The first-order extremum condition, half-space derivative lemma, boundary
classification/structure, support lemmas, cutoffs, continuous-form convention,
zero-dimensional integration, common refinement, manifold–Riemann agreement,
general Stokes, and ambient-form restriction repairs remain in place.

Disk area in the early cross-section computations is justified by Cartesian
slices and one-variable trigonometric substitution, so it does not presuppose
the later polar theorem. Section-integrability, not the continuous-rectangle
Fubini theorem, justifies zero-extended indicators. Boundary nullity uses finite
Lipschitz pieces. Cylindrical central/seam errors have explicit box bounds;
the original noncircular polar truncation proof is unchanged.

Substitutions specify source-to-target maps and determinant direction. The
linear-expression inverse has absolute determinant 1/2, not 2. The trapezoid
integrand contributes one factor 1+u and the area element another. Polar order
(r,theta) in the new examples is explicitly distinguished from (theta,r) in
the retained example. Scalar integrals use absolute determinants; work/flux
retain orientation. Cylinder sides use two patches to remove the repeated seam.

Direct calculations checked: wire mass 2R²; segment work 2; helix length
2π√(R²+c²); plane area √6; cylinder side area 2πRh and flux 2πR²h;
parabolic area 4/3 and integral of y equal to 4/5; cylinder/cone/ball volumes;
ellipse area πab and normalized quadratic integral πab/2; diamond integral 4/3;
trapezoid integral of y equal to 7/6; radial fourth-power integral πR⁶/3.

## Build and visual review

Validation evidence is stored in `tmp/build-340-final.txt`, `main.log`, and
`tmp/qa340/`. The requested `latexmk -pdf main.tex` build is run with
`-interaction=nonstopmode -halt-on-error` for diagnostics. Installed MiKTeX is
invoked by its absolute executable path because it is not on the desktop PATH.

The source audit checks labels and references across every active input, excluding
the unused “Copy” sources. Visual review covers the differentiability sequence,
all new figures and computations, the strategy guide, the classical calculations,
and the complete Appendix B including exercises. Figure explanations found to
cross a page boundary were kept with their diagrams in the final layout pass.

The stabilized build produces 305 PDF pages. Its final LaTeX log has no warnings,
undefined references, multiply defined labels, or overfull/underfull boxes.
The active-source audit finds 349 distinct labels and 380 reference uses, with
no missing targets or duplicate labels. The MiKTeX launcher prints a harmless
Perl locale fallback; latexmk completes successfully.

Rendered 74 selected pages with Poppler, inspected contact sheets for the full
selection and individual pages for the new diagrams and pagination repairs.
The complete Appendix B occupies PDF pages 278–303; every page was included
in the continuous-reading review. The final trapezoid-label adjustment was
checked separately at full-page scale. QA page inventory is in
`tmp/qa340/pages.json`; source preservation results are in
`tmp/qa340/source-audit.txt`. No new figure has an explanation stranded from it,
and no diagram label overlaps a boundary after the final adjustment.

</details>

<a id="historical-consolidated-3.3.0-audit"></a>
<details>
<summary>CONSOLIDATED 3.3.0 AUDIT</summary>

# Consolidated pedagogical and dependency audit — Version 3.3.0

Revision date: September 12, 2026. Local revision draft; no tag, commit, or GitHub release created.

## Baseline and source provenance

Work used the actual working-tree LaTeX sources, whose preamble and README identified
Version 3.2.0 (revision draft), September 12, 2026. The timestamp-named PDF and README
in the request were not separately present in the workspace; exact byte identity with
those exports was not independently established. The pre-edit sources, README,
preamble and PDF are preserved under `tmp/revision-330-baseline/`. Existing uncommitted
work was retained; Git HEAD was not substituted for this baseline.

Consulted the available sibling Algebra source: `chapters/tensor-products.tex`
(Chapter 8), its `chapters/exterior-algebra.tex` input, permutation material in
`chapters/groups-foundations.tex` (Section 1.5), and determinant exposition in
`chapters/modules.tex` (Section 5.12). Used these for motivation and sequence,
specializing to vector spaces and preserving the analysis appendix's fuller proofs.
The older preview was available in `chapters/ch13-forms-stokes - Copy.tex`; its
local-to-global principle and Chapter 10–12 bridge were adapted to the current
classical-first route. No claim is made to have consulted an unavailable export or
new edition of any reference. No module, ring, group, bundle, measure, spectral, or
derivation theory was introduced.

## Dependency order and substantive findings

Chapter 12: owned-cell step sum → Darboux definition/criterion → compatibility and
worked grid → continuity/scalar linearity → restriction/gluing/additivity → face strips
and rectangular zero extension → translation → vector integration/Fubini → Jordan
sets/null modifications → linear/nonlinear change of variables. Jordan finite-union
volume uses the early face-strip result, so does not presuppose general null modification.
Fubini tags are explicitly chosen once per factor cell. Closed faces never become
literally disjoint in these arguments.

Chapter 13: classical curves/Green/surfaces/patch Stokes and box divergence → **13.5
Beyond One Parametrization: Why Manifolds?** (informal) → **13.6 alternating covectors,
elementary wedges, basis, shuffle product and exterior algebra** → varying forms →
Euclidean and half-space form integrals → formal manifolds/tangents/differential →
localization/global integral → Stokes. Signed finite sets are introduced before use;
the discrete-manifold compactness justification appears after the formal definitions.

Appendix B: **B.1** quotients; **B.2–B.4** binary universal problem, formal construction,
arithmetic and bases; **B.5** unit, symmetry, binary associativity, finite distributivity;
**B.6** named induced binary maps; **B.7** direct finite products, three-factor comparison,
all-parenthesizations induction, tensor powers/maps; **B.8** Tensor–Hom/finite dual map;
**B.9** exterior universal problem, repeated relations, calculations, basis/nonvanishing;
**B.10** exterior maps, minors, determinant action; **B.11** multiplication; **B.12**
finite exterior algebra and assembled homomorphism; **B.13** duality, compatibility with
maps and the main-text shuffle product. Dimensions are finite where counted;
characteristic two, degree zero and above-dimension cases are included.

The determinant result is retrospective: exterior-basis detectors already use
determinant theory. Its four viewpoints are normalized alternation, Leibniz, recursive
Laplace (empty determinant 1), and top exterior action. It is not a replacement
foundation for the earlier determinant proofs.

## Coverage matrix

Request numbers refer to the user's consolidated prompt; locations refer to the revised
source. Each row identifies concrete content and its treatment. A retained row does not
claim a new proof. Combined rows group related clauses rather than infer completion
from the mere presence of terminology. The optional accumulating-bumps illustration
was not added because the neighborhood definition and local-finiteness proof already
give the needed distinction; the required content is retained.

| Request | Content and disposition | Status | Revised location |
|---|---|---|---|
| 1 | Scope, finite-dimensional formulas, arbitrary-vector-space constructions, finite factors/sums, structural appendices | already present and retained | Chapter B opening; [app-tensors.tex:9](chapters/app-tensors.tex#L9) |
| 1 | Preserve the working 3.2.0 source and existing proofs, not a reset to Git HEAD | already present and retained | Chapter B opening; [app-tensors.tex:14](chapters/app-tensors.tex#L14) |
| 2 | Problem before construction; map types, well-definedness, reverse maps and both composites | newly implemented | B.7; [app-tensors.tex:849](chapters/app-tensors.tex#L849) |
| 2 | Algebra Chapter 8 pacing adapted to vector spaces; detailed quotient/tensor diagrams retained | already present and retained | B.1; [app-tensors.tex:83](chapters/app-tensors.tex#L83) |
| 2 | Elementary tensor/wedge terminology; canonical isomorphism versus equality and coordinates versus decompositions | locally corrected | B.5.2; [app-tensors.tex:490](chapters/app-tensors.tex#L490) |
| 3A | Owned-cell step integral independent through common owned-cell refinement | already present and retained | 12.1; [ch12-multivariable-integration.tex:59](chapters/ch12-multivariable-integration.tex#L59) |
| 3A | Step compatibility after Darboux criterion, strips bounded by 2M delta, preliminary sum squeezed by both sums | locally corrected | 12.1; [ch12-multivariable-integration.tex:139](chapters/ch12-multivariable-integration.tex#L139) |
| 3B | Closed shared faces treated by thin strips, not identically zero | locally corrected | 12.1.1; [ch12-multivariable-integration.tex:316](chapters/ch12-multivariable-integration.tex#L316) |
| 3B | Restriction, finite grid gluing and scalar integral additivity proved from grids | newly implemented | 12.1.1; [ch12-multivariable-integration.tex:294](chapters/ch12-multivariable-integration.tex#L294) |
| 3B | Zero extension and unrelated containing rectangles handled before Jordan volume independence | locally corrected | 12.3; [ch12-multivariable-integration.tex:752](chapters/ch12-multivariable-integration.tex#L752) |
| 3B | Translation of grids/integrands, then Jordan translation before local volume comparison | newly implemented | 12.1.1; [ch12-multivariable-integration.tex:336](chapters/ch12-multivariable-integration.tex#L336) |
| 3C | Segment Taylor integer k>=0; second derivative only k>=1; componentwise intermediate points | locally corrected | 11.2; [ch11-multivariable-differentiation.tex:753](chapters/ch11-multivariable-differentiation.tex#L753) |
| 3C | Single implicit-function motivation retaining block derivative definitions and equal dimensions | locally corrected | 11.4; [ch11-multivariable-differentiation.tex:1343](chapters/ch11-multivariable-differentiation.tex#L1343) |
| 3C | Remove repeated Lagrange kernel summary, retain graph velocities and functional decomposition | locally corrected | 11.4; [ch11-multivariable-differentiation.tex:1602](chapters/ch11-multivariable-differentiation.tex#L1602) |
| 3C | Derivatives transport tangent directions; pullbacks transport covectors/forms | locally corrected | 11.5; [ch11-multivariable-differentiation.tex:1786](chapters/ch11-multivariable-differentiation.tex#L1786) |
| 3D | Define C([a,b]) at first occurrence and distinguish whole f_k from f_k(x) | newly implemented | Chapter 6 opening; [ch06-function-sequences.tex:4](chapters/ch06-function-sequences.tex#L4) |
| 3D | Accumulation endpoint x versus bound dummy t; renaming does not change F | newly implemented | 9.4; [ch09-riemann-integration.tex:743](chapters/ch09-riemann-integration.tex#L743) |
| 3D | Chapter 5 composition, isolated points, O/o, infinite L'Hopital, improper comparison hypotheses | already present and retained | Chapter 5 opening; [ch05-limits-continuity.tex:1](chapters/ch05-limits-continuity.tex#L1) |
| 3D | Early C^k convention and differentiation/improper integration repairs left intact | already present and retained | Chapter 8 opening; [ch08-differentiation.tex:1](chapters/ch08-differentiation.tex#L1) |
| 4 | Frechet norm ratio, epsilon-delta, open domain, affine output approximation and zero remainder | already present and retained | 11.1; [ch11-multivariable-differentiation.tex:29](chapters/ch11-multivariable-differentiation.tex#L29) |
| 4 | Uniqueness along h=tv with t-independent normalized expression and continuity norm estimate | already present and retained | 11.1; [ch11-multivariable-differentiation.tex:108](chapters/ch11-multivariable-differentiation.tex#L108) |
| 4 | Fixed direction versus speed, unit rate, coordinate partials; explicit remainder/abs(t), v=0 | locally corrected | 11.1; [ch11-multivariable-differentiation.tex:270](chapters/ch11-multivariable-differentiation.tex#L270) |
| 4 | Polynomial first; homogeneity versus additivity; changing-direction path; directional assignment versus scalar value | already present and retained | 11.1; [ch11-multivariable-differentiation.tex:63](chapters/ch11-multivariable-differentiation.tex#L63) |
| 4 | Pointwise versus uniform directional quantifiers without a new derivative theory | already present and retained | 11.1; [ch11-multivariable-differentiation.tex:349](chapters/ch11-multivariable-differentiation.tex#L349) |
| 4 | Output-component differentiability in all inputs and finite remainder bounds; matrix entries versus columns | already present and retained | 11.1; [ch11-multivariable-differentiation.tex:299](chapters/ch11-multivariable-differentiation.tex#L299) |
| 4 | Zero coordinate increments handled before mean value theorem | already present and retained | 11.1; [ch11-multivariable-differentiation.tex:371](chapters/ch11-multivariable-differentiation.tex#L371) |
| 4 | Operator C1 versus entrywise continuity; differentiable but not C1 example | already present and retained | 11.1; [ch11-multivariable-differentiation.tex:397](chapters/ch11-multivariable-differentiation.tex#L397) |
| 4 | First-order extrema, maximal gradient directional rate and local Lipschitz consequence | already present and retained | 11.2; [ch11-multivariable-differentiation.tex:703](chapters/ch11-multivariable-differentiation.tex#L703) |
| 4 | Multilinear norms, segment derivatives, worked quadratic, Hessian versus diagonal; compactness and extrema in second-order test | already present and retained | 11.2; [ch11-multivariable-differentiation.tex:518](chapters/ch11-multivariable-differentiation.tex#L518) |
| 4 | Contraction geometric Cauchy estimate, limit, completeness, self-map and q<1 | already present and retained | 11.3; [ch11-multivariable-differentiation.tex:865](chapters/ch11-multivariable-differentiation.tex#L865) |
| 4 | Inverse correction map, nontrivial source/target example, injectivity versus inverse; detailed inverse and higher regularity | already present and retained | 11.4; [ch11-multivariable-differentiation.tex:976](chapters/ch11-multivariable-differentiation.tex#L976) |
| 4 | Implicit proof, block computations and higher regularity preserved | already present and retained | 11.4; [ch11-multivariable-differentiation.tex:1351](chapters/ch11-multivariable-differentiation.tex#L1351) |
| 4 | Lagrange candidates versus classification, y^2 versus y, cusp exercise, exercises before transition | already present and retained | 11.4; [ch11-multivariable-differentiation.tex:1616](chapters/ch11-multivariable-differentiation.tex#L1616) |
| 5 | Scalar-first input x as one vector, output one ordered real, bounded value sets, vector-index inf/sup | locally corrected | 12.1; [ch12-multivariable-integration.tex:12](chapters/ch12-multivariable-integration.tex#L12) |
| 5 | Rectangle volume, owned cells, lower/upper approximations and the two refinement ingredients | already present and retained | 12.1; [ch12-multivariable-integration.tex:44](chapters/ch12-multivariable-integration.tex#L44) |
| 5 | Four-cell x+y example, areas/heights L=1/2 U=3/2; m-grid gap without Fubini | newly implemented | 12.1; [ch12-multivariable-integration.tex:163](chapters/ch12-multivariable-integration.tex#L163) |
| 5 | Expanded coordinate-volume notation, double/triple/multiple naming and dA/dV not form identities | locally corrected | 12.1; [ch12-multivariable-integration.tex:99](chapters/ch12-multivariable-integration.tex#L99) |
| 5 | Vector integration follows scalar linearity; arbitrary linear output map and continuity, no denial of partial orders | already present and retained | 12.1.1; [ch12-multivariable-integration.tex:347](chapters/ch12-multivariable-integration.tex#L347) |
| 5 | Fubini blocks, section f(x,dot), scalar G, remaining integration, integral estimate reference | already present and retained | 12.2; [ch12-multivariable-integration.tex:412](chapters/ch12-multivariable-integration.tex#L412) |
| 5 | Consistent x_R and y_S chosen once per factor cell | locally corrected | 12.2; [ch12-multivariable-integration.tex:460](chapters/ch12-multivariable-integration.tex#L460) |
| 5 | Two-dimensional integration by parts before hats, face functions, explicit omission and n=1 endpoint | locally corrected | 12.2; [ch12-multivariable-integration.tex:513](chapters/ch12-multivariable-integration.tex#L513) |
| 5 | Zero-extension domain and integrability distinction; Jordan measurability does not integrate every bounded function | already present and retained | 12.3; [ch12-multivariable-integration.tex:860](chapters/ch12-multivariable-integration.tex#L860) |
| 5 | Compact support defined before open integrals; rectangle contains support, not whole domain | already present and retained | 12.5; [ch12-multivariable-integration.tex:1874](chapters/ch12-multivariable-integration.tex#L1874) |
| 5 | Linear COV grid steps linked to owned-cell convention and later null modifications | locally corrected | 12.4; [ch12-multivariable-integration.tex:1159](chapters/ch12-multivariable-integration.tex#L1159) |
| 5 | COV source/target diagram, scalar transformed function, substitution versus dummy renaming | already present and retained | 12.5; [ch12-multivariable-integration.tex:1247](chapters/ch12-multivariable-integration.tex#L1247) |
| 5 | Five-operation normalization, separate errors, exact-grid remainders, measurability before volume | already present and retained | 12.5; [ch12-multivariable-integration.tex:1289](chapters/ch12-multivariable-integration.tex#L1289) |
| 5 | Early polar motivation with linear scaling/local linearization/uniform bounds/summation plan | locally corrected | 12.3; [ch12-multivariable-integration.tex:581](chapters/ch12-multivariable-integration.tex#L581) |
| 5 | Rigorous polar small-disk/seam errors preserved; parameter order versus nested instruction and wedge sign | locally corrected | 12.5.1; [ch12-multivariable-integration.tex:2062](chapters/ch12-multivariable-integration.tex#L2062) |
| 5 | Cell osc, pointwise omega and uniform mu distinguished with diameter bound | already present and retained | 12.1; [ch12-multivariable-integration.tex:181](chapters/ch12-multivariable-integration.tex#L181) |
| 5 | Convergence x vector, k sequence, n dimension; uniform and Arzela with separately integrable limit; no new multivariable Arzela | already present and retained | 12.6; [ch12-multivariable-integration.tex:2104](chapters/ch12-multivariable-integration.tex#L2104) |
| 6 | Restore preview immediately after full classical Stokes including box divergence; formal manifold definitions remain later | newly implemented | 13.5; [ch13-forms-stokes.tex:494](chapters/ch13-forms-stokes.tex#L494) |
| 6 | Circle/sphere/torus local dimensions; actual upper/right circle charts, transitions, no global chart or repeated traversal chart | newly implemented | 13.5; [ch13-forms-stokes.tex:503](chapters/ch13-forms-stokes.tex#L503) |
| 6 | Chart direction versus inverse parametrization; compactness obstruction for one chart | newly implemented | 13.5; [ch13-forms-stokes.tex:514](chapters/ch13-forms-stokes.tex#L514) |
| 6 | Local coordinate independence, tangent space versus curved M and coordinate vectors; alternating rules | newly implemented | 13.5; [ch13-forms-stokes.tex:515](chapters/ch13-forms-stokes.tex#L515) |
| 6 | Interval/disk/circle intrinsic boundary and half-space preview distinct from ambient boundary | newly implemented | 13.5; [ch13-forms-stokes.tex:523](chapters/ch13-forms-stokes.tex#L523) |
| 6 | Overlap compatibility and smooth localization motivate pullbacks, orientation, partitions; Chapters 10-12 roles | newly implemented | 13.5; [ch13-forms-stokes.tex:531](chapters/ch13-forms-stokes.tex#L531) |
| 6 | Preview explicitly informal; combine with Why Forms rather than repeat transitions | newly implemented | 13.5; [ch13-forms-stokes.tex:496](chapters/ch13-forms-stokes.tex#L496) |
| 7 | Main text through real alternating covectors, independent of tensor quotients | already present and retained | 13.6; [ch13-forms-stokes.tex:567](chapters/ch13-forms-stokes.tex#L567) |
| 7 | Low-degree input/output and zero/one/above-dimension conventions; signed-area rule before determinant | newly implemented | 13.6; [ch13-forms-stokes.tex:583](chapters/ch13-forms-stokes.tex#L583) |
| 7 | Elementary wedge evaluation matrix rows covectors/columns vectors; row/column laws and numerical two-wedge evaluation | locally corrected | 13.6; [ch13-forms-stokes.tex:598](chapters/ch13-forms-stokes.tex#L598) |
| 7 | Basis before multiplication; arbitrary coefficients recovered by increasing tuple; 3D basis/flux sign conversion | newly implemented | 13.6; [ch13-forms-stokes.tex:639](chapters/ch13-forms-stokes.tex#L639) |
| 7 | Three-term 1-by-2 example, internally ordered shuffle blocks, alternation/bilinearity and concatenation proof | already present and retained | 13.6; [ch13-forms-stokes.tex:652](chapters/ch13-forms-stokes.tex#L652) |
| 7 | Associativity through three ordered blocks and graded commutativity via pq swaps; optional full-permutation formula justified | already present and retained | 13.6; [ch13-forms-stokes.tex:707](chapters/ch13-forms-stokes.tex#L707) |
| 7 | Elementary wedges span but need not exhaust; 4D real non-elementarity square retained | already present and retained | 13.6; [ch13-forms-stokes.tex:724](chapters/ch13-forms-stokes.tex#L724) |
| 7 | Exterior algebra only after product; unit, finite components, homogeneous/mixed and degree-grouped example | newly implemented | 13.6; [ch13-forms-stokes.tex:745](chapters/ch13-forms-stokes.tex#L745) |
| 7 | Fixed covector to varying form, omega/omega_p/evaluation; form degree versus polynomial; superscripts are indices | locally corrected | 13.7; [ch13-forms-stokes.tex:793](chapters/ch13-forms-stokes.tex#L793) |
| 8 | Four scalar classical outputs comparison, distinguished from componentwise vector integration | newly implemented | 13.4; [ch13-forms-stokes.tex:423](chapters/ch13-forms-stokes.tex#L423) |
| 8 | Field continuity assumed before parameter integrand continuity for curves and surfaces | locally corrected | 13.1.1; [ch13-forms-stokes.tex:50](chapters/ch13-forms-stokes.tex#L50) |
| 8 | P dx+Q dy before Green; orientation reversal, reparametrization/path independence, multiplicity | already present and retained | 13.2; [ch13-forms-stokes.tex:159](chapters/ch13-forms-stokes.tex#L159) |
| 8 | Surface derivative 3x2, cross-product area, normal cancellation, expanded change determinant | already present and retained | 13.3.1; [ch13-forms-stokes.tex:292](chapters/ch13-forms-stokes.tex#L292) |
| 8 | First Stokes boundary explicitly Phi(partial D), not ambient boundary; corners retained | locally corrected | 13.4; [ch13-forms-stokes.tex:440](chapters/ch13-forms-stokes.tex#L440) |
| 8 | Pullbacks by evaluation; arbitrary smooth-map pullback versus admissible integral invariance | already present and retained | 13.7; [ch13-forms-stokes.tex:763](chapters/ch13-forms-stokes.tex#L763) |
| 8 | D2 f versus d(df), workflow, scalar form coefficient, graph versus unsigned area | already present and retained | 13.7.2; [ch13-forms-stokes.tex:1137](chapters/ch13-forms-stokes.tex#L1137) |
| 8 | Parametrized form integration consistently uses k and N | locally corrected | 13.8; [ch13-forms-stokes.tex:1323](chapters/ch13-forms-stokes.tex#L1323) |
| 8 | Half-space top-form integral beside open integral before overlap proposition; later boundary chart only applies it | locally corrected | 13.8; [ch13-forms-stokes.tex:1231](chapters/ch13-forms-stokes.tex#L1231) |
| 8 | Practical boundary box after chart invariance; interval/ray/ball examples and full tangent versus constrained curves | newly implemented | 13.9.1; [ch13-forms-stokes.tex:1553](chapters/ch13-forms-stokes.tex#L1553) |
| 8 | Tangent equivalence classes, vector operations, intrinsic differential, coordinate/dual bases preserved | already present and retained | 13.9.2; [ch13-forms-stokes.tex:1606](chapters/ch13-forms-stokes.tex#L1606) |
| 8 | Graph differential evaluation at (a,b), linear image versus affine tangent plane | locally corrected | 13.9.3; [ch13-forms-stokes.tex:1797](chapters/ch13-forms-stokes.tex#L1797) |
| 8 | Smooth-localization motivation and neighborhood local finiteness; optional accumulating-bumps example omitted to avoid redundant illustration; required neighborhood definition and localization motivation are retained | intentionally not adopted | 13.9; [ch13-forms-stokes.tex:1444](chapters/ch13-forms-stokes.tex#L1444) |
| 8 | Scalar coefficient before global integral; full common-refinement proof and two-chart circle computation | already present and retained | 13.10; [ch13-forms-stokes.tex:2267](chapters/ch13-forms-stokes.tex#L2267) |
| 8 | Stokes degree guide, work/flux degrees, local dtheta versus no global potential | already present and retained | 13.12; [ch13-forms-stokes.tex:2593](chapters/ch13-forms-stokes.tex#L2593) |
| 9.1 | First-order extremum theorem before boundary invariance | already present and retained | 11.2; [ch11-multivariable-differentiation.tex:703](chapters/ch11-multivariable-differentiation.tex#L703) |
| 9.2 | Half-space derivative independence and chain rule, inverse derivatives without boundary-preservation assumption | already present and retained | 12.5; [ch12-multivariable-integration.tex:1904](chapters/ch12-multivariable-integration.tex#L1904) |
| 9.3 | Interior open, boundary closed, inherited topology, smooth inclusion, positive transverse block | already present and retained | 13.9.1; [ch13-forms-stokes.tex:1566](chapters/ch13-forms-stokes.tex#L1566) |
| 9.4 | Tangent and intrinsic differential before manifold-form operations | already present and retained | 13.9.3; [ch13-forms-stokes.tex:1737](chapters/ch13-forms-stokes.tex#L1737) |
| 9.5 | Continuous-form convention and C1 pullback retained; smooth Stokes hypotheses unchanged | already present and retained | 13.7; [ch13-forms-stokes.tex:845](chapters/ch13-forms-stokes.tex#L845) |
| 9.6 | Signed finite-set convention first; discrete compact support justified after manifold definitions | locally corrected | 13.8; [ch13-forms-stokes.tex:1174](chapters/ch13-forms-stokes.tex#L1174) |
| 9.7 | Support of d omega, boundary pullback and existence of both integrands; arbitrary pullbacks need not preserve compact support | already present and retained | 13.9.4; [ch13-forms-stokes.tex:1952](chapters/ch13-forms-stokes.tex#L1952) |
| 9.8 | External refinement theorem and local finiteness before partition proof; compact cutoff follows | already present and retained | 13.9; [ch13-forms-stokes.tex:1451](chapters/ch13-forms-stokes.tex#L1451) |
| 9.9 | Compact boundary support admits one ambient extension; zero only across artificial edges | already present and retained | 13.10; [ch13-forms-stokes.tex:2187](chapters/ch13-forms-stokes.tex#L2187) |
| 9.10 | Euclidean COV before overlap integrals; manifold/Jordan comparison before classical recoveries, not using Stokes to define integrals | already present and retained | 13.10.1; [ch13-forms-stokes.tex:2351](chapters/ch13-forms-stokes.tex#L2351) |
| 9.11 | Global surface Stokes applies ambient work form via inclusion, identifying both pullbacks | already present and retained | 13.12; [ch13-forms-stokes.tex:2675](chapters/ch13-forms-stokes.tex#L2675) |
| 10 | Integer coefficients versus laws; concrete F2 before Fp, Bezout background for field assertion | newly implemented | A.1; [app-determinants.tex:40](chapters/app-determinants.tex#L40) |
| 10 | Minus 30 in characteristics 2,3,5,7 and invertibility only after interpretation | newly implemented | A.3; [app-determinants.tex:333](chapters/app-determinants.tex#L333) |
| 10 | Additional order/norm/topology structure, positive-characteristic order obstruction, characteristic zero not positivity; Hermitian self-value real | already present and retained | A.1; [app-determinants.tex:22](chapters/app-determinants.tex#L22) |
| 10 | Q2 positive dot product, sqrt not necessarily rational, real-valued norm after embedding versus F2 | newly implemented | A.1; [app-determinants.tex:63](chapters/app-determinants.tex#L63) |
| 10 | Bijections, cycles, transpositions, parity before inversions retained | already present and retained | A.2; [app-determinants.tex:81](chapters/app-determinants.tex#L81) |
| 10 | Third-index pairs integrated into Vandermonde proof; explicit nonzero integer evaluation; parity separate from field signs | locally corrected | A.2.3; [app-determinants.tex:203](chapters/app-determinants.tex#L203) |
| 10 | Laplace remaining row/column lists, residual permutation sigma(c_s)=r_pi(s) and cofactor sign | newly implemented | A.3; [app-determinants.tex:322](chapters/app-determinants.tex#L322) |
| 10 | Normalized form rescales by det(P)^-1; fixed endomorphism conjugates; distinct spaces need choices | newly implemented | A.3; [app-determinants.tex:338](chapters/app-determinants.tex#L338) |
| 10 | Preserve Chapter 10 expansion, indices, cofactors, elimination, orientation; only retrospective cross-reference added | locally corrected | 10.17; [ch10-topology-linear-algebra.tex:2189](chapters/ch10-topology-linear-algebra.tex#L2189) |
| 10 | Exercise A.1 different from repeated worked permutation | locally corrected | A.3; [app-determinants.tex:355](chapters/app-determinants.tex#L355) |
| 11 | Required order A-J realized as B.1-B.13; binary unit/symmetry/associativity/distributivity before named maps and finite products | locally corrected | B.5; [app-tensors.tex:444](chapters/app-tensors.tex#L444) |
| 11 | Detailed binary-only associativity before direct products; no Tensor-Hom dependency | locally corrected | B.5.3; [app-tensors.tex:496](chapters/app-tensors.tex#L496) |
| 11 | Symmetry interchanges distinct basis tensors, not literal commutativity | newly implemented | B.5.2; [app-tensors.tex:490](chapters/app-tensors.tex#L490) |
| 11 | Binary/finite distributivity maps and four-component forward/reverse calculation retained before finite abstraction | already present and retained | B.5.4; [app-tensors.tex:635](chapters/app-tensors.tex#L635) |
| 12 | Quotient basis by extension, separate spanning/independence, dimension and chosen-complement inverse/composites | newly implemented | B.1; [app-tensors.tex:144](chapters/app-tensors.tex#L144) |
| 12 | Algebraic finite support, label/symbol/coefficient/sum distinctions; huge formal space versus F tensor F | newly implemented | B.3.1; [app-tensors.tex:274](chapters/app-tensors.tex#L274) |
| 12 | Full formal-basis extension, four relations, quotient descent/uniqueness, universality forces spanning not surjectivity | already present and retained | B.3.1; [app-tensors.tex:293](chapters/app-tensors.tex#L293) |
| 12 | Zero/scalar tensor identities before examples and finite nonzero elementary-tensor criterion | newly implemented | B.3.1; [app-tensors.tex:335](chapters/app-tensors.tex#L335) |
| 12 | Coefficient table not canonical V-to-W map; V* evaluation and row i column j matrix unit; explicit inverse basis-independent | locally corrected | B.8.2; [app-tensors.tex:1008](chapters/app-tensors.tex#L1008) |
| 13 | Named binary induced maps with bilinear input, identity/composition/inverse laws | locally corrected | B.6; [app-tensors.tex:675](chapters/app-tensors.tex#L675) |
| 13 | Direct finite universal property, formal symbols, slot checks, basis detectors and three-factor example retained | already present and retained | B.7; [app-tensors.tex:716](chapters/app-tensors.tex#L716) |
| 13 | Three-factor forward/reverse and both composites preserved after direct construction | locally corrected | B.7; [app-tensors.tex:826](chapters/app-tensors.tex#L826) |
| 13 | Every finite parenthesization theorem; block induction, map-valued multilinearity, evaluation last, canonical inverses and route independence | newly implemented | B.7; [app-tensors.tex:849](chapters/app-tensors.tex#L849) |
| 13 | One-factor and zero-factor conventions; induced finite maps/tensor powers after comparisons; direct/iterated compatibility | locally corrected | B.7.1; [app-tensors.tex:924](chapters/app-tensors.tex#L924) |
| 14 | Alternating universal problem before quotient; concrete two-input case then general construction | newly implemented | B.9.1; [app-tensors.tex:1018](chapters/app-tensors.tex#L1018) |
| 14 | All repeated vectors essential, F2 coefficient counterexample, three-vector R2 basis and one-dimensional quotient in characteristic two | newly implemented | B.9.1; [app-tensors.tex:1035](chapters/app-tensors.tex#L1035) |
| 14 | Full tensor stage, relation check, quotient stage, two uniqueness clauses and diagrams retained | already present and retained | B.9.1; [app-tensors.tex:1112](chapters/app-tensors.tex#L1112) |
| 14 | Explicit elementary wedge calculus, sign from repeated input without division by two, permutations | newly implemented | B.9.1; [app-tensors.tex:1127](chapters/app-tensors.tex#L1127) |
| 14 | Full F3 expansion, remove/sort/collect, determinant basis detectors, zero/above-dimension conventions | already present and retained | B.9.2; [app-tensors.tex:1142](chapters/app-tensors.tex#L1142) |
| 14 | Elementary-wedge nonzero iff independent, dependence expansion and basis extension; not arbitrary sums | newly implemented | B.9.2; [app-tensors.tex:1192](chapters/app-tensors.tex#L1192) |
| 14 | Characteristic-independent F4 coefficient obstruction and unique coordinates/nonunique presentations retained; real square only later illustration | already present and retained | B.9.3; [app-tensors.tex:1207](chapters/app-tensors.tex#L1207) |
| 15 | Named exterior maps from alternating input, identities/composition/inverse/degree zero and quotient square | locally corrected | B.10; [app-tensors.tex:1228](chapters/app-tensors.tex#L1228) |
| 15 | Minors theorem via detectors including rectangular matrix, example and k=1; move existing Lambda2 matrix example here | newly implemented | B.10; [app-tensors.tex:1264](chapters/app-tensors.tex#L1264) |
| 15 | Named fourth determinant characterization before multiplication, scalar uniqueness/rescaling, singular and n=0 cases | newly implemented | B.10; [app-tensors.tex:1296](chapters/app-tensors.tex#L1296) |
| 15 | Four established determinant viewpoints, not invented numbered axioms; retrospective multiplicativity and no circular foundation | newly implemented | B.10; [app-tensors.tex:1315](chapters/app-tensors.tex#L1315) |
| 15 | Distinct top source/target lines do not canonically give a scalar | newly implemented | B.10; [app-tensors.tex:1325](chapters/app-tensors.tex#L1325) |
| 15 | After duality top covector pullback, normalization versus real orientation, no ordered claim over arbitrary F | locally corrected | B.13.2; [app-tensors.tex:1586](chapters/app-tensors.tex#L1586) |
| 16 | Exterior multiplication after calculations/maps/determinant, full fixed-list/map-valued/two-stage proof retained | already present and retained | B.11; [app-tensors.tex:1328](chapters/app-tensors.tex#L1328) |
| 16 | Degree zero, spanning-tuples lemma, uniqueness, associativity and graded commutativity retained | already present and retained | B.11; [app-tensors.tex:1335](chapters/app-tensors.tex#L1335) |
| 16 | Finite-dimensional exterior algebra components, homogeneous/mixed/unit/above dimension; explicit mixed-degree example | newly implemented | B.12; [app-tensors.tex:1450](chapters/app-tensors.tex#L1450) |
| 16 | Assembled Lambda T only after product, unit/product proof; fixed degree linear versus graded algebra homomorphism | newly implemented | B.12; [app-tensors.tex:1460](chapters/app-tensors.tex#L1460) |
| 16 | Both duality identifications and explicit inverses retained; Alt0 at first use | locally corrected | B.13.1; [app-tensors.tex:1493](chapters/app-tensors.tex#L1493) |
| 16 | Map compatibility pairing identity proved on elementary wedges then spanning; push/pull scalar explanation | newly implemented | B.13.2; [app-tensors.tex:1570](chapters/app-tensors.tex#L1570) |
| 16 | Abstract multiplication identified with Chapter 13 shuffle multiplication by determinant calculation | already present and retained | B.13.2; [app-tensors.tex:1596](chapters/app-tensors.tex#L1596) |
| 16 | Bivector terminology, bilinear map B in Tensor-Hom, B.9 coefficient 2/dependence in char 2; new comparisons/complements/minors/mixed exercises | locally corrected | B.13.2; [app-tensors.tex:1683](chapters/app-tensors.tex#L1683) |
| 17 | Preserve expanded Chapter 10 topology/direct sums/matrices/basis changes/inner products/norms/duals/determinant | already present and retained | Chapter 10 opening; [ch10-topology-linear-algebra.tex:1](chapters/ch10-topology-linear-algebra.tex#L1) |
| 17 | Preserve analytic chain/mixed partial/Neumann/inverse/implicit proofs, linear/nonlinear COV, compact Jordan comparison | already present and retained | 11.1; [ch11-multivariable-differentiation.tex:142](chapters/ch11-multivariable-differentiation.tex#L142) |
| 17 | Preserve intrinsic tangent/differential/exterior derivative, partition construction, boundary extension, global integral and Stokes proofs | already present and retained | 13.11; [ch13-forms-stokes.tex:2445](chapters/ch13-forms-stokes.tex#L2445) |

## Preservation and validation

All edits were applied to the current working tree. Chapter 5 and Chapter 8 were not
edited in this pass; Chapters 6 and 9 received only the requested notation explanations.
Chapter 10 received only the determinant cross-reference. Existing proofs in Chapters
11–13 were retained except the explicitly corrected local arguments and duplicated prose.
Appendix B's binary associativity, distributivity/four-component example, formal-symbol
proofs, three-factor comparison, tensor–map inverse, exterior basis/coefficient obstruction,
two-stage product, duality inverses and shuffle compatibility remain in full.

### Actual build results

Compilation was performed with MiKTeX `latexmk -pdf main.tex`, using
`-interaction=nonstopmode -halt-on-error -synctex=1` during revision builds.
The final build succeeded (exit 0), producing **295 PDF pages**. Latexmk reports
all targets up to date after its reruns; references, contents, numbering, and
bibliography stabilized. The final `main.log` contains no LaTeX warnings,
undefined references, or overfull/underfull boxes. The Windows launcher emitted
a Perl locale fallback warning; this did not affect compilation.
Build transcripts are `tmp/revision-330-build.txt` and
`tmp/revision-330-final-build.txt`.

### Completed visual review

Compared changed source lines against the pre-edit snapshots and used SyncTeX
to locate rendered pages, including neighboring lines. Rendered and inspected
81 selected pages, with **all of Appendices A and B**, title/contents, the
Chapter 12 introduction and integration repairs, and the Chapter 13 transition,
exterior algebra, and boundary material. Reviewed all 21 contact sheets at
original image resolution; individual page PNGs remain available.

The last wording/layout corrections affected only PDF pages 189, 231, 238, 239,
as verified by comparing decoded PDF page content streams before and after the
final rebuild. All four were rerendered and inspected. Also inspected page 230
(shuffle products) and bibliography pages 294–295: **84 distinct pages reviewed**
in total. No clipped equations, overlapping content, malformed diagrams, or
inappropriate heading breaks were found. Closure bars, hats, signs, and
superscript/subscript placement were checked in the rendered images.

Initial page manifest and 21 reviewed sheets:
`tmp/revision-330-visual/page-manifest.json` and `sheet-01.jpg`–`sheet-21.jpg`.
Final affected-page manifest and two reviewed sheets:
`tmp/revision-330-final-visual/pages.json` and `sheet-1.jpg`–`sheet-2.jpg`.
Final notation refinements explicitly restore boundedness in Chapter 12's first
infimum/supremum discussion, name the types in Chapter 13's mixed-degree example,
and keep the parametrized-integral definition together more naturally.

The 140 coverage entries above record implemented, retained, corrected, and
explicitly optional material. No Git tag or GitHub release was created.

</details>

<a id="historical-focused-dependency-audit"></a>
<details>
<summary>FOCUSED DEPENDENCY AUDIT</summary>

# Focused dependency and exposition audit — Version 3.1.0

Date: September 12, 2026. Baseline: Version 3.0.0 revision draft.

This pass completes remaining construction interfaces and improves selected examples and exercises. It preserves the manuscript's architecture and scope. The resulting PDF has 270 pages, compared with 265 in the baseline. README, ERRATA, OUTLINE, and the displayed version have been updated. No release, tag, commit, or push was made during this pass.

## Request-by-request implementation

Page numbers below are physical PDF page numbers; the main-text printed page number is seven less. Source labels are stable navigation points even if pagination changes later.

| Request | Implementation and location |
| --- | --- |
| I.A.1: local smooth-map definition | `chapters/ch13-forms-stokes.tex`, `def:smooth-manifold-map`, PDF p. 225. Requires charts with the source neighborhood mapped into the target neighborhood, displays the coordinate representative's domain, treats boundary charts by smooth extensions, derives continuity, and checks other charts on explicitly restricted overlaps. |
| I.A.2: intrinsic manifold operations | Same file, subsection 13.9.4, `sec:manifold-form-operations`, pp. 228–229. Defines the typed intrinsic pullback using the previously constructed differential, verifies its chart expression and smoothness, and defines wedge products pointwise. `prop:manifold-exterior-derivative` constructs local candidates and proves that they glue using the transition-pullback identity and Euclidean commutation with exterior differentiation. Boundary extension independence and the intrinsic calculus rules are included. This precedes manifold integration. |
| I.A.3: degrees above dimension | Euclidean and manifold forms definitions explicitly set the corresponding spaces to zero above the dimension. Degree zero and the pointwise vector-space operations are also specified. |
| I.B.1: closed-grid face bookkeeping | `chapters/ch12-multivariable-integration.tex`, linear change-of-variables proof, pp. 192–193. Closed indicator sums are distinguished from interior-defined step functions. Lower and upper functions have cell infima/suprema on interiors and values minus/plus a global bound on the finite union of faces. Pointwise inequalities now hold there too. The existing null-modification theorem justifies unchanged integrals before and after the linear map. |
| I.B.2: discarded strips | Same file, nonlinear change-of-variables proof, p. 199. Replaces the incorrect closure equality by coverage of the rectangle and intersection contained in finitely many coordinate faces. Zero-width strips remain harmless null sets. The subsequent volume estimates and separated error terms are retained. |
| I.B.3: Jordan set algebra | Same file, `prop:jordan-set-algebra`, p. 186. Proves measurability of unions, intersections, and differences using boundary containment in the union of the original boundaries; cited at later retained-set differences. |
| I.C.1: closed sequence tails | Inspected the actual Chapter 10 source. The nested sets already use closures of sequence tails. The compactness proof and its subsequent use of those closed sets are consistent; no mathematical change was necessary. |
| I.C.2: compact derivative maximum | Inspected `lem:local-volume-comparison` in the Chapter 12 source. Its derivative maximum already runs over the closure of the ball. The lemma's statement and proof are unchanged. |
| II.A: matrix-example progression | `chapters/ch10-topology-linear-algebra.tex`, matrix sections, pp. 140–144. Retains one basis-image example, replaces the next repetition with reconstruction in a nonstandard target basis, and makes the entrywise-multiplication warning a short callback using the second basis vector. |
| II.B: matrix vector-space operations | Same file, p. 144. Defines addition and scalar multiplication entrywise, then derives the matrix formula for a linear combination by evaluating basis images before identifying the space of linear maps with a matrix space. |
| II.C: positive internal direct sum | Same file, `ex:positive-direct-sum`, p. 137. Works through the plane and complementary line, membership, existence, uniqueness, component maps, external summation map, its inverse, and both composites. Explains that uniqueness is the defining issue and that the example is not orthogonal. |
| II.D: genuinely different operator norms | Same file, p. 147. For T(x,y)=(x+2y,0), proves infinity operator norm 3 and sum operator norm 2, with upper bounds and attaining unit vectors. Retains the warning that a bound alone does not establish equality. |
| III.A: four-component tensor example | `chapters/app-tensors.tex`, `ex:four-tensor-components`, pp. 255–256. Applies the already constructed finite distributivity isomorphism, sends an elementary tensor forward, sends a nontrivial component tuple backward, checks composites explicitly, and only then checks dimensions. |
| III.B: three-factor factorization | Same file, `ex:three-factor-functional`, pp. 257–258. Uses factors of dimensions 2, 2, and 3; displays separate linearity in each slot, specifies the induced functional and its basis values, identifies the three nonzero basis values, and evaluates a sum proved to be non-elementary. |
| III.C: exterior/shuffle compatibility | Same file, `prop:abstract-shuffle-compatibility`, p. 267. Compares the already constructed bilinear products, checks elementary covector wedges using the determinant expansion by shuffles, and extends by spanning. Includes scalar degrees and explains the identification of the two exterior algebras over the reals. |
| IV.A: surface introduction | Chapter 13, `prop:cross-product-identities`, p. 210. Separates the cross-product definition, proved identities and consequences, and regular surface-patch definition. Explains orthogonal as zero Euclidean dot product. Chapter 12 uses a coordinate reflection instead of an undefined general orthogonal map. |
| IV.B: general-dimensional flux | Chapter 13, `def:general-flux`, pp. 236–237. Defines the signed omitted-coordinate flux form and boundary-flux notation before the n-dimensional divergence theorem. Checks agreement with the three-dimensional cross-product formula and the one-dimensional endpoint convention. |
| V: convergence consistency | Chapter 12's remark following the uniform theorem distinguishes limit integrability supplied by uniform convergence from the separately assumed integrable limit in Chapter 9's one-dimensional Arzela theorem. The final broad perspective sentence was located in Chapter 13 and corrected there as well. Lebesgue comparisons remain; no multivariable Arzela theorem is claimed. |
| VI: focused exercise audit | Chapter 10 adds a parameter-dependent complementary-line problem and nonstandard-basis matrix operations; revises repeated kernel/rank and inverse exercises. Appendix B adds quotient factorization with an inverse and failed-kernel condition, reverse distributivity with a non-elementary block, and the three-factor functional's kernel. Chapter 13 uses real circle coordinates and adds pullback/exterior-derivative exercises, including a two-form pulled back to a curve. Other exercises remain. |
| VII.1: explicit references | `chapters/ch08-differentiation.tex` now labels the elementary-series convergence proposition and cites it explicitly for elementary-function derivatives; tangent positivity cites the pi-construction theorem explicitly. Inserted results use labels and resolved references. |
| VII.2: attribution | `chapters/references.tex` acknowledges the determinant pattern, permutation exposition, and Appendix B proof architecture separately. `chapters/app-determinants.tex` has a matching local permutation attribution. The note does not attribute the entire manuscript to the algebra notes. |
| VII.3: trigonometric-series claim | Preserved the continuity/uniform-convergence conclusion and the warning about a failed derivative majorant; no nowhere-differentiability claim was introduced. |
| VII.4: Chapter 13 title | Full chapter heading, contents entry, and PDF bookmark use Differential Forms, Stokes' Theorem, and Calculus on Manifolds. The shorter running header remains intentional. |

## Scope and smaller alternatives

- Used the requested preferred interior-plus-null-faces convention rather than changing the linear change-of-variables strategy.
- Retained degenerate remainder rectangles and stated the exact coverage/intersection properties needed, rather than redesigning the grid.
- Verified the two sensitive overlines directly in LaTeX and left the correct proofs unchanged.
- Replaced the early orthogonal-map example with a coordinate reflection; no orthogonality theory was added.
- Applied the convergence perspective correction where the sentence actually occurs, in Chapter 13, as well as updating Chapter 12's convergence remark.
- Added applications of existing tensor constructions and a short product comparison, without extending the abstract theory's scope. Terminology remains elementary tensors and elementary wedges.

## Proof and dependency preservation

The working baseline is saved under `tmp/pre-focused-3.1.0/`. Source comparisons and focused mathematical checks are recorded under `tmp/focused-31-qa/`.

Entire Chapters 3, 9, and 11 are byte-for-byte unchanged from that baseline. This preserves the uniqueness-first real-number construction, the strengthened differentiation-under-limits and Arzela proofs, and the inverse/implicit-function proofs.

Automated source comparisons also confirm unchanged statements and proofs for metric compactness, local volume comparison, tangent transitions and tangent vector-space structure, the manifold differential, quotient factorization, first isomorphism, tensor uniqueness and existence, the scalar tensor isomorphism, currying, the exterior universal property, and exterior duality. Additional comparisons preserve the full slot-by-slot determinant construction and its explanatory remark, the two-stage exterior-multiplication section, and the termwise-differentiation proof.

Review of the focused source diffs confirms retention of the distinct compactness arguments, nonlinear change-of-variables architecture, chart-sign orientation treatment, two-chart circle integral, and constructed forward/reverse canonical maps. New manifold operations depend on already constructed tangent maps and already proved Euclidean identities. New tensor examples invoke existing maps before comparing their values.

Exact calculations check the direct-sum inverse, nonstandard-basis matrix reconstruction, operator-norm maximizers, distributivity forward/reverse component calculations, all twelve values of the trilinear functional, and the coefficient-minor obstruction to its example tensor being elementary. Twenty finite determinant/shuffle checks cover dimensions 1 through 5, including degree-zero cases. These checks supplement the written proofs; they are not formal proof verification.

## Compilation, references, and visual verification

- Compiled with `latexmk -pdf -interaction=nonstopmode -halt-on-error main.tex`; latexmk completed its reruns and reported all targets up to date. The final build log is `tmp/focused-31-build2.txt`.
- Final output: 270 pages. Final LaTeX log has no warnings, undefined references, overfull boxes, or underfull boxes. `git diff --check` passes.
- Active-source audit: 19 files, 320 unique labels, 336 resolved reference occurrences. Newly inserted theorem numbers and their forward/backward uses were checked against the stable build.
- Rendered all 270 pages. Reviewed contact sheets 12–14 and 16–23 for reflow, diagrams, contents, and surrounding material.
- Inspected full-size pages 5, 137, 141, 144, 147, 186, 192–193, 199, 210, 225, 228–229, 236–237, 255–258, and 267. These include every specifically requested visual-review area. No clipping, malformed diagrams, or layout defects caused by this pass were found.
- Checked the PDF cover version and full Chapter 13 bookmark programmatically; the contents and chapter heading also render correctly.

Final PDF SHA-256: `9a2c8afe2cb36000c9f2735e144bac4e4993b6e7b876dcfdc7348bc2ff7dd3d1`.

Machine-readable evidence: `source-check.json`, `proof-and-exact-checks.json`, `additional-preservation.json`, `render-manifest.json`, and `final-artifact-check.json` in `tmp/focused-31-qa/`. Authoring and verification scripts remain in `tmp/` for traceability. Existing backup copies and earlier audit documents were preserved.

</details>

<a id="historical-focused-revision-audit"></a>
<details>
<summary>FOCUSED REVISION AUDIT</summary>

# Focused pedagogical and structural revision

Revision date: September 11, 2026. This pass edits the existing local draft;
it does not reset the pre-existing working-tree changes or edit the copied
backup sources. Version remains 1.3.0 (revision draft).

## Scope and requirement map

| Requested area | Implementation |
| --- | --- |
| Chapter 5 limit points | Domain membership versus accumulation; missing endpoints; isolated points; sequential limit-point criterion; why the punctured limit otherwise loses uniqueness. |
| Chapter 5 continuity | Domain-point requirement, included versus excluded input, explicit self-comparison at isolated points, and the precise limit/continuity equivalence at accumulation points. One-sided limits now state the appropriate one-sided accumulation hypothesis. |
| Chapter 5 asymptotics | Regime dependence, bounded/vanishing coefficient translations, epsilon estimates, absolute versus relative smallness, failure of both converse first-order implications, sum/product/comparison calculus, asymptotic equivalence, and derivative remainder preview. Focused exercises added. |
| Chapter 10 structure | Seven numbered sections in the requested order: metric/topological spaces; products/compactness/connectedness; linear foundations; norms; duality/multilinearity; determinants/orientation; perspective/transition. |
| Topology dependencies | Euclidean dot product and norm; metric accumulation, boundedness, diameter, convergence, Cauchy sequences, completeness; topological continuity defined first; metric equivalence proved; rectangles define finite product topology; max-metric compatibility and coordinate continuity established. |
| Compactness | Separate finite-net and cover-radius mechanisms; compact iff sequentially compact; arbitrary-cover Lebesgue-number consequence without repeating the contradiction proof; compact extreme values used in norm proofs. |
| Connectedness | Convexity defined; interval connectedness argument expanded; explicit constant-sign corollary. |
| Linear foundations | Subspaces, combinations, span, independence, basis reduction, replacement/exchange, dimension, basis extension, coordinates, linear maps, kernel/image, rank/nullity, rank–nullity, equal-dimension bijectivity. |
| Matrices | Basis images force the columns; linearity forces matrix-vector multiplication; composition forces matrix multiplication; matching dimensions, order, associativity, and failure of entrywise multiplication explained. |
| Coordinate changes | Identity-map transition matrices, inverse transitions, general domain/codomain transformation, endomorphism similarity identity, and complete 2-by-2 example. No similarity theory introduced. |
| Norms | Norm definition, reverse triangle, norm equivalence, completeness, linear continuity, compact unit-ball maximum for operator norm, submultiplicativity, diagonal worked example. |
| Duality and multilinearity | Linear-map space and its dimension, dual basis, covector evaluation/pullback, bilinear examples and product-space warning, basis-tuple determination and bounds, alternation from repeated inputs. |
| Norm-valued asymptotics | Sum, bounded-linear, composition, and bounded-bilinear estimates proved. The composed remainder requires r(0)=0 when intermediate increments can vanish; Chapter 11 explicitly uses this convention. |
| Determinants | Signed area motivation; normalized alternating-form existence/uniqueness; slot expansion and 27-to-six example; laws and multiplicativity from uniqueness; forced Leibniz formula; transpose and basis-independent operator determinant; minors, cofactors, both Laplace expansions; sparse 3-by-3 and 4-by-4 and elimination examples; orientation and elementary factorization retained. |
| Chapter 11 | Recalls the linear-map space and multilinearity; explains symmetric higher derivatives versus alternating forms; computes a bilinear second derivative and distinguishes its diagonal specialization. |
| Chapter 12 | Source unchanged in this pass. Its determinant, compactness, Lebesgue-number, and elementary-factorization references still resolve to the required proved results. |
| Chapter 13 | Recalls Chapter 10 prerequisites; exterior powers as alternating covectors; elementary wedges by determinants; early basis/dimension theorem; shuffle product before full-permutation normalization; product laws; non-elementary two-form example; direct sums defined locally. |
| Appendix A | Arbitrary-field distinctions and positive-characteristic counterexamples; cycles, transpositions, integer Vandermonde parity, sign, even/odd permutations, inversions, permutation matrices; determinant construction and pair cancellation in characteristic two; Laplace expansion and optional adjugate/Cramer exercise. |
| Appendix B | Universal tensor product, canonical uniqueness, formal-symbol quotient construction, tensor basis, non-elementary tensors, tensor powers, alternating quotients, exterior bases/products, induced maps and composition, duality, top exterior determinant, return to real volume forms. |
| Supporting files | Main inputs/appendices, automatic numbering/contents, bibliography and attribution, README, outline, errata, revision date, and prior-audit pointer updated. |

## Algebra notes and benchmarks

The active algebra source consulted was `../Algebra/chapters/modules.tex`.
Its compiled `main.aux` identifies label `thm:det-form` as Theorem 5.12.3,
“Existence and uniqueness of the determinant form.” The adaptation is
specifically its one-slot-at-a-time coordinate expansion, coefficient
bookkeeping, repeated-index cancellation, and explanation that the remaining
tuples are precisely permutations. It appears in the main determinant
theorem and its dimension-three example, with attribution in the manuscript
and bibliography. No algebra files were modified.

The [Pearson contents and description](https://www.pearson.com/en-us/subject-catalog/p/linear-algebra/P200000006185/9780134876979)
confirm the requested Friedberg–Insel–Spence vector-space / linear-map /
matrix organization. [Wiley's Apostol listing](https://www.wiley-vch.de/en/areas-interest/mathematics-statistics/mathematics-16ma/calculus-16ma3/calculus-volume-2-978-0-471-00007-5)
was used for bibliographic verification. These checks do not claim full-text
consultation of those books. Their requested pedagogical roles are reflected
in the organization; the explicit proof adaptation is from the available
algebra notes. Munkres remains a further-reading benchmark in the bibliography.

## Dependency and mathematical audit

- Metric convergence and accumulation are defined before sequential closure
  and map limits. Topological continuity is defined rather than described
  as a characterization of an undefined notion.
- The metric compactness equivalence uses the separately proved net/cover
  lemma. Lebesgue numbers then follow without a second copy of its proof.
  The nonempty-space hypothesis excludes the empty-cover edge case.
- Exchange precedes dimension, extensions precede rank–nullity, and all
  matrix rules follow basis coordinates. Coordinate changes precede
  orientation and the intrinsic determinant of an endomorphism.
- Norm equivalence first proves Euclidean continuity by a coordinate bound,
  then applies compact extreme values. This avoids assuming continuity
  in the norm whose equivalence is being proved.
- Basic multilinear bounds and remainder-composition estimates precede
  Chapter 11's product and chain rules. Derivative remainders are zero at
  zero; the punctured little-o hypothesis alone does not supply that value.
- The main determinant existence argument contains its own elementary
  integer parity justification. Appendix A expands this construction but
  is not a hidden premise of the analysis. Multiplicativity precedes the
  invertibility criterion; transpose invariance precedes row cofactor laws.
- Chapter 12 still has the elementary row operations and their determinants
  needed for linear change of variables, and the generalized Lebesgue-number
  result implies its former finite-cover use.
- Chapter 13 builds its basis picture before the general wedge product;
  neither tensor products nor the quotient construction is required there.
  A general alternating covector need not be one elementary wedge.
- Over arbitrary fields, alternation means zero on repeated inputs. The
  existence proof uses paired cancellation, not division by two. Permutation
  parity is constructed over the integers before signs are interpreted in F.
  Tensor/exterior quotient and basis arguments use no positivity or factorial
  inverses. The non-elementary exterior example has a coefficient proof
  that remains valid in characteristic two.
- No eigenvalue, diagonalization, spectral, module, or category theory was
  added to the main text or required by either appendix.

## Validation

- Final PDF: 210 pages. pdfLaTeX compilation completed successfully; auxiliary files, contents,
  and bookmarks stabilized on repeated builds.
- The final log contains no undefined references, unresolved citations,
  duplicate labels, overfull boxes, or underfull boxes.
- Active-source checks cover 19 files, 267 unique labels, and 293 resolved
  reference occurrences, plus theorem/proof and display delimiters.
- Independent exact-arithmetic calculations verify the sparse determinants
  (-30 and -10), elimination example (7), and worked change-of-basis matrix.
- Visual checks include Chapter 5 limits/asymptotics, matrix construction and
  coordinate change, determinant expansion and cofactor computation, exterior
  basis/shuffle formula, appendix parity and tensor construction, and contents.
  The visual review prompted shortened appendix running headers and wider
  contents number columns for two-digit Chapter 13 section numbers.
- `git diff --check` passes; Git reports only line-ending normalization
  notices. Existing unrelated edits and copied files were preserved.
- This is a mathematical and editorial review, not a machine-checked proof.
  No commit, push, tag, release, or publication was performed.

Build logs, exact-arithmetic/source-check code, and representative page
renders are under the ignored `tmp/` directory and are not build dependencies.

</details>

<a id="historical-major-pedagogical-audit"></a>
<details>
<summary>MAJOR PEDAGOGICAL AUDIT</summary>

# Major pedagogical revision audit

Version 2.0.0 (revision draft), September 12, 2026.

This revision develops the existing course rather than adding a new syllabus.
The final PDF has 244 physical pages: cover, six numbered front-matter pages,
and 237 main/back-matter pages. Chapter 10 occupies printed pages 111–142;
Appendix A occupies 219–224 and Appendix B occupies 225–235. These are actual
lengths, not the illustrative page ranges in the revision request.

## Request-to-manuscript map

| Requested area | Revised treatment |
|---|---|
| Chapter 10 introduction and organization (1–2) | A substantial introduction connects scalar calculus to derivatives as linear maps, Jacobians, determinants, and integration. Twelve sections separate matrices, composition, and coordinate changes before inner products, norms, duality, and determinants. |
| Metrics and topology (3) | Concrete distances and neighborhoods precede abstraction; examples distinguish isolated points, incomplete spaces, and discrete metrics. Compactness retains separate finite-net, cover-radius, and finite-subcover mechanisms. A unit-sphere example connects compactness to optimization. |
| Vector spaces and linear maps (4–5) | Coordinate and polynomial examples, subspaces, span, independence, removal and exchange, basis extension, coordinates, kernels, images, and rank–nullity receive explicit intermediate reasoning and computations. |
| Matrices, composition, coordinates (6–8) | Images of basis vectors produce columns before the general formula. Row/column roles are explained; two composition calculations and multiple two- and three-dimensional basis changes accompany the commuting coordinate diagram. |
| Inner products, norms, operators (9–10) | Abstract real inner products include a polynomial-integral example; positivity, Cauchy–Schwarz, and the triangle inequality are proved. Norm geometry, coordinate bounds, continuity of linear maps, and operator-norm examples precede later differentiation. |
| Duality and multilinearity (11) | An explicit nonstandard dual basis, metric-dependent gradient discussion, coefficient expansions, and a bilinear continuity calculation distinguish vectors, coordinates, and covectors. |
| Determinants, computation, orientation (12–14) | Normalized alternating forms and slot-by-slot multilinear expansion remain the structural route. The exposition explains all n^n choices and why repeated indices vanish. Minimal sign facts refer to Appendix A. A complete six-row Leibniz table, sparse 3-by-3 and 4-by-4 cofactor examples, elimination, and orientation connect theory to calculation. |
| Appendix A (15) | Bijections, right-to-left composition, cycles, disjoint cycles, adjacent swaps, the parity problem, the sign proof, inversions, and permutation matrices are developed concretely without group-theory prerequisites. Arbitrary-field and characteristic-two distinctions are retained. |
| Appendix B tensors (16) | Bilinearity is motivated before universality. Diagrams, canonical inverse maps, a quotient-space example, formal symbols, relations, descent, coefficient detectors, and a tensor-basis table explain the construction. Constructing a map is distinguished from checking equality of existing maps. Symmetry, associativity, induced maps, and a small Tensor–Hom correspondence include their mechanisms. |
| Exterior powers and algebra (17–18) | A second-exterior-power example precedes the general construction. Tensor-stage factorization and alternating quotient descent are separated. Spanning and independence use different arguments. A full coefficient obstruction proves nondecomposability in every characteristic. Exterior multiplication is constructed through universal properties; graded signs, sums of degrees, duality, and top-degree determinants are explained. |
| Chapters 5 and asymptotics (19–20) | Function-limit laws precede their use; the square-root example has a direct estimate. The prior limit-point, continuity, and isolated-point work is preserved. Relative-scale explanations reinforce big-O/little-o and the zero-value condition. |
| Chapters 3–4 (21–22) | Supremum versus maximum, approximation from below, and the levels in the rational-Cauchy construction are explained. Decimal expansions are introduced as three separate tasks, with a 1/7 calculation. Limsup oscillation and a completeness-dependency diagram support the existing proofs. |
| Chapter 6 (23) | A low-degree Bernstein calculation, explicit first moment, near/far error budget, equicontinuity examples, diagonal-selection table, and three-term finite-test-point estimate make the main mechanisms visible. The equicontinuity limit proposition uses pointwise convergence. |
| Chapters 7–8 (24–25) | Dyadic and Cauchy-product diagrams, endpoint convergence, and the relocated alternating remainder support series. A sequence differentiation theorem precedes its series corollary. Both derivative-radius inequalities, a numerical Taylor estimate, rational-power compatibility, cutoff derivatives, and the convex tangent/chord picture are supplied. |
| Chapter 9 preparation (26) | A complete uniform-partition Darboux computation and tagged-cell crossing diagram explain the integral's approximation mechanism. |
| Arzelà bounded convergence (27) | The theorem assumes pointwise convergence, a common bound, and integrability of the limit. An internal interval-length/compact-core proof gives convergence of absolute error integrals and then of integrals. Finite rational indicators show why limit integrability is essential. Uniform Riemann interchange, Arzelà convergence, Dini, and Lebesgue domination are distinguished. |
| Remaining Chapter 9 (28) | A good/bad interval error budget supports the Lebesgue criterion. The two divergent sides of 1/x are distinguished from principal-value cancellation. Continuous FTC is a corollary of the stronger accumulation-function result. |
| Chapter 11 (29) | The differentiability hierarchy, coordinate staircase, higher-derivative types, rectangular mixed-partial argument, second-order Taylor–Peano estimate, compact-sphere positivity, contraction hypotheses/errors, Neumann partial sums, implicit examples, and Lagrange kernel argument are expanded. |
| Chapter 12 (30–31) | Fubini and early polar geometry motivate the formalism. The rectangle example's domain is corrected. Open covers, compact margins, and a fine-grid lemma repair boundary and zero-extension estimates, including null supports. Triangle/split-region calculations and a Lipschitz box/face lemma support the change-of-variables route. The existing small-cube closure compactness is verified. |
| Curves through patch Stokes (32–36) | Curve/velocity, length, scalar integral, and work are separated. Speed and reversal examples, Green boundary cancellation, tangent-parallelogram geometry, curved-paraboloid area and flux, and a parameter-boundary diagram support the classical theorems. |
| Forms and pullback (37–38) | A running form is tracked as a field, a point covector, and a scalar evaluation. A numerical shuffle example and a pullback workflow distinguish vector pushforward from form pullback. A two-form pulled onto a graph illustrates degree preservation without invertibility. |
| Charts and tangent spaces (39–40) | Concrete chart transitions precede separated definitions of chart, compatible atlas, smooth structure, and boundary. Moving-point velocities derive the transition rule; boundary tangent spaces retain the coordinate definition. |
| Orientation (41) | Orientation is intrinsic to tangent frames. Boundary charts record coordinate signs, with an oriented interval showing opposite endpoint chart signs. The integration definition, overlap argument, and Stokes localization carry those signs consistently. |
| Partitions and general Stokes (42–43) | A two-weight construction, support diagram, and artificial-versus-genuine boundary explanation support the retained partition proof and local-to-global argument. The refinement theorem remains explicitly external. |
| Exercises, bibliography, cleanups (44–46) | Exercises were added across the requested chapters and appendices. Bartle's second edition is included and annotated. Algebra-source sections are identified. Duplicated explanations, an unused proof parameter, stale lettered proof references, and a stale parity forward/backward reference were corrected. |
| Final pedagogy and scope (47–49) | Examples, proof strategies, object types, dependencies, and transitions were reviewed. The course still stops short of spectral theory, developed orthogonal-basis theory, measure theory, tensor categories, and a full differential-geometry syllabus. |

## Mathematical dependency checks

- The uniqueness-first real-number construction and the prior corrections to
  rational approximation and tail inequalities remain in place.
- The determinant proof uses finite multilinear expansion and the parity facts
  established in Appendix A; it does not presuppose exterior powers.
- Appendix B works over fields and explicitly avoids division by two in its
  arbitrary-characteristic nondecomposability argument.
- Arzelà's proof does not reuse the uniform-convergence argument. Its auxiliary
  open-interval length facts are proved before use, through compact finite
  interval covers and compact-core trimming; Lebesgue integration is not invoked.
- Chapter 12 separates finite Jordan covers from countable negligible covers.
  Boundary cells enter an open neighborhood using a positive compact margin.
- Boundary chart signs appear in both manifold integration and localization of
  Stokes. The interval example tests the zero-dimensional boundary convention.
- Chapter 13 still explicitly imports the manifold refinement theorem. The
  revision does not claim to have supplied an internal proof of that theorem.

## Sources consulted and attribution limits

The neighboring Algebra manuscript was consulted at the permutation discussion
in Section 1.5, the determinant development in Section 5.12, and the tensor
construction material in Chapter 8. The determinant discussion acknowledges
the adapted slot-by-slot proof in the manuscript itself.

Bartle's bibliographic details were checked against the
[publisher's second-edition listing](https://www.wiley-vch.de/en/areas-interest/mathematics-statistics/mathematics-16ma/calculus-16ma3/real-analysis-16ma34/the-elements-of-real-analysis-978-0-471-05464-1).
The complete Bartle text was not available for page-by-page comparison.
The pointwise bounded-convergence statement was independently checked against
[Nadish de Silva's elementary-proof paper](https://arxiv.org/pdf/1408.1439).
The manuscript supplies its own compact-core interval argument, rather than
claiming to reproduce Bartle's proof. Further-reading entries are not claims
that every cited book was consulted in full.

## Compilation and verification

The complete manuscript was compiled with installed MiKTeX pdfLaTeX, repeating
passes until the auxiliary, contents, and outline files stabilized. The final
log contains no undefined references, LaTeX warnings, overfull boxes, or
underfull boxes. No BibTeX/Biber step is needed.

The source checker covered 19 active LaTeX files, found 274 unique labels and
298 resolved reference occurrences, and checked paired display delimiters and
the principal theorem/proof/example/exercise environments. The label check is
a consistency check, not a formal verification of the mathematical arguments.

Independent exact-arithmetic checks covered four determinant examples, all six
Leibniz contributions, three basis changes, the graph pullback integral, the
paraboloid area and flux coefficients, the running covector evaluation, and
the complete polynomial cancellation in the exterior coefficient obstruction.
These checks use integers and rational arithmetic, not rounded numerical fits.

Every page was rendered and inspected at contact-sheet scale. Selected pages
were additionally inspected at page scale, including the Bernstein and diagonal
arguments, Arzelà's lemmas and proof, basis-change matrices, determinant table,
Jordan estimates, surface calculations, pullback diagram, interval orientation,
and tensor/exterior constructions. The final contents pages were inspected
individually, including numbering such as 10.10 and 13.10.

The visual pass corrected an almost empty final contents page and kept the
six-term determinant table with its introduction. After that rebuild, image
hashes matched the previously inspected renderings for every page except the
four contents pages, two front-matter pages, and three determinant pages.
Those changed pages were inspected individually. A final wording correction
replaced the stale phrase "parity argument above" with the Appendix A reference;
the PDF was rebuilt and rendered again. The final PDF has 244 pages.

Local validation artifacts are in `tmp/major-qa/`, with the final PDF SHA-256,
page count, and selected-page index in `render-manifest.json`. Exact-check
results are in `tmp/major-numerical-checks.txt` and label results in
`tmp/focused-source-check.txt`. These scratch artifacts are not build dependencies.

## Repository and documentation

README, OUTLINE, ERRATA, version/date macros, and this audit describe the current
revision. Earlier audits retain their historical dates and scope. The incoming
workspace already contained uncommitted revisions and backup copies; they were
preserved. A pre-edit source snapshot is in `tmp/pre-major-2026-09-12/`.
No commit, push, or publication was performed.

</details>

<a id="historical-part-i-audit"></a>
<details>
<summary>PART I AUDIT</summary>

# Part I Mathematical Audit

## Scope and method

This is an independent, theorem-by-theorem audit of Chapters 2--9, completed on 2026-08-21. For each definition, proposition, lemma, theorem, corollary, and substantial example, the audit checked stated hypotheses, conclusions, prior dependencies, endpoint cases, strict inequalities, inverse-function domains, completeness uses, and justification of limiting and series operations. The source was revised only where the audit found a concrete defect or proof gap.

Severity labels used here are:

- **CRITICAL:** a false theorem, circular argument, undefined object, or a gap that breaks later development.
- **MAJOR:** a substantial proof gap, missing hypothesis, dependency problem, or unjustified theorem-level claim.
- **MINOR:** a localized missing argument, imprecise statement, notation problem, or excessive proof compression.
- **EDITORIAL:** documentation, cross-reference, formatting, or stylistic matter.

## Findings and repairs

| Identifier | Location | Severity | Description and mathematical consequence | Repair made | Status |
|---|---|---|---|---|---|
| PI-01 | Chapter 3, ordered-field preliminaries | MAJOR | Absolute value was used in the basic-order-rules proposition before it was defined. This was a local dependency inversion at the foundation of the construction. | Moved the absolute-value definition before the proposition. | Resolved |
| PI-02 | Chapter 5, Intermediate Value Theorem | MAJOR | The supremum proof attempted to choose a point right of the supremum without excluding endpoint \(b\); its symmetric case likewise needed endpoint \(a\). | Added the endpoint exclusions and an explicit choice \(0<r<\min(\delta,b-c)\). | Resolved |
| PI-03 | Chapter 6, uniform products | CRITICAL | The assertion that a product of two uniformly convergent sequences is uniformly convergent when only \((f_n)\) is uniformly bounded is false. On \(\mathbb R\), \(f_n=1/n\) and \(g_n=g=x\) meet the former hypothesis but \(f_ng_n=x/n\) does not converge uniformly to \(0\). | Required both sequences to be uniformly bounded and supplied the correct product estimate. | Resolved |
| PI-04 | Chapter 7, deferred material | MINOR | “Power-Series Operations Deferred” was styled as a theorem despite containing only a forward-reference discussion. | Recast it as an unnumbered explanatory paragraph. | Resolved |
| PI-05 | Chapter 8, Taylor theorem | MINOR | The repeated-Rolle mechanism did not explicitly record all zeros at \(a\), leaving successive applications implicit. | Recorded \(H(a)=H'(a)=\cdots=H^{(n)}(a)=0\), the first zero of \(H'\), and the continuity/differentiability hypotheses at every stage. | Resolved |
| PI-06 | Chapter 8, exponential range | MAJOR | The positivity argument treated a square as automatically positive and compressed the tail and range arguments. | Used \(\exp(x/2)\exp(-x/2)=1\) to prove nonvanishing, then strict positivity; made both limiting tails and the IVT range argument explicit. | Resolved |
| PI-07 | Chapter 8, construction of \(\pi\) | CRITICAL | The proposed zero set for the least positive zero contained \(0\), so its infimum was \(0\). The later inverse-trigonometric construction therefore lacked a valid foundation. | Proved \(\cos 3<0\), obtained a zero-free interval \([0,\delta]\), took the infimum of the nonempty zero set in \([\delta,3]\), and proved its least-positive-zero property. The sequel proves signs, special values, periodicity, ranges, tangent limits, inverse domains, and derivative formulas. | Resolved |
| PI-08 | Chapter 9, basic integral properties | MAJOR | The Darboux proof of linearity stated key inequalities but did not show how they prove integrability and equality of integrals. | Added common-refinement estimates, the Darboux-gap argument, two-sided integral bounds, scalar cases, and the order argument. | Resolved |
| PI-09 | Chapter 9, Fundamental Theorem of Calculus | MAJOR | FTC I used a reversed integral for negative increments before an oriented-integral convention was defined. FTC II invoked the MVT when \(x=a\). | Treated positive and negative increments separately and handled \(x=a\) before applying MVT on \([a,x]\). | Resolved |
| PI-10 | Chapter 9, \(p\)-series test | MINOR | The dependency on real powers, logarithms, and FTC was implicit. | Cited the real-power and logarithm derivative theorems, displayed both antiderivatives, and invoked FTC II before the Integral Test. | Resolved |
| PI-11 | Chapter 9, step approximation | MINOR | Assigning a lower-sum value on every closed partition interval gave incompatible values at common endpoints and did not justify the pointwise comparison under the integral. | Defined endpoint values explicitly, introduced a dominating step function, and used order preservation. The finite-endpoint step-function proof was expanded. | Resolved |
| PI-12 | Chapters 4 and 6 | EDITORIAL | Two forward-looking discussions were formatted as theorems although no proof was intended. | Recast them as unnumbered explanatory paragraphs. | Resolved |
| PI-13 | Preface, README, outline/status descriptions | EDITORIAL | Documentation described the project as if only the architecture and Chapter 1 were present despite a substantial Part I, and the outline overstated a few Chapter 6--9 topics. | Updated the preface, README, and outline; the Integral Test is now described only in Chapter 9. | Resolved |

## Independent-audit conclusions before the final polish pass

- Chapters 2--9 have no unresolved **CRITICAL** or **MAJOR** issue identified by this audit.
- The construction and uniqueness framework for \(\mathbb R\), completeness equivalences, sequence and series results, power-series arguments, elementary-function definitions, Riemann theory, improper integration, and the Lebesgue criterion for Riemann integrability were checked for dependency order. No remaining circular dependency was found.
- At the time of this audit, the Integral Test and formal \(p\)-series test remained in Chapter 9. The later final-polish pass records the dependency-safe relocation of the rational-exponent result to Chapter 7.
- Parts II and later remain planned or less developed material; this audit does not certify them.

## Build and source checks

On 2026-08-21, main.tex compiled successfully with two MiKTeX pdflatex passes. The resulting 66-page PDF has no LaTeX errors, unresolved references, or matched overfull/underfull-box warnings in main.log.

## Final polish pass

The final polish pass retained the prior audit history and made the following dependency-safe organizational refinements.

- Chapter 7 now proves the \(p\)-series criterion for rational exponents using positive roots and Cauchy condensation. This is the strongest formulation available there without introducing arbitrary real powers prematurely.
- Chapter 9 retains the Integral Test and its \(p\)-series calculation as an analytic rederivation that extends the criterion to every real exponent after Chapter 8 defines
  \[
  x^p=\exp(p\log x).
  \]
- Chapter 8 now defines \(\log\) only after the exponential-bijection theorem, and defines the inverse trigonometric functions only after the corresponding trigonometric restrictions have been proved bijective.
- Chapter 1’s integration preview now matches the later Darboux-sum development. Focused exercises and brief explanatory paragraphs were added without altering the established proofs.

No new CRITICAL or MAJOR issue was found in this focused pass. On 2026-08-21, two post-polish MiKTeX pdflatex passes produced a clean 70-page PDF with no LaTeX errors, unresolved references, or matched overfull/underfull-box warnings.

## Section 9.5 Criterion Clarification

**Historical annotation (PI-11).** Superseded by later revision: the
Fourier-analytic Riemann--Lebesgue material was removed when Section 9.5 was
corrected to the intended Lebesgue criterion for Riemann integrability.

| Identifier | Location | Severity | Description and mathematical consequence | Repair made | Status |
|---|---|---|---|---|---|
| PI-14 | Chapter 9, Section 9.5 | MINOR | The criterion used the potentially ambiguous name “Riemann--Lebesgue,” and its covering proof compressed the conversion of closed partition intervals to open covers and the finite-cover estimate. | Renamed the result as Lebesgue's criterion, added terminology notes, a countable-cover lemma, and an explicit compact-interval Lebesgue-number argument. | Resolved |
| PI-15 | Chapter 9, Section 9.5 examples | EDITORIAL | The criterion lacked a contrasting example showing that a dense, countable discontinuity set can still permit Riemann integrability. | Added Thomae's function with complete continuity, discontinuity, negligibility, and integral-zero proofs, followed by the Dirichlet--Thomae comparison. | Resolved |

The Section 9.5 proof was checked after these changes: endpoint covers, the
good/bad interval estimates, compact finite subcovers, the identity
\[
\operatorname{Disc}(f)=\bigcup_{m=1}^{\infty}D_{1/m},
\]
and countable unions of negligible sets are all explicit.  No measure theory
is used.  No unresolved CRITICAL or MAJOR issue is known in Part I.

## Project-wide structural follow-up

The final structural pass does not alter any Part I mathematical statement or
proof.  All former remarks now use the upright theorem-style environment, and
each chapter has a dedicated Exercises section with a counter independent of
the definition--theorem--proposition counter.  No unresolved **CRITICAL** or
**MAJOR** issue was introduced or identified in Part I.

## Uniform-limit integration follow-up

Chapter 9 now contains a separate, proved uniform-interchange theorem for
Riemann integrals, its dominated-uniform formulation, and an explicit remark
that the genuine Lebesgue dominated convergence theorem needs only
almost-everywhere convergence.  This prevents the Riemann result from being
mistaken for the stronger measure-theoretic theorem.  Exercises headings are
now unnumbered while their chapter-based exercise numbers remain unchanged.

The same follow-up adds Dini's compact-continuous monotone-convergence
theorem for Riemann integrals.  It is explicitly distinguished from the full
Lebesgue monotone convergence theorem, which is not assumed or used.

## Convergence terminology polish

The uniform-plus-domination result is now a corollary titled ``Uniform
convergence under an integrable domination,'' rather than a Riemann
``dominated convergence theorem.''  The one-variable compact-continuous
result is named Dini's Theorem, and its passage through the integral is
explicitly identified as an application of the preceding uniform-interchange
theorem.  The forward-looking Lebesgue comparisons remain nontechnical.

## Foundational and finite-integration completion

This narrowly scoped completion pass makes the elementary arithmetic chain
\[
\N\longrightarrow\Z\longrightarrow\Q\longrightarrow\R
\]
explicit.  Chapter~2 now takes \(\N\) and \(\N_0\), with their usual
induction and well-ordering structure, as the restrained foundational
starting point, then constructs \(\Z\) and \(\Q\) as quotient sets and
records their operations, embeddings, and order.  Chapter~3 now points back
to this construction rather than treating \(\Q\) as an unexplained external
prerequisite.

Chapter~9 adds FTC-based one-variable substitution, integration by parts,
and the elementary mean-value theorem for integrals.  These use only the
chain rule, product rule, Extreme/Intermediate Value Theorems, and the two
parts of the FTC already available there.  The targeted dependency check
found no circularity and no unresolved **CRITICAL** or **MAJOR** issue in
Part~I.

## Final informal-preview clarification

Chapter~2 now labels the decimal presentation of Cantor's diagonal argument
as an informal preview. Chapter~3 constructs \(\R\), and Chapter~4 explains
that decimals acquire their later formal meaning through limits of finite
truncations. No subsequent formal result relies on this preview, and no
unresolved **CRITICAL** or **MAJOR** issue was introduced.

## Relations and ordered-field foundations

Chapter~2 now defines binary relations before equivalence relations and
introduces partial and total orders before they are used in Chapter~3.
Chapter~3 now defines an ordered field as a field with a compatible total
order; the positive-cone formulation is retained and proved equivalent.
The construction of the Cauchy-sequence model now invokes that
characterization explicitly. No later Chapter~3 proof required a substantive
change, and no unresolved **CRITICAL** or **MAJOR** issue was introduced.

## Publication-preparation review

The release-candidate review classified theorem-like material throughout the
notes and converted explanatory items labelled as remarks into the dedicated
`Remark` environment without altering their numbering sequence. The Part~I
exercise sets were checked for available prerequisites, stated hypotheses,
notation, and duplicate prompts; no substantive correction was required. The
front matter now identifies the notes as Version~1.0 Release Candidate,
documents the limits of the scope, and states that explicitly identified
external theorems may be used without proof. No new **CRITICAL** or **MAJOR**
issue was identified in Part~I.

</details>

<a id="historical-part-ii-audit"></a>
<details>
<summary>PART II AUDIT</summary>

# Part II Mathematical Audit

## Scope and method

This audit records the major mathematical and pedagogical revision of
Chapters 10--13 begun on 2026-08-21. Each theorem-level result is checked
for stated hypotheses, prior definitions, dependency order, compactness
arguments, differentiability assumptions, orientation conventions, and the
Jordan/Riemann restrictions used in Chapters 12 and 13.

Severity labels are:

- **CRITICAL:** a false theorem, circular argument, undefined object, or gap
  that breaks later development.
- **MAJOR:** a substantial proof gap, missing hypothesis, unjustified
  theorem-level claim, or dependency problem.
- **MINOR:** a localized missing argument, imprecise statement, or excessive
  compression.
- **EDITORIAL:** notation, cross-reference, wording, stale documentation, or
  formatting.

## Findings and repairs

| Identifier | Location | Severity | Description and mathematical consequence | Repair made | Status |
|---|---|---|---|---|---|
| PII-01 | Chapter 10, topology definitions | MAJOR | Closed sets were used in the closure definition before being defined. | Added the complement definition of closed subsets before closure is introduced. | Resolved |
| PII-02 | Chapter 10, compactness | MINOR | The Part I connection and the general compact-implies-uniformly-continuous theorem were absent, inviting later ad hoc arguments. | Added the metric-space theorem with a sequential-compactness proof. | Resolved |
| PII-03 | Chapter 10, determinants | MAJOR | The determinant formula used \(S_n\) and \(\operatorname{sgn}\) without a prior definition or proof of the required multiplicativity. | Added a purpose-built permutation/sign subsection based on inversions. | Resolved |
| PII-04 | Chapter 12, local volume comparison and change of variables | MAJOR | The existing proof relied on unproved box-enlargement and shrinkage claims, so the nonlinear change-of-variables proof was only a sketch. | Replaced it with a quantitative cube lemma: after normalizing by the derivative, a contraction argument proves both inner and outer volume bounds. The global proof now sums local errors and controls boundary strips in the Jordan framework. | Resolved |
| PII-05 | Chapter 13, partitions of unity and global Stokes | MAJOR | The argument silently used paracompactness and unproved smooth bump-function claims; the globalization of Stokes was too compressed. | Identified the second-countable manifold refinement step, constructed chartwise Euclidean bumps explicitly, and expanded the finite chartwise reduction in global Stokes. | Resolved |
| PII-06 | Chapter 11, partial derivatives | MINOR | The coordinate proof of the \(C^1\) differentiability criterion did not identify its intermediate points, and the failure of partial derivatives to imply differentiability was only implicit. | Added the coordinate polygonal path and Mean Value Theorem points explicitly, together with a worked counterexample. | Resolved |
| PII-07 | Chapters 10--13, Part I connections | EDITORIAL | The multivariable material did not consistently identify its one-variable prototypes. | Added targeted bridges for metric continuity, compactness, Fr\'echet derivatives, determinants/Jacobians, differential forms, and the FTC/Stokes relation. | Resolved |

## Current status

The baseline document compiled cleanly before this revision. Part I was not
altered. After the final dependency review, no unresolved **CRITICAL** or
**MAJOR** issue was identified in Chapters 10--13. The remaining use of the
second-countable manifold refinement is stated and motivated at the natural
undergraduate level; a full general-topology proof of paracompactness is
outside the intended scope.

## Final validation

On 2026-08-21, two final MiKTeX pdflatex passes compiled main.tex
successfully. The 114-page PDF has no LaTeX errors, unresolved references, or
matched overfull/underfull-box warnings in main.log.

## Structural and precision follow-up

| Identifier | Location | Severity | Description and mathematical consequence | Repair made | Status |
|---|---|---|---|---|---|
| PII-08 | Chapter 12, continuous functions on Jordan sets and change of variables | MINOR | The local integrability lemma was stated more strongly than required, while the global estimate used an unspecified \(O(\eta)\) term and the face-covering argument suppressed its quantitative bound. | Stated the bounded relative-continuity hypothesis actually needed for zero extensions, replaced the asymptotic notation by an explicit constant, and made the Lipschitz face-cover estimate explicit. | Resolved |
| PII-09 | Chapters 1--13, theorem styling and exercises | EDITORIAL | Remarks were styled separately and exercises shared the main theorem counter, obscuring both the requested uniform presentation and exercise numbering. | Recast every remark as an upright theorem-style result and gave exercises their own chapter-based counter under a dedicated Exercises section in every chapter. | Resolved |

No unresolved **CRITICAL** or **MAJOR** issue was identified in the focused
follow-up.  The nonlinear change-of-variables theorem remains explicitly a
Jordan/Riemann theorem; its hypotheses and the polar-coordinate exercise keep
the singular origin and the angular seam outside the direct application.

Two final MiKTeX pdflatex passes on 2026-08-21 produced the current
125-page PDF with no LaTeX errors, unresolved references, or matched
overfull/underfull-box warnings in `main.log`.

## Uniform-limit integration follow-up

Chapter 12 now states and proves the multiple-Riemann-integral analogue of
the Chapter 9 uniform-interchange theorem, and explicitly distinguishes it
from multivariable Lebesgue dominated convergence.  The result relies on
uniform convergence; domination alone is not substituted for it in the
Riemann setting.

Chapter 12 also gives the corresponding Dini's Theorem on rectangles and
explains why the unrestricted multivariable monotone convergence theorem
belongs to Lebesgue integration.

The latest two-pass MiKTeX build produces a clean 126-page PDF with no
LaTeX errors, unresolved references, or matched overfull/underfull-box
warnings in `main.log`.

## Terminology and manifold-dependency polish

Chapter 12 now calls the compact-continuous result Dini's Theorem and makes
its use of the preceding uniform-interchange theorem explicit; domination is
described only as a foreshadowing of the Lebesgue theorem.  Chapter 13 now
refers back to the Chapter 10 definition of homeomorphism and the Chapter 11
definition of diffeomorphism instead of duplicating either.  Its orientation
definition now identifies an orientation with an equivalence class of
oriented atlases and states the positive-transition characterization of
equivalent oriented atlases.

## Final targeted structural revision

| Identifier | Location | Severity | Description and mathematical consequence | Repair made | Status |
|---|---|---|---|---|---|
| PII-10 | Chapter 10, Theorem 10.18 (metric compactness) | MAJOR | A reintroduced proof error treated raw sequence tails as closed. For example, a tail of \(1/n\) in \([0,1]\) omits its limit point \(0\), so the compact finite-intersection argument did not apply as written. | Replaced raw tails by their closures; explicitly proved nonemptiness, closedness, nesting, the finite-intersection conclusion, and the recursive increasing-index construction. The converse now states the finite-ball and small-ball-cover arguments directly rather than relying on undefined named terminology. | Resolved |
| PII-11 | Chapter 10, compactness preliminaries | MINOR | Hausdorff was used in the compact-subsets theorem without an explicit definition. | Added a concise definition and the metric-space separation observation before its first use. | Resolved |
| PII-12 | Chapter 13, manifold globalization | MINOR | The refinement theorem and partitions of unity used second countability, local finiteness, refinement, precompactness, paracompactness, support, compact support, and subordination without a single prior terminology point. | Added a compact preliminary terminology block; preserved cross-references to the existing homeomorphism and diffeomorphism definitions. | Resolved |
| PII-13 | Chapter 13, General Stokes proof | EDITORIAL | “Boundary-preserving oriented charts” was not explicit terminology. | Replaced it with the stated half-space chart and boundary-hyperplane condition. | Resolved |
| PII-14 | Chapter 13, final section | EDITORIAL | The closing perspective did not yet map the principal natural continuations of the text. | Renamed it “Perspective and Further Directions” and added concise expository connections to measure theory, topology, functional analysis, complex analysis, differential geometry, de Rham theory, PDE, and probability. | Resolved |

The final terminology/dependency sweep confirms that Hausdorff, second
countable, locally finite, refinement, precompact, paracompact, support,
compact support, and subordinate are defined before their Chapter~13 uses.
The proof of metric compactness now avoids undeclared uses of “total
boundedness” and “Lebesgue number.” Homeomorphism and diffeomorphism remain
defined, respectively, in Chapters~10 and~11 and are referenced rather than
duplicated. No additional unresolved **CRITICAL** or **MAJOR** issue was
identified in this targeted revision.

On 2026-08-21, two final MiKTeX pdflatex passes produced the current
130-page PDF with no LaTeX errors, unresolved references, or matched
overfull/underfull-box warnings in main.log.

## Change-of-Variables Conceptual Bridge

Chapter~12 now includes an alternative pullback-and-manifold-integration
viewpoint immediately after its Riemann/Jordan change-of-variables theorem.
The existing analytic proof, including its local-volume and boundary-control
arguments, is preserved as the foundational proof.  The new discussion
explains the signed determinant in the pullback of a top-degree form, the
absolute value in scalar volume integration, and the role of orientation.  It
explicitly records the noncircular dependency from the Euclidean theorem to
coordinate invariance and then to manifold integration, with forward
references to Chapter~13.  It concludes by identifying Lebesgue theory as a
later, more flexible viewpoint without using or proving measure-theoretic
results here.

On 2026-08-21, two MiKTeX pdflatex passes after this addition produced the
current 131-page PDF with no LaTeX errors, unresolved references, or matched
overfull/underfull-box warnings in main.log.

## Integration-by-parts completion

Chapter~12 now derives the coordinatewise integration-by-parts formula on a
rectangle directly from the one-variable formula and Riemann--Fubini; it
states the coordinate-face contribution explicitly and records why an
intrinsic boundary integral waits for Chapter~13.  Chapter~13 now derives
the coordinate-free form identity from the graded Leibniz rule and General
Stokes.  This makes the progression from product rule plus FTC, through
Fubini on rectangles, to Stokes on manifolds explicit and gives an accurate
forward connection to Green identities and weak PDE formulations.  The
targeted dependency check found no unresolved **CRITICAL** or **MAJOR** issue
in Part~II.

## Final fixed-point and change-of-variables rigor pass

The following focused audit was completed on 2026-08-22.  It did not alter
the proof strategies or add topics beyond the prerequisites needed by the
six target results.

| Identifier | Location | Severity | Description and mathematical consequence | Repair made | Status |
|---|---|---|---|---|---|
| PII-15 | Chapter 11, Inverse Function Theorem | MAJOR | The fixed-point proof compressed the closed-ball self-map argument, local injectivity, the little-\(o\) conversion for the inverse, and continuity of matrix inversion. | Specified a complete closed ball and contraction constant; wrote the self-map and injectivity inequalities; constructed the precise open source and target neighborhoods; proved the inverse Lipschitz estimate and the remainder conversion; identified the perturbation proposition's base and perturbed maps; and proved continuity of inversion with a local inverse bound. | Resolved |
| PII-16 | Chapter 11, Implicit Function Theorem | MAJOR | The reduction to the inverse theorem did not fully record the product-neighborhood choices, pointwise uniqueness quantifiers, or nearby invertibility of \(D_yF\). | Chose the inverse neighborhoods and product neighborhoods explicitly, defined the implicit map through the second projection, proved uniqueness for every \(x\) and \(y\) in the stated neighborhoods, kept the graph in a region where \(D_yF\) is invertible, and checked the dimensions in the derivative formula. | Resolved |
| PII-17 | Chapter 12, linear volume and linear change of variables | MAJOR | Shear invariance, the passage from elementary matrices to general Jordan sets, null-overlap additivity, and the Darboux integrability squeeze were too compressed. | Proved shear preservation with quantitative inner and outer fiber prisms; tracked elementary volume and determinant multipliers through Gaussian elimination; proved boundary nullity by a face-cover estimate; added the required null-modification and finite-additivity result; distinguished transformed Jordan step functions from rectangular ones; and made the Darboux squeeze and prior measurability of the image explicit. | Resolved |
| PII-18 | Chapter 12, local volume comparison | MAJOR | The normalization argument omitted needed smallness, norm conversion, inner-cube surjectivity, local injectivity, and image-boundary details. | Required \(\delta<\min\{1,1/\sqrt n\}\), computed the normalized derivative, kept contraction in the Euclidean norm, proved the inner and outer cube inclusions, proved injectivity, established the compact-to-Hausdorff homeomorphism and boundary inclusion, quantified the Lipschitz face cover, and scaled the final estimate through the linear-volume lemma. | Resolved |
| PII-19 | Chapter 12, nonlinear change of variables | MAJOR | The global proof hid the Lebesgue-number step, determinant-tag transfer, construction and image control of discarded strips, finite additivity across image cubes, and the final epsilon bookkeeping. | Added and proved the compact-metric Lebesgue-number lemma in Chapter 10; selected a finite local cover with both local-volume and Jacobian controls; constructed retained cubes and explicit boundary rectangles; proved a uniform Lipschitz image-volume bound; summed the local integral errors using null-overlap additivity; controlled both discarded integrals; and completed a single ordered epsilon argument. | Resolved |
| PII-20 | Chapter 13, change of parametrization | MAJOR | The proposition was broader than the rectangular-domain change-of-variables theorem used in its proof. | Restricted the reparametrization to a diffeomorphism between open neighborhoods of compact rectangles mapping one rectangle onto the other, and applied the scalar theorem with the constant determinant sign stated explicitly. | Resolved |
| PII-21 | Chapter 13, support | EDITORIAL | PDF text extraction appeared to omit the closure in the support definition. | Verified that the LaTeX source already defines function and form support as the closure of the nonzero locus.  No source change was needed. | Resolved |

The polar-coordinate example and exercise continue to avoid both the
singular set \(r=0\) and the angular seam during each direct application of
the change-of-variables theorem.  The pullback discussion remains downstream
of the Euclidean theorem, so no circular dependency was introduced.  No
unresolved **CRITICAL** or **MAJOR** issue remains in the six target proofs.

## Final local well-definedness and notation cleanup

The proof of Proposition~13.26 now explicitly compares two subordinate
partitions through the finite common products
\(\rho_\alpha\sigma_\beta\) on the compact support of the form, using
Proposition~13.19 on chart overlaps. The classical consequences section now
also identifies the differential-form flux expression behind the customary
vector-calculus notation. These are local clarifications only; no unresolved
**CRITICAL** or **MAJOR** issue was found.

## Publication-preparation review

The release-candidate review identifies the manifold refinement theorem in
Chapter~13 as an **external theorem used without proof**, records its role in
the partition-of-unity construction, and cites a standard reference. The
remaining Chapter~10--13 principal results are proved within the manuscript
from their stated prerequisites. The Part~II exercises were checked for
dependency order, stated hypotheses, notation, and scope; no substantive
correction was required. Explanatory theorem-like items labelled as remarks
are now classified as `Remark`s. No new **CRITICAL** or **MAJOR** issue was
identified in Part~II.

</details>

<a id="historical-patch-3.1.1-audit"></a>
<details>
<summary>PATCH 3.1.1 AUDIT</summary>

# Focused proof-and-dependency patch: Version 3.1.1

Date: September 12, 2026. Baseline: Version 3.1.0 revision draft.

This is a local patch. Chapter and section ordering, subject scope, orientation conventions, notation, and the construction-first proof architecture remain intact. The only new subsection is the requested Euclidean-domain integration bridge in Section 13.10. README and source version metadata now agree on Version 3.1.1; the revision date remains September 12, 2026. No release, tag, commit, or push was made.

## Requested repairs

Numbers in the first column refer to the revision request. PDF pages below are physical pages; subtract seven for printed main-text page numbers.

| Request | Implementation | Nature and validation |
| --- | --- | --- |
| 1. Continuity of composition | Chapter 5, Proposition 5.22, `prop:continuous-composition-real`, PDF p. 54, immediately after continuity algebra. Chapter 8's chain-rule proof cites it on p. 81. | States the domains and point, applies the sequential criterion twice, and restricts the chain-rule source locally so its image lies in the target domain. Closes the Part I dependency. |
| 2. Reciprocal example's domain | Chapter 5, now Example 5.27, p. 55. | Uses x_n=1/(n+1) and y_n=1/(n+2). All terms belong to (0,1), input differences tend to zero, and reciprocal differences remain 1. No expansion of the example. |
| 3. Infinite L'Hôpital variants | Chapter 8, paragraph following Theorem 8.12, p. 83. | Separate finite-threshold proofs for 0/0 and infinity/infinity. The latter fixes K, chooses c, freezes c, and then bounds the positive prefactor and vanishing additive term. The negative case uses -f. The finite-limit theorem statement and proof are unchanged. |
| 4. Elementary series at zero | Chapter 8, Proposition 8.16, p. 84. | Separates x=0 before calculating consecutive-term ratios; the existing ratio-test calculation remains. |
| 5. Improper limit comparison | Chapter 9, Corollary 9.36, p. 112. | Explicitly assumes Riemann integrability on every finite [a,b]. The existing tail-comparison proof is unchanged. |
| 6. Determinant proof grammar | Chapter 10, Theorem 10.115, pp. 152–153. | Defines the transformed determinant map in a display and then asserts alternation and multilinearity in a separate sentence. This is a grammatical/presentation change, not a new determinant argument. |
| 7. Linear-image measurability | Chapter 12, Lemma 12.27, pp. 191–192. | Uses L=E_1^{-1}...E_k^{-1} and explicitly constructs A_j=E_{k-j+1}^{-1}(A_{j-1}). Each step first establishes Jordan measurability and then uses the volume rule. Only afterward are the identities multiplied. The unit cube and arbitrary rectangles follow by taking those initial sets; the redundant forward calculation has been removed. The existing shear argument is retained. |
| 8. Chapter 12 title | Chapter opening p. 181, contents p. 4, and bookmark. | All use “Multivariable Riemann Integration.” Checked the actual PDF bookmark as well as the rendered heading and contents. |
| 9A. Smooth Euclidean domains | Chapter 13, Section 13.10.1, p. 235, `sec:euclidean-integral-bridge`. | Specifies the induced Euclidean smooth structure, identity interior charts, and ambient boundary-straightening diffeomorphisms. Distinguishes these assumed domains from an arbitrary simple closed curve. |
| 9B. Jordan measurability | Proposition 13.68, p. 235, `prop:smooth-domain-jordan`. | Compact boundary is covered by finitely many images of compact coordinate faces. Derivatives are bounded on compact coordinate rectangles; segment estimates give Lipschitz bounds. The existing face-cover lemma gives nullness, followed by the Jordan boundary criterion. Includes the one-dimensional point-face case. |
| 9C. Agreement of integrals | Proposition 13.69, pp. 235–236, `prop:manifold-riemann-agreement`. | Uses finitely many localized functions and compact unions of coordinate grid rectangles. Chapter 12's compact-Jordan change-of-variables corollary establishes image measurability and compares each scalar integral with its coordinate integral. Chart signs convert determinants to absolute determinants. Support and Jordan set algebra justify extending the localized integral to the whole domain; summing the weights proves agreement. Stokes is not used in this proof. |
| 9C. Classical consequences | FTC and Green, p. 238; divergence, p. 239. | Each proof now cites the agreement proposition in addition to general Stokes. Green and divergence explicitly assume the smooth Euclidean domains just defined. The FTC citation closes the same identification in dimension one. |
| 10. One extension near compact support | Lemma 13.64, p. 233, `lem:compact-boundary-extension`; applied in Stokes on p. 237. | Chooses finitely many local extensions, constructs compactly supported Euclidean bumps, divides their weighted sum by the positive sum of bumps, and verifies agreement with the original coefficients on the half-space. Uses common weights for the finitely many form coefficients. Stokes then retains the ambient extension across the genuine boundary and uses the existing cutoff/zero extension only across artificial edges. |
| 11. Area exercise | Chapter 13, Exercise 13.12, p. 240. | Assumes a compact smooth planar domain with positively oriented boundary and asks for the one-half integral of x dy - y dx. References the precise global Green corollary. No Jordan curve theorem is assumed or added. |
| 12. Presentation cleanup | Chapter 6, Example 6.10 and Exercises 6.1–6.3, pp. 61 and 65; Chapter 13, pp. 236, 238, 240. | Restores ordinary inline prose for interval/function introductions and short requests. Retains useful displays for constructions, substantial formulas, and conclusions. The mathematical content of these presentation-only edits is unchanged. |
| 13. Preservation | Source comparisons against the saved 3.1.0 baseline; see below. | No changes to Chapter 11 or either appendix. Protected proof blocks in other edited chapters compare identically. |
| 14. Same-types audit | Focused source searches across all active chapters, appendices, preface, and references, followed by checks of relevant contexts. | Reviewed domain/integrability hypotheses, ratio denominators, compact extrema, finite-before-limit choices, construction/gluing interfaces, exercise domain assumptions, and references/titles. The small additional boundary-case treatment is recorded below. |
| 15. Build and record | Final `main.pdf`, README, ERRATA, this file, and local QA evidence. | Clean stabilized latexmk build, 273 pages, all edited locations visually inspected. Version/date synchronized. |

## Local alternatives and the same-types audit

The agreement proof uses Chapter 12's **compact Jordan-region change-of-variables corollary** on finite coordinate rectangle unions, including half-space rectangles. This directly handles ambient straightening charts and proves the necessary measurability before taking integrals. It avoids asserting a new half-space-to-curved-domain formula or invoking Stokes circularly. The existing half-space coordinate-integral convention supplies the meaning of the local manifold term.

The compact-extension justification is a short reusable lemma placed after the partition-of-unity construction and before integration. Its proof uses that existing finite bump construction, not a new topological extension theorem.

The linear-volume proof also explicitly treats zero-width boxes using the existing Lipschitz-face lemma before the shear calculation chooses a positive tolerance smaller than a side length. The chapter initially defines rectangles with positive side lengths; this short extension keeps the volume rule compatible with the degenerate boxes/faces used later in remainder-strip bookkeeping. No second shear proof was added.

The audit intentionally left already justified arguments alone:

- The ratio test already requires eventually nonzero terms. The power-series differentiation proof handles zero and infinite radii through inequalities, without arithmetic substitution of infinity.
- Improper integration's definition, ordinary comparison theorem, absolute-convergence proposition, and integral test already give the relevant finite-truncation hypotheses. Their proofs and statements remain unchanged apart from the requested limit-comparison statement.
- The differentiation-under-limits proof already chooses the finite index first and then freezes it before choosing the increment. The termwise corollary inherits the immediately preceding interval setup; its proof was not rewritten.
- The sequence compactness proof already uses closed tails, and local volume comparison already takes its derivative maximum over the closed ball. Literal LaTeX overlines were checked again.
- Manifold exterior differentiation already glues its local candidates and checks independence of boundary extensions. No replacement was needed there; the new lemma addresses the distinct need for one ambient extension near a whole compact support.
- Quotient/tensor constructions already construct maps before using uniqueness to compare them. Both appendices remain byte-for-byte identical to the baseline.
- The trigonometric-series discussion retains only its internally established convergence/continuity claims. The external refinement theorem and existing attribution notes are unchanged.
- Searches for hard-coded theorem/section numbers found only the intentional external algebra-note citations. Active internal references use labels. The full Chapter 13 title and intentional shorter running header remain consistent.

This was a focused mathematical and editorial audit, not formal verification of the entire manuscript or a new general expansion pass.

## Preservation evidence

The baseline is saved in `tmp/pre-focused-3.1.1/`. Source changes are confined to Chapters 5, 6, 8, 9, 10, 12, and 13, plus version/revision documentation. Chapter 6 changes are presentation only; Chapter 10 has only the requested local grammatical change. Chapters 1–4, 7, and 11, both appendices, the preface, and the references are unchanged from that baseline.

Automated source comparisons confirm unchanged statement/proof blocks for:

- finite-limit L'Hôpital, differentiation of a sequence, and termwise differentiation;
- Arzela bounded convergence;
- metric compactness and the full determinant construction;
- linear change of variables (including its grid-face repair), local volume comparison, and nonlinear change of variables (including its remainder-strip and separated-error architecture);
- tangent transitions, tangent-space structure, the intrinsic differential, manifold exterior derivative, partition of unity, and manifold-integral well-definedness.

The source diffs also retain the two-chart circle example, support localization, orientation/chart-sign conventions, and all established linear-algebra and tensor applications. The new extension and agreement statements are placed before their uses. These comparisons verify preservation of text; the written mathematical arguments were reviewed separately.

## Build and visual validation

- Ran `latexmk -pdf -interaction=nonstopmode -halt-on-error main.tex`. Latexmk completed its reruns and reported all targets up to date. Final build log: `tmp/focused-311-build.txt`.
- Final PDF: **273 pages**, three more than Version 3.1.0.
- Final log: no LaTeX errors or warnings, unresolved references, overfull boxes, or underfull boxes.
- Active-source check: **19 files, 326 unique labels, 352 resolved reference occurrences**. Environment/display pairing checks pass. The rendered inserted theorem numbers and their references were checked.
- All 273 pages were rendered. Full-size visual inspection covered physical pages **1, 4–5, 54–55, 61, 65, 80–81, 83–84, 112, 152–153, 181, 191–192, 233, 235–240**. This covers every authored change, including the cover, contents, title, proof continuations, and revised exercises.
- No malformed equations, clipping, duplicated inserted paragraphs, or headings stranded without their opening text were found at the changed locations. The agreement statement ends a page and its complete proof begins the next; both are legible and the subsection heading stays with its introductory text.
- Cover, README, and preamble agree on Version 3.1.1 and September 12, 2026. PDF bookmarks for Chapters 12 and 13 were checked programmatically. `git diff --check` passes; Git reports only existing LF/CRLF normalization notices.

Final PDF SHA-256: `79d64e9601e14faa52e261ef21b37a633e8647c75d50c6b787190cf158d281af`.

Machine-readable evidence in `tmp/focused-311-qa/`: `preservation-check.json`, `source-check.json`, `render-manifest.json`, and `final-artifact-check.json`, together with focused chapter diffs and rendered pages. Existing backup copies and previous revision-audit files were preserved.

</details>

<a id="historical-pedagogical-dependency-3.2.0-audit"></a>
<details>
<summary>PEDAGOGICAL DEPENDENCY 3.2.0 AUDIT</summary>

# Version 3.2.0 pedagogical-and-dependency revision audit

Revision date: September 12, 2026. Baseline: the current working Version 3.1.1 draft, preserved in `tmp/pre-focused-3.2.0/` before edits. Existing unrelated working-tree changes and historical revision records were retained. No GitHub tag or release was created.

This pass preserves chapter order and the overall course architecture. Rows 1–8 are mathematical dependency repairs; exposition additions are recorded separately and are not described as mathematical corrections. “Location” gives the final source file and one-based starting line, with an anchor describing the relevant passage rather than relying on old theorem numbers.

## Requested items

| Item | Exact starting location | Classification | Implementation / disposition |
| --- | --- | --- | --- |
| 1. First-order extremum condition | `chapters/ch11-multivariable-differentiation.tex:701` | Dependency repair | Proved by fixed-line restriction and cited in optimization and boundary classification; explains both signs of the parameter. |
| 2. Half-space derivatives | `chapters/ch12-multivariable-integration.tex:1800` | Dependency repair | Extension independence, composition, and both inverse derivative identities precede the half-space corollary and Chapter 13; no use of boundary preservation in the lemma. |
| 3. Boundary structure | `chapters/ch13-forms-stokes.tex:1454` | Dependency repair | Proves interior open, boundary closed, induced boundary atlas, inherited separation/countability, and smooth inclusion with injective derivative; adds transverse block sign. |
| 4. Support lemmas | `chapters/ch13-forms-stokes.tex:1846` | Dependency repair | Proves both support inclusions and compactness, gives constant-map counterexample, and checks both Stokes integrals before its statement. |
| 5. Compact cutoff | `chapters/ch13-forms-stokes.tex:2053` | Dependency repair | Derived after partition of unity using the two-set cover; defines compact-support notation and cites the corollary in Stokes. |
| 6. Continuous forms | `chapters/ch13-forms-stokes.tex:754` | Dependency repair | Defines continuous coefficients before integration; continuous pullback by a C1 map follows from coefficient products. Stokes regularity unchanged. |
| 7. Zero-dimensional integration | `chapters/ch13-forms-stokes.tex:1082` | Dependency repair | Signed point sum before the interval boundary integral; extends to compact support on discrete manifolds. Later orientation paragraph only explains signs. |
| 8. Ambient surface form restriction | `chapters/ch13-forms-stokes.tex:2561` | Dependency repair | Constructs both inclusions and applies Stokes to the pullback; explicitly states induced surface smooth structure and identifies work and curl flux. |
| 9. Frechet derivative types | `chapters/ch11-multivariable-differentiation.tex:19` | Pedagogical expansion | Input/output increments, openness, linear versus affine approximation, epsilon-delta statement, and affine example. |
| 10. Uniqueness scaling and continuity | `chapters/ch11-multivariable-differentiation.tex:122` | Pedagogical expansion | Displays the scale-invariant normalized expression and the norm remainder bound for continuity. |
| 11. Output components | `chapters/ch11-multivariable-differentiation.tex:297` | Pedagogical expansion | Both directions proved with finite-dimensional estimates; warns against replacing full input differentiability by coordinate-line tests. |
| 12. Vector partials and Jacobian | `chapters/ch11-multivariable-differentiation.tex:236` | Pedagogical expansion | Scalar entries, vector columns, and matrix representation precede the Jacobian display; continuous-partials theorem uses representation wording and handles zero coordinate increments separately. |
| 13. Directional derivatives | `chapters/ch11-multivariable-differentiation.tex:229` | Pedagogical expansion | Fixed direction/speed and scalar parameter, homogeneity, polynomial example, explicit nonadditivity, zero functional wording, and changing-direction path. |
| 14. Pointwise versus uniform | `chapters/ch11-multivariable-differentiation.tex:502` | Pedagogical expansion | Quantified one-delta condition over all unit directions; no new differentiability theory. |
| 15. C1 regularity | `chapters/ch11-multivariable-differentiation.tex:404` | Pedagogical expansion | Linear-map-valued continuity, partials equivalence with proof, and differentiable non-C1 example. |
| 16. Gradient geometry | `chapters/ch11-multivariable-differentiation.tex:716` | Pedagogical expansion | Cauchy–Schwarz maximum, attaining unit direction, inner-product dependence, and covector distinction. |
| 17. Local Lipschitz consequence | `chapters/ch11-multivariable-differentiation.tex:567` | Pedagogical expansion | Derivative bound on a convex domain and small-ball proof for every C1 map. |
| 18. Higher derivatives and Taylor | `chapters/ch11-multivariable-differentiation.tex:606` | Pedagogical expansion | Multilinear norm and estimate, Chapter 10 boundedness, first two segment derivatives, quadratic worked example, and varied duplicate exercises. |
| 19. Contraction mechanism | `chapters/ch11-multivariable-differentiation.tex:894` | Pedagogical expansion | Displays finite geometric sum and uniform Cauchy bound, then the complete limit/fixed-point identity. |
| 20. Inverse motivation and evaluation | `chapters/ch11-multivariable-differentiation.tex:1006` | Pedagogical expansion | Affine exact-solution motivation, nonzero source/target inverse matrices, sufficient-condition caveat; four-stage proof preserved verbatim. |
| 21. Block derivatives | `chapters/ch11-multivariable-differentiation.tex:1328` | Pedagogical expansion | Block definitions and domains/codomains, vector zero equation, square auxiliary-map dimensions; detailed implicit proof retained. |
| 22. Optimization and exercises | `chapters/ch11-multivariable-differentiation.tex:711` | Pedagogical expansion | Candidate versus classification discussion, both compactness and attainment references, irregular defining-equation example, cusp exercise clarified, all end exercises precede transition. |
| 23. Scalar integration opening | `chapters/ch12-multivariable-integration.tex:12` | Pedagogical expansion | One vector input point and one ordered real output precede sums. |
| 24. Why Darboux arguments transfer | `chapters/ch12-multivariable-integration.tex:68` | Pedagogical expansion | Explicit analogy table, volume subdivision, ordered inf/sup inequalities, and refinement mechanism. |
| 25. Rectangular step functions | `chapters/ch12-multivariable-integration.tex:42` | Pedagogical expansion | Disjoint endpoint ownership, representation-independent integral, closed-cell lower/upper approximants, and elementary agreement with Darboux integral before Jordan theory. |
| 26. Multiple-integral notation | `chapters/ch12-multivariable-integration.tex:103` | Pedagogical expansion | Expanded coordinate volume first, then dx abbreviation and double/triple examples; distinguished from forms. |
| 27. Multiple versus iterated | `chapters/ch12-multivariable-integration.tex:304` | Pedagogical expansion | Direct grid definition versus successive integrals, with Fubini supplying equality. |
| 28. Vector integration | `chapters/ch12-multivariable-integration.tex:256` | Pedagogical expansion | Introduced after scalar linearity; proves linear combinations, commutation with linear maps, and continuous integrability. |
| 29. Fubini block variables | `chapters/ch12-multivariable-integration.tex:311` | Pedagogical expansion | Fixed-block section, scalar G, both block dimensions, and workflow; corrected estimate citation and p-variable proof wording. |
| 30. Coordinatewise integration by parts | `chapters/ch12-multivariable-integration.tex:412` | Pedagogical expansion | Two-dimensional example, remaining coordinates and face integral, including explicit n=1 empty-tuple convention. |
| 31. Zero-extension domain | `chapters/ch12-multivariable-integration.tex:609` | Pedagogical expansion | Piecewise map on containing rectangle, restrictions, and warning against undefined multiplication; existing integrability warning retained. |
| 32. Compact support on open sets | `chapters/ch12-multivariable-integration.tex:1764` | Pedagogical expansion | Relative closure, separation from exterior, continuous zero extension, and rectangle containing only support; proper Riemann interpretation. |
| 33. Substitution types | `chapters/ch12-multivariable-integration.tex:1385` | Pedagogical expansion | Source/target diagram, transformed scalar integrand, composition versus volume factor, and renaming versus substitution. |
| 34. Local normalization | `chapters/ch12-multivariable-integration.tex:1239` | Pedagogical expansion | Explains each operation and expands chain-rule derivative; cube comparison proof otherwise retained. |
| 35. Oscillation notation | `chapters/ch12-multivariable-integration.tex:144` | Pedagogical expansion | Cell osc, pointwise omega, and modulus mu have separate input types; updates shear and nonlinear proof notation. |
| 36. Line-integral scalar functions | `chapters/ch13-forms-stokes.tex:48` | Pedagogical expansion | Field types and scalar g/h before integration, with piecewise continuity/existence and distinction from vector integral. |
| 37. Planar work notation | `chapters/ch13-forms-stokes.tex:114` | Pedagogical expansion | Full parameter coefficient and differential factors before the running example and Green; distinguishes area notation. |
| 38. Reparametrization versus path independence | `chapters/ch13-forms-stokes.tex:144` | Pedagogical expansion | Same traversal versus distinct paths, using the gradient line FTC. |
| 39. Surface dimensions and scalars | `chapters/ch13-forms-stokes.tex:312` | Pedagogical expansion | 3-by-2 derivative, no determinant, scalar area factor and integrands, normal cancellation, and two-dimensional parameter area. |
| 40. Surface reparametrization calculation | `chapters/ch13-forms-stokes.tex:350` | Pedagogical expansion | Expands both tangent derivatives and all cross-product contributions; determinant belongs to the parameter change. |
| 41. Form versus value | `chapters/ch13-forms-stokes.tex:692` | Pedagogical expansion | Base point versus vector slots, degree versus polynomial power, and pointwise exterior space versus space of forms. Corrects ambiguous requested notation by writing omega_p(v) for v=(v1,v2). |
| 42. Pullback coordinate rules | `chapters/ch13-forms-stokes.tex:802` | Pedagogical expansion | Derives function and differential rules by evaluation, including continuous coefficients; distinguishes existence from integral invariance. |
| 43. Second derivative versus d squared | `chapters/ch13-forms-stokes.tex:1015` | Pedagogical expansion | Nonzero symmetric Hessian compared with zero antisymmetrized exterior derivative for x squared plus y squared. |
| 44. Parametrized scalar coefficient | `chapters/ch13-forms-stokes.tex:1235` | Pedagogical expansion | Derives coefficient by evaluating on the parameter basis, checks integrability, and compares graph two-form integral with unsigned area. |
| 45. Tangent coordinate basis | `chapters/ch13-forms-stokes.tex:1615` | Pedagogical expansion | Names the constructed basis and its dual, then connects inclusion differential to graph tangent plane; no derivation model. |
| 46. Boundary pullback | `chapters/ch13-forms-stokes.tex:1160` | Pedagogical expansion | Computes inclusion pullback, vanishing transverse differential, rectangular face explanation, and optional annulus signs. |
| 47. Smooth partition motivation | `chapters/ch13-forms-stokes.tex:1871` | Pedagogical expansion | Indicator discontinuity, smooth localized forms, derivative cancellation, local versus pointwise finiteness; removes repeated motivation without changing construction. |
| 48. Manifold integral workflow | `chapters/ch13-forms-stokes.tex:2112` | Pedagogical expansion | Localized form, coordinate top coefficient, signed scalar integrals, and workflow precede compact formula; refinement proof and circle example preserved. |
| 49. Stokes form-degree guide | `chapters/ch13-forms-stokes.tex:2487` | Pedagogical expansion | Four-case degree table, work versus flux forms, surface dimension, and local-angle/global-obstruction clarification. |
| 50. Early Ck convention | `chapters/ch08-differentiation.tex:18` | Pedagogical expansion | Open-interval derivatives and continuous one-sided endpoint extensions before serious use. |
| 51. Determinant wording | `chapters/ch10-topology-linear-algebra.tex:2108` | Terminology/wording cleanup | Already correct in the current 3.1.1 draft: “Define F” followed by “This map is alternating and n-linear.” Verified and retained without editing Chapter 10. |
| 52. Appendix B terminology | `chapters/app-tensors.tex:863` | Terminology/wording cleanup | Renames the bilinear map B in tensor–map proof; calls the degree-two exterior vector a bivector in the nondecomposable example. |

## Focused whole-manuscript audit

Reviewed active manuscript sources (excluding historical “Copy” files) for type changes, componentwise arguments, integrability/support, pullback maps, boundary derivatives, coordinate matrices, reused oscillation notation, and exercise prerequisites. Search evidence is in `tmp/focused-320-audit-search.txt`; the source/reference and dependency-order checks are in `tmp/revise_320_qa.py` and `tmp/focused-320-qa/manifest.json`.

- Additional corrections within this scope: changed implicit-proof “m-by-n map” wording to actual source/target spaces and separate matrix sizes; changed the polar example to a Jacobian representation; distinguished the shear proof's cell oscillation from its function argument; supplied smooth compact-support hypotheses before the Chapter 12 form preview's integrals; defined the empty-tuple face integral for the n=1 integration-by-parts case; defined C_c-infinity notation at first use.
- Chapter 10's foundations and determinant section are unchanged from the working baseline. Earlier “componentwise” uses there and in Appendix B concern vector operations and finite coordinate formulas, not an unproved differentiability equivalence. Chapter 8's remaining “same proof” text is followed by the relevant endpoint/domain mechanism.
- Chapter 11's cusp exercise now asks about the full local zero set and separately treats both one-sided branches. Its quadratic exercise and later Peano exercise now use different functions from the worked example. All chapter-end exercises precede the transition. No new stronger theorem requirement was found in the focused exercise review.
- Local-normalization changes explain the existing map; nonlinear change-of-variables changes explain notation and rename moduli. They do not replace the grid-boundary, strip-error, Jordan, or local-volume arguments.
- Tangent construction, manifold differential, partition construction, common-refinement proof, compact boundary-extension lemma, two-chart circle, and general Stokes architecture remain. General Stokes gained an explicit cutoff citation and prior existence checks. The surface corollary now constructs the pulled-back form.

## Deliberate dispositions

- Item 51 was already satisfied in the supplied working draft; no redundant edit was made.
- In item 41, the requested expression `omega_p(v1,v2)` could look like two vector inputs to a one-form. The text instead writes `omega_p(v)=a^2 v2` with the single vector `v=(v1,v2)` explicitly declared. This implements the intended example with unambiguous type information.
- The optional transverse-block, annulus, and locally-bijective cube examples were included. No required mathematical item was omitted. No general embedding theory, bundles as main-text sections, derivation tangent model, densities, measure theory, or broader topology course was added.
- Regularity remains smooth for exterior differentiation and Stokes. The continuous-form convention only supplies the integration and C1-pullback cases requested.

## Preservation and verification

Automated checks resolved all 368 reference occurrences against 332 unique labels and checked matching environments and the repaired dependency order. Exact pre-pass/final proof-body comparisons passed for 13 protected results: `thm:heine-borel-rn`, `thm:compact-extreme-value`, `prop:multivariable-derivative-rules`, `thm:schwarz`, `prop:perturbation`, `thm:multivariable-inverse-function`, `prop:jordan-boundary-criterion`, `prop:jordan-null-additivity`, `thm:linear-change-variables`, `thm:tangent-space`, `thm:manifold-differential`, `thm:partition-unity`, `prop:manifold-integral-well-defined`.

Build command: `latexmk -pdf -interaction=nonstopmode -halt-on-error main.tex` (the requested PDF build with diagnostic flags). MiKTeX was run through its installed executable because the desktop sandbox could not launch it directly. Latexmk completed its required reruns and reported all targets up to date. Final log: `tmp/focused-320-build-final.txt`; TeX log: `main.log`. No LaTeX errors, unresolved references, rerun warnings, malformed environments, or overfull/underfull boxes remain. The source version/date are read by the title page through the preamble macros and match README: Version 3.2.0 (revision draft), September 12, 2026.

Final PDF: 287 pages. SHA-256: `e33bd549d0d8e6b0df6b42f696291e10b07e6ad07d6d2130befb6efd684e9d35`.

## Visual review

Rendered the focused review pages to PNG and inspected contact sheets plus detailed pages. Checked opening Chapter 11 pages; directional, component/Jacobian, inverse/implicit transitions; Chapter 12 opening, step/Darboux notation, Fubini blocks, coordinatewise integration by parts, and change-of-variables notation; line/surface definitions; first forms and pullbacks; tangent/boundary passages; smooth partition motivation; manifold integration; and general/classical Stokes. Review also covers zero-dimensional integration and support lemmas. Corrected the Fubini diagram label overlap, new reference-related overflow, and an awkward split in the local-versus-global inverse example; removed repeated partition motivation. Final-page review evidence and PDF hash are in `tmp/focused-320-qa/`.

The following are physical PDF page numbers, including front matter (not printed chapter page numbers):

- chapter11-opening: 163.
- uniqueness: 164.
- jacobian-components: 167.
- continuous-partials: 168.
- directional: 169.
- uniform-directional: 170.
- higher-derivatives: 171.
- extremum: 172.
- inverse-transition: 177.
- implicit-transition: 181.
- chapter12-opening: 188.
- step-functions: 188.
- darboux-notation: 189.
- fubini: 192.
- integration-by-parts: 193.
- zero-extension: 196.
- local-normalization: 204.
- change-variables: 206.
- halfspace: 212.
- line-integrals: 218.
- surface-integrals: 222.
- forms: 227.
- pullback: 228.
- local-stokes: 233.
- parametrized-forms: 234.
- boundary: 237.
- tangent-basis: 239.
- partition-motivation: 243.
- cutoff: 245, 250.
- manifold-integral: 246.
- stokes-existence: 249.
- stokes-proof: 250.
- classical-guide: 251.
- surface-stokes: 252.
- jacobian-matrix: 166.
- zero-dimensional: 232.
- support-lemma: 242.

</details>

<a id="historical-pedagogy-3.5.0-audit"></a>
<details>
<summary>PEDAGOGY 3.5.0 AUDIT</summary>

# Version 3.5.0: focused pedagogical revision

Baseline: the working source corresponding to Version 3.4.1, saved before
editing in `tmp/revision-342-baseline/`. This revision preserves the user's
existing uncommitted work and does not create a commit, tag, or release.

## Coverage of the request

| Area | Revision |
| --- | --- |
| 10: linear estimates | Replaced the matrix-entry continuity proof with a finite-basis coefficient-norm Lipschitz proof. Explained normalization, the least amplification constant, attainment, dependence on both norms, exact versus upper bounds, and the gradient/functional bridge. |
| 10: series | Added the finite-dimensional vector-series bridge, absolute convergence by completeness, commutation with linear maps, and the operator geometric series. The later perturbation proof now cites it and records the inverse composition order. |
| 10: determinants | Added a self-contained inversion-based proof of the swap, composition, and inverse sign rules before determinant construction. Displayed the forced expansion with the scalar c; retained the expanded slot mechanism and verified the Leibniz construction. Appendix A is explicitly supplementary. |
| 10/12: geometric factorization | Removed the elimination determinant example and named elementary-matrix machinery. The replacement normalizes the first basis image with target maps, removes the other first components with source shears, inducts on the complementary space, and explicitly undoes the changes on the correct sides. Linear-volume scaling now applies the geometric factors in their actual order. The historical lemma label is retained for references. |
| 11: opening | Added Section 11.1 with limits and continuity, pointwise/uniform convergence, and equicontinuity/Arzelà–Ascoli. Recalled existing path examples, added one curved-path warning, displayed component and quantifier criteria, and distinguished sequences of points from sequences of functions. |
| 11: families | Proved compact equicontinuity implies uniform equicontinuity; constructed the dense set from finite nets, selected a diagonal subsequence, and used a finite net for uniform Cauchyness. Chapter 6 remains unchanged and is explicitly cited as the first interval treatment. |
| 11: differentiation | Added scalar mean-value equality before the vector estimate, retained the vector counterexample, and proved differentiating limits on a closed ball with a typed operator-valued derivative limit. Added the derivative-bound/equicontinuity bridge. |
| 11: higher derivatives | Added the typed second-order chain rule, Taylor polynomial and homogeneous-polynomial interpretation, Hessian coordinate forms, general Peano error, and the vector norm error bound via a fixed scalar projection. Expanded the existing exponential-cosine example rather than duplicating it. |
| 11: convexity | Proved supporting-hyperplane and everywhere-positive-semidefinite-Hessian criteria by segment restriction. Distinguished global convexity from the local critical-point Hessian test and supplied a quadratic optimization example. |
| 11: inverse/implicit consequences | Added regular level graphs, velocities equal to the derivative kernel, projection coordinates, local diffeomorphisms as open maps, local orientation sign, and parameter dependence with a square-root branch example. These precede Lagrange multipliers; the existing inverse/implicit proofs remain unchanged. |
| 9: computations | Added the two FTC directions immediately after the second FTC proof, and the logarithm integration-by-parts example explaining the factor choice. Retained the existing exponential example and exercises. |
| 12: opening | Placed the concrete two-dimensional grid before general product cells. Explicitly relabeled the finite collection, displayed its union and volume sum, and used that finite indexing for the first Darboux sums. Taught common refinement and its local inequalities before abbreviation. Added tagged sums and promoted the existing four-cell example and figure. |
| 12: integrability | Displayed mesh and the boxed oscillation-volume gap identity before proving continuous integrability through the modulus of continuity. Moved owned-cell functions and compatibility after continuous integrability, explained their purpose, and added the gluing roadmap and explicit local-sum identities. Corrected the moved material's directional reference to sums defined above. |
| 12: computations | Added the coordinatewise FTC, a two-variable calculation, a complete integration-by-parts computation with face and remaining integrals, and the endpoint/face comparison. |
| 12: convergence | Kept uniform interchange, explained absolute-error integral convergence and zero-extension transfer to Jordan regions, and proved multivariable Arzelà bounded convergence through elementary open-box content. Retained Dini in Chapter 12 and compared the distinct hypotheses and mechanisms without adding Lebesgue theory. |
| Appendices | Reframed Appendix A's introduction without removing its fuller permutation or arbitrary-field material. In Appendix B, displayed the binary tensor map's complete source/target and defining values, and renamed the two evaluation inputs in B.29 to xi and eta. No other Appendix B expansion was made. |
| Documentation | Updated the cover version/date, README, and OUTLINE. Existing symbolic references automatically track renumbering. |

## Mathematical and dependency review

The geometric factorization has `A L B = I ⊕ L'`, hence
`L = A⁻¹ (I ⊕ L') B⁻¹`; target and source compositions are explicitly
distinguished. The volume proof independently names factors in order of
application, establishes Jordan measurability at every step, and only then
uses the corresponding volume identity.

The vector Taylor bound projects onto the final remainder direction and
applies the scalar theorem to that fixed projection. It does not assert a
common Lagrange point for vector components. The Peano argument uses only
continuity of the kth derivative. Convexity is stated on an open convex
domain, and the local positive-Hessian comparison includes the critical-point
hypothesis. Regular-level tangent directions are defined through actual
curve velocities, and both inclusions in the kernel characterization are proved.

The open-box-content lemma uses only finite box volumes and compactness.
Subadditivity follows by a finite subcover and a subordinate subdivision of
each compact test union. A nearly maximizing compact box union leaves an
open remainder of small content. Summable losses then produce nonempty
nested compact intersections. Applying this to tail unions of open bad
cells proves bounded convergence with a separately integrable limit; no
Jordan measurability of an arbitrary open set, countable Jordan additivity,
or Lebesgue measure is asserted. The lemma's numbered clauses and proof
references use matching numerals.

## Preservation and cross-reference audit

Only Chapters 9–12 and Appendices A–B differ from the saved chapter baseline.
Chapters 1–8, Chapter 13, the preface, and references are unchanged. In
particular Chapter 3's architecture, Chapter 6's original family theory,
and the complete Chapter 13 manifold, boundary, support, and Stokes material
remain intact. Appendix B's foundational and universal-property proofs
remain intact except for the requested local input renaming.

The automated audit explicitly compares ten protected proof bodies, including
the inverse and implicit theorems, mixed partials, chain-rule algebra,
Lagrange multipliers, the Jordan criterion, local volume comparison, linear
and nonlinear changes of variables, and half-space derivatives. All match
the baseline. Differentiability counterexamples retain their original order.

The included sources contain 364 distinct labels and 381 reference uses,
with no missing targets or duplicates. Environment balance and control-character
checks pass. Numeric-reference searches found only the intentionally fixed
reference to Theorem 5.12.3 in the author's external algebra notes; the
renumbered manuscript uses symbolic references. Dini remains in Chapter 12.

## Build and visual review

Built with the installed MiKTeX `latexmk -pdf main.tex`, adding
`-interaction=nonstopmode -halt-on-error` for diagnostics. The final PDF has
316 pages. The stabilized log contains no LaTeX warnings, undefined
references, duplicate labels, or overfull/underfull boxes. Extracted text
from every page contains no unresolved `??`. The MiKTeX launcher emits its
existing Perl locale fallback; the compiler and latexmk complete successfully.

Visual review covers 81 distinct PDF pages: cover/contents 1–6; Chapter 9
110–112; Chapter 10's revised tail and all of Chapter 11, 151–195;
Chapter 12 opening and computations, 196–207; linear volume, 215–220;
convergence, 232–236; Appendix A, 282–283; and the touched Appendix B
pages, 297 and 301. Contact sheets and individual page images are in
`tmp/qa342/`. Figure checks cover the new grid, lower/upper columns,
tangent-plane and gradient figures, circle graph, and linear-volume figures.

The page-break review prompted local space reservations that keep the circle
example with its diagram and the concrete grid paragraph with its diagram.
All affected pages were re-rendered and inspected after those changes.
No clipping, overlapping labels, caption mismatch, or problematic whitespace
remains in the reviewed material.

Evidence: `tmp/build-342-final.txt`, `main.log`, `tmp/qa342/audit.json`,
the baseline-relative chapter diffs in `tmp/qa342/`, and
`tmp/qa342/compiled-text.txt`. Review scripts are `tmp/qa342.py` and
`tmp/finalqa342.py`. The final PDF remains at the repository's established
`main.pdf` path.

</details>

<a id="historical-pedagogy-3.6.0-audit"></a>
<details>
<summary>PEDAGOGY 3.6.0 AUDIT</summary>

# Version 3.6.0 revision audit

September 13, 2026. Baseline: the local Version 3.5.0 manuscript saved before
this revision, rather than the older Git HEAD. The changes are a local review
draft; no commit, tag, or release was created.

## Chapters 10–12

- Chapter 10 adds a subsection after matrix multiplication on augmented matrices,
  echelon and reduced echelon forms, pivots and free variables, Gaussian and
  Gauss–Jordan elimination, consistency, elementary matrices, and inversion.
  A three-variable system is reduced and checked; a second example distinguishes
  free parameters from inconsistency. Determinant row-operation rules appear
  after determinant construction and transpose invariance. A triangularization
  calculation complements the existing sparse cofactor examples. The gradient
  operator-norm identity now explicitly assumes a Euclidean source.
- Chapter 11 explains substitution, rationalization, norm bounds, uniform radial
  estimates, path tests, balancing denominator terms to choose curves, and the
  difference between joint and iterated limits. The existing examples carry
  these lessons rather than introducing additional pathologies. Function
  sequences are treated through fixed inputs, error functions, exact suprema,
  moving bad points, domain bounds, componentwise tests, and index dependencies.
  Boxed workflows summarize both methods. The Arzelà–Ascoli application checklist
  distinguishes convergence of a subsequence from convergence of a sequence.
- The Jacobian discussion derives columns from the derivative's basis images,
  explains rows and dimensions, works a rectangular example, and expands the
  existing two-component example into an affine prediction. Composition includes
  dimension annotations. Matrix and determinant terminology is explicit.
- The second-order Peano proof cites the **C^k Peano part** of the general
  corollary. The Lagrange proof invokes the regular-level-set corollary for
  tangent equals kernel and retains the explicit functional-proportionality
  argument. The touched segment-Taylor regularity hypothesis is integrated
  into its sentence.
- Chapter 12 uses Latin cell indices, with distinct indices for local refinement;
  named moduli of continuity are unchanged. Backward references identify the
  Chapter 9 Darboux, continuous-integrability, algebra, absolute-value, additivity,
  FTC, uniform-interchange, Arzelà, and Dini mechanisms. A comparison table maps
  interval length and compact interval approximations to box content and compact
  box approximations. Closed-cell Darboux theory still precedes owned-cell step
  functions. New multidimensional geometry is retained in full.

## Appendix B: source alignment and final scope

The source consulted is the current sibling Algebra project's
`chapters/tensor-products.tex`, with its included `chapters/exterior-algebra.tex`.
These are the source files for Chapter 8; the stale nested Algebra copy was not
used. The Algebra project was not edited.

| Algebra Chapter 8 progression | Appendix B treatment |
| --- | --- |
| Binary universal construction | Bilinear vector-space problem, formal basis, relation subspace, quotient factorization, uniqueness and working rule; a self-contained quotient prelude is retained. |
| Finite associativity | Both nested maps constructed by successive universal properties; both composites checked. |
| Direct sums | Specialized to **finite** families only, with independently constructed maps for both slots and both inverse identities. |
| Symmetry | Field-vector-space swap, after associativity and direct sums. |
| Finite multilinear products | Direct construction followed by comparison with every binary parenthesization, preserving the full map-valued induction. |
| Induced maps and calculations | Binary and finite-factor maps, scalar unit over the same field, basis detectors, rectangular coordinate calculations, and four-component direct-sum example. |
| Tensor–Hom | The entire previous section is preserved verbatim: currying and its inverse, linearity and both identities, finite-dimensional tensor–map identification and inverse, basis independence, and matrix units. A compatibility calculation is added afterward. |
| Exterior powers | Alternation quotient, characteristic-two distinction, basis detectors, nonvanishing, induced exterior maps through both tensor and quotient stages, minors, determinant, and constructed wedge multiplication. |
| Exterior algebra and alternating forms | A finite direct sum of degrees for finite-dimensional V, grading, computations, determinant pairing, duality inverses, and compatibility with Chapter 13. |

The user's additions govern the specialization: only vector spaces are discussed;
only finite direct sums are included; there is no restriction or extension of
scalars; and exactness is omitted. Accordingly, Chapter 8's broader scalar
settings, scalar-change discussions, exactness, and flatness are not imported.
The scalar-unit isomorphism uses the same fixed field throughout and does not
change scalars. Formal-symbol constructions still use finite linear combinations,
as required to construct the tensor space itself.

## Preservation and validation

Only Chapters 10, 11, 12 and Appendix B changed among the manuscript chapter
files relative to the 3.5.0 snapshot. Chapters 1–9 and 13, Appendix A, preface,
and references are unchanged. README, OUTLINE and version metadata were updated.

Automated comparisons confirm that the main determinant construction and laws,
permutation-sign proof, basis-estimate continuity proof, geometric factorization,
directional-derivative proof, Arzelà–Ascoli proof, inverse and implicit function
proofs, Schwarz proof, Jordan boundary criterion, Fubini proof, local-volume
comparison, nonlinear change-of-variables proof, and half-space derivative proof
are unchanged. The Chapter 12 linear change-of-variables proof changes only its
cell-index notation. The Tensor–Hom preservation check compares the complete
previous source section, not merely its theorem statements.

The final PDF has **322 pages**, **367 unique labels**, and **387 reference uses**.
`latexmk -pdf -interaction=nonstopmode -halt-on-error main.tex` completes
successfully. The final log has no warnings, undefined references, duplicate
labels, or overfull/underfull boxes. Extracted PDF text contains no unresolved
`??`. Source checks also detect unexpected control characters and excluded scope.

Visual review covers **94 pages**: cover and contents; the row-reduction,
operator-norm and determinant additions; all Chapter 11; the Chapter 12 opening,
coordinate FTC and integration by parts, linear change of variables, and
convergence sections; and all Appendix B. Matrices, dimension annotations,
boxed workflows, diagrams, tables and page transitions were inspected. The
malformed multiplication symbol found in the finite-sum proof was corrected
and its final rendering checked after rebuilding.

</details>

<a id="historical-pedagogy-3.7.0-audit"></a>
<details>
<summary>PEDAGOGY 3.7.0 AUDIT</summary>

# Version 3.7.0 — focused pedagogical revision

Revision date: September 13, 2026. This remains a local revision draft; no Git
tag or release was created. Comparisons use the saved current 3.6.0 source,
not Git HEAD, so earlier local revisions are preserved.

## Changes

- Chapter 8 now develops repeated differentiation, the higher Leibniz rule,
  Taylor-polynomial derivative matching and uniqueness, explicit remainder
  bounds, and Taylor–Peano approximation. It distinguishes fixed-order local
  approximation from equality with an infinite Taylor series. The smooth
  cutoff demonstrates why smoothness does not imply analyticity.
- Chapter 11 computes partials on coordinate slices and explains why their
  values specify only a candidate derivative. A rectangular Jacobian example
  proves differentiability directly by estimating its remainder. The continuous
  example x³/(x²+y²), extended by zero, has partials but no total derivative at
  the origin. Its normalized absolute error on the diagonal is constant;
  the signed quotient changes sign, correcting that detail in the prompt.
- The higher-derivative discussion proceeds from first-partial functions to
  Hessians, component Hessians for vector-valued maps, and general symmetric
  multilinear derivatives. A third-derivative example and a working procedure
  make the coordinate formula concrete. The modest multi-index introduction
  explains analytic coefficients and the infinite Taylor expansion without
  introducing a general power-series theory.
- Chapter 13 recalls symmetry before introducing alternation, and explicitly
  distinguishes the symmetric Hessian D²f from the exterior identity d²f = 0.
- Chapter 12 changes only terminology concerning the Jacobian determinant
  and its absolute value.
- Appendix B takes recursive binary tensor products as its primary finite
  construction. Universality is proved inductively; the direct quotient is
  then compared by maps in both directions. Other parenthesizations, induced
  maps, and finite tensor bases follow from this construction. The binary basis
  theorem supplies the only independent tensor-basis proof. The exterior-map
  descent proof again includes its commuting square, and the exterior algebra
  has a named definition as a finite direct sum.

## Dependencies and preservation

The Appendix B benchmark remains Chapter 8 of the author's current Algebra
notes (`../Algebra/chapters/tensor-products.tex`), with its exterior-algebra
companion. The latest request specifically changes the primary finite-product
presentation to recursive binary construction. Algebra source files were not
edited.

The quotient preparation and binary construction, and the complete Tensor–Hom
section, are unchanged from the saved 3.6.0 source. Appendix B remains about
vector spaces over fields, uses only finite direct sums, and excludes exactness
and restriction or extension of scalars. Finitely many factors need not mean
finite-dimensional factors; basis-dimension claims state their hypotheses.

The recursive universality proof constructs the intermediate linear maps before
using equality on elementary spanning tensors. Comparison maps precede the
derived finite basis theorem. Recursive induced maps occur after binary induced
maps. In the analysis chapters, computational patterns that anticipate later
elementary-function results are marked as forward references. The rectangular
Jacobian example uses a direct estimate; the later continuous-partials theorem
is explicitly identified when anticipated. Taylor and symmetry references
connect Chapters 8, 11, and 13. The analytic paragraph does not infer analytic
inverse-function regularity from the smooth theorem.

Chapters 1–7, 9, and 10, Appendix A, the preface, and references are unchanged.
Source comparisons also preserve the existing proofs of the one-variable
Taylor theorem, smooth cutoff, power-series differentiation, inverse and
implicit function theorems, Schwarz symmetry, directional derivative result,
finite-dimensional Arzelà–Ascoli theorem, second-order chain rule, segment
Taylor theorem, Jordan boundary criterion, change of variables, local volume
comparison, half-space derivative lemma, and Riemann–Fubini theorem. Chapter
13's entire text after “One form through all its types,” including the manifold
and general Stokes machinery, is unchanged.

## Validation

- Standard pdfLaTeX/latexmk build: 326 pages.
- Source checks: 380 unique labels and 402 reference uses, with references
  resolved, checked environment pairs balanced, and no unexpected control
  characters.
- Final LaTeX log: no warnings, undefined references, or overfull/underfull boxes.
- Extracted PDF text: no unresolved `??`.
- Visual inspection: 74 selected pages covering the cover and contents, the
  edited passages in Chapters 8, 11, 12, and 13, and the complete Appendix B.
  Taylor displays, higher-derivative arrays, multi-index formulas, tensor maps,
  quotient diagrams, and page breaks were reviewed. Unedited downstream pages
  affected only by pagination were not individually reviewed.
- Version metadata, README, and outline updated to describe this revision.

Reproducible local evidence is in `tmp/qa344.py`, `tmp/qa344/audit.json`,
`tmp/qa344/compiled-text.txt`, chapter comparison files and rendered page images
under `tmp/qa344`, and `tmp/build-344-final.txt`.

</details>

<a id="historical-pedagogy-3.8.0-audit"></a>
<details>
<summary>PEDAGOGY 3.8.0 AUDIT</summary>

# Version 3.8.0 — covectors, coordinate differentials, and calculus bridges

Revision date: September 13, 2026. Source of truth: the current Version 3.7.0
manuscript, saved under `tmp/revision-345-baseline` before editing. Earlier
local revisions were preserved; Git HEAD was not used as the baseline. This
is a revision draft, with no Git tag or release.

## Focused changes

Chapter 10 now has a named definition of covectors and the dual space, with
the vector/covector/scalar type distinction. The dual-basis expansion,
nonstandard-basis example, row-versus-column interpretation, inner-product
dependence of the representing gradient, and covector pullback are retained.
The earlier linear-map-space discussion points forward to the named
definition. Exercises use standard dual-basis notation until Chapter 11
explains coordinate differentials.

Chapter 11 defines polar coordinates before the first radial substitution in
the limit examples. It explains coordinate curves, nonuniqueness, the origin,
and the need for estimates uniform in the angle. After partial derivatives,
the polar Jacobian gives perpendicular columns of lengths 1 and r, preparing
the rigorous area factor and the parameter-order comparison in Chapter 12.

The Jacobian is now defined whenever all scalar partial derivatives exist;
total differentiability separately identifies it as the derivative's matrix.
The early derivative example explicitly points forward to this definition.
The existing candidate-versus-justification workflow and counterexamples remain.

Coordinate projections now supply the definition of dx_i as their Fréchet
derivatives. Their independence of the base point explains the identification
with the standard dual basis. The scalar differential df is the same derivative
viewed as a covector, and its partial derivatives are its dual-basis coordinates.
The one-variable explanation interprets f′ as a coefficient relative to dx,
without treating differentials as infinitesimal real numbers or ordinary fractions.

The curve discussion follows the Euclidean gradient interpretation. It defines
coordinate velocity, derives the curve chain rule from the existing chain rule,
shows the input-to-output velocity map, and evaluates df on velocity. One
calculation reuses the level-ellipse function. The level-set argument now
explicitly places tangent velocities in the kernel of the derivative covector.

Chapter 13 adds a compact parametrization prelude and recalls the curve chain
rule. Ordinary covectors and coordinate differentials are recalled before
k-covectors. Wedge evaluation is displayed as a coordinate minor determinant,
with repeated rows, repeated inputs, and orientation changes distinguished.
The form discussion separates fixed coordinate basis covectors from varying
scalar coefficients and warns that a general 1-form need not be one global df.
Coordinate pullback is expanded into Jacobian rows, then specialized to curves.
The top-degree pullback identity is derived by evaluation and determinant
multiplicativity, as an interpretation of the Chapter 12 theorem.

Chapter 9 adds a bound-variable notation remark after the Riemann-integral
definition. Chapters 12 and 13 distinguish unsigned scalar integration notation
from oriented top forms, including absolute versus signed determinants.

## Local corrections and scope

- Chapter 8's repeated-input kth derivative becomes the kth Taylor term only
  after division by k!.
- The analytic-series paragraph displays the smaller-box derivative majorant,
  handles the zero-order convention and vanishing derivatives, and explicitly
  applies the M-test before successive termwise differentiation.
- The D²f versus d²f comparison now assumes a smooth scalar function, matching
  the chapter's exterior-derivative convention. Its polynomial example remains.
- The scalar surface-area factor is a_Phi; J_Phi is reserved for a matrix.
- Appendix B changes only one `Needspace` instruction to keep the recursive
  space and tuple-map definitions together. Its entire mathematical text,
  recursive finite-product structure, and full Tensor–Hom coverage are unchanged.
  Its vector-space scope, finite direct sums, and exclusions of exactness and
  restriction or extension of scalars remain intact.

No new bundle, connection, curvature, infinite-tensor, low-regularity exterior
calculus, or general power-series theory was introduced. The existing chapter
and section architecture is retained; new discussions use local definitions,
examples, and unnumbered headings.

## Definition order and conceptual continuity

| Object or mechanism | Introduction and subsequent use |
| --- | --- |
| Covector and dual space | Named Chapter 10 definition; chapter-opening mentions are previews. The earlier linear-map discussion explicitly refers forward. |
| Dual basis | Defined by evaluation on basis vectors; superscripts are labels, not powers. |
| dx_i | Mentioned only as forthcoming notation in Chapter 10; rigorously defined through coordinate projections in Chapter 11 before substantive use. |
| df | Chapter 11 identifies it with the scalar Fréchet derivative and expands it in dx_i; Chapter 13 recalls that identification. |
| Polar coordinates | Defined before the first Chapter 11 polar limit substitution; the Jacobian example explicitly marks its use of the continuous-partials theorem as forward. |
| Parametrized curve | Defined in Chapter 11 before its derivative mechanism and level-set use; Chapter 13 recalls it before the practical examples. |
| Pullback | Linear covector pullback is defined in Chapter 10. Curve and integration previews are marked; Chapter 13 defines form pullback and derives the coordinate identities. |
| k-covector and wedge | Chapter 13 recalls ordinary covectors, defines alternating k-linear maps, and then defines elementary wedges by determinants. Earlier wedge mentions are previews. |
| Integration | Chapter 9 remains a Darboux construction; Chapter 12 proves scalar change of variables; Chapter 13 interprets oriented forms using those results. |

The resulting progression is vector → covector → coordinate differential →
scalar differential → gradient representation → evaluation on curve velocity →
alternating covectors and forms → pullback → signed determinant and oriented
integration. The two roles of the polar map connect the limit and derivative
calculations to the later integral theorem.

## Preservation and validation

Final results: 330 PDF pages, 388 unique labels, 418 reference uses, no LaTeX
warnings, no overfull/underfull boxes, and no unresolved `??`. Visual review
covers 54 pages selected through source mapping and front-matter checks.

Automated comparison verifies that all 345 existing proof bodies remain
verbatim. The new curve-chain-rule proof is an addition. Chapters 1–7, Appendix
A, the preface, and references are unchanged. Chapter 13's entire text from
“Integration over an open set” onward is unchanged, preserving the manifold
and general Stokes machinery. Appendix B's sole difference is the layout hint.

The standard pdfLaTeX/latexmk build uses SyncTeX for source-to-page mapping.
Source checks cover unique labels, reference targets, environment pairs,
control characters, proof preservation, and the local scope restrictions.
The extracted PDF is checked for unresolved `??`. Visual review covers the
pages mapped from edited source passages, with surrounding paragraph context,
plus the cover and contents. It includes the new dual-basis discussion,
coordinate-differential formulas, curve type flow, polar Jacobian, majorant,
wedge determinants, pullbacks, integration notation, and Appendix B page break.

Local evidence: `tmp/qa345.py`, `tmp/qa345/audit.json`, chapter comparison files,
extracted PDF text and rendered images under `tmp/qa345`, and
`tmp/build-345-final.txt`. README, outline, and version metadata describe 3.4.5.

</details>

<a id="historical-pedagogy-3.9.0-audit"></a>
<details>
<summary>PEDAGOGY 3.9.0 AUDIT</summary>

# Version 3.9.0 — first-use and dependency cleanup

Revision date: September 14, 2026. The source of truth is the current 3.8.0
manuscript, saved in `tmp/revision-346-baseline` before editing. Existing local
changes were preserved. No Git tag or release was created.

## Changes and progression

Chapter 8 now introduces parametrized plane curves after the trigonometric
functions, inverses, and unit-circle discussion. Coordinate functions give
position, coordinatewise derivatives give velocity, and the square root of
the sum of the two squared derivatives gives speed. The short examples cover
graphs, segments, circles, ellipses, and the difference between image and
traversal. Polar coordinates arise from radius times the unit-circle point;
the text explains nonuniqueness, quadrant selection, and one polar curve.
The polar-motion proposition derives both velocity components and the speed
formula by ordinary product and chain rules, explicitly cancelling cross terms.
No formal vector-space, normed-space, Jacobian, or form machinery enters this
new Part I subsection.

Chapter 9 translates integration-by-parts shorthand into ordinary derivatives
at its first shorthand computation. The logarithm example now explains why
choosing dv = dx means choosing v′ = 1. The substitution preview distinguishes
signed derivative factors from the absolute determinant used for scalar volume.

Chapter 10 collects the coordinate 1-, 2-, 3-, 4-, general finite-p, and maximum
formulas immediately after the norm definition. It verifies the three norms
used later using scalar inequalities and the already proved Euclidean
Cauchy–Schwarz argument. Minkowski's general p-norm triangle inequality is
explicitly unproved and unused. The useful comparisons, function sup-norm
connection, abstract-space conventions, and default Euclidean norm are stated.
An early operator-norm example is phrased directly in terms of a scalar linear
functional instead of anticipating gradient notation.

Chapter 11 recalls Chapter 8's polar geometry for uniform angular limit
estimates. In Section 11.2 the order is coordinate differentials, a concrete
df evaluation and finite-change comparison, the named Euclidean gradient,
recalled curves, the curve chain rule, and the level-set kernel/normal
interpretation. The curve discussion directly combines coordinate remainders;
it does not rely on the componentwise-differentiability proposition that now
comes later. The polar Jacobian explicitly identifies the radial and angular
contributions already computed in Chapter 8.

Section 11.3 keeps higher derivatives, Hessians, and Taylor theory together.
It contrasts the fixed linear map h ↦ Df(a)h with the derivative-valued map
x ↦ Df(x), gives their types, and uses linear f and f(x) = x² to expose the
different variable roles. A bounded bilinear differentiation proposition proves
the remainder estimate before the second-order chain rule uses evaluation.
The curved-path corollary includes acceleration; the unit-circle example
shows its cancellation with the Hessian term. Two new exercises cover df and
the curve chain rule, and polar conversion with quadrant selection.

Chapter 13 recalls the earlier curve material, distinguishes arc length from
linear coordinate covectors, and compares the integrals of dx and ds on a
circle. It adds an integrated polar pullback calculation: coordinate forms,
their wedge, and the running circulation form. A short consequence of d² = 0
makes the warning about general 1-forms concrete. The differential-of-a-function
proposition now cites Chapter 11 instead of repeating the basis calculation.
Early Euclidean tangent notation is replaced by a based displacement vector;
the cotangent space is named after tangent spaces are constructed; and the
intrinsic differential identifies du^i with the differential of the chart's
coordinate function.

## First-use and dependency audit

| Item | Location and dependency check |
| --- | --- |
| Parametrized curve, velocity, speed | Named elementary definition in Chapter 8. The preceding unit-circle paragraph is geometric motivation using its explicit coordinate derivative. Chapter 11 recalls and interprets this; Chapter 13 adds integration regularity conventions. |
| Polar coordinates | Defined in Chapter 8 after trigonometry and inverse functions, including radius, angle, and nonuniqueness. Chapter 11 now has a recall paragraph, not a competing first definition. |
| Euclidean norm | The coordinate length and its Cauchy–Schwarz proof already occur in early Chapter 10 metric geometry. The formal norm discussion subsequently verifies and names it as a norm. |
| p-norm and maximum norm | Formulas collected after the general norm definition. General Minkowski is explicitly excluded from the proof dependencies. |
| Default norm | Named convention in Chapter 10, referenced at the opening of Chapter 11. Abstract norms remain specified; source/target and operator norms retain their distinct roles. |
| Covector, dx_i, df | Chapter 10's covector definition and Chapter 11's coordinate-projection construction are preserved. The new numerical example follows the coordinate expansion. |
| Gradient | Its named definition is now in Section 11.2 before the curve formula or total-derivative workflow uses it. Chapter 10's dual-space discussion remains a preview of its inner-product representation. |
| D²f | Recursive definition explicitly gives f: U ⊂ V → W; the immediate clarification distinguishes the moving base point from a fixed-map increment. Linear and quadratic examples retain independent slots. |
| Bilinear differentiation | Proved before the second-order chain-rule proof invokes evaluation. The product-space remainder estimate and composed-function version are included. |
| Tangent space | The manifold introduction previews it; the actual chart-equivalence construction remains unchanged. Earlier Euclidean evaluations use vectors in R^n based at a point. |
| Cotangent space | Defined as the dual of the constructed tangent space before its first notation use in form values. No cotangent bundle is constructed. |
| Differential form and pullback | Existing definitions and rules are preserved. The polar example follows the pullback composition/wedge rules. The non-potential example follows d² = 0. |
| ds | Defined through scalar line integration and promptly distinguished from linear coordinate differentials through reversal behavior and the circle calculation. |

The three remaining Euclidean 2-norm subscripts in Chapters 11–13 are deliberate:
the Chapter 11 convention reminder, the coordinate/Euclidean length comparison
at its opening, and the Euclidean/maximum comparison in Chapter 12's local
volume lemma. Chapter 13 needs no remaining explicit Euclidean 2-norm subscript.
Other subscripts such as vector components and named Euclidean balls are not
norm subscripts and were not changed.

## Preservation

Appendix B is byte-for-byte unchanged, including its recursive finite tensor
construction, direct comparison, parenthesizations, induced maps, bases,
exterior constructions, and full Tensor–Hom treatment. Its existing vector-space
scope and exclusions remain intact. Chapters 1–7, Appendix A, preface, and
references are unchanged.

Of the 346 proof bodies in the 3.8.0 baseline, 344 are preserved after allowing
only the requested Euclidean-norm subscript simplifications. Two are deliberately
revised: the second-order chain-rule proof cites the newly proved bilinear rule,
and the Chapter 13 differential formula cites its Chapter 11 construction.
The inverse/implicit, Jordan/change-of-variables, partition-of-unity, and general
Stokes arguments are preserved. Chapter 13's entire text from the partitions
of unity and integration section onward is unchanged apart from the norm
subscript in the existing bump formula.

## Validation

The final PDF has 337 pages. All checks pass for 399 unique labels and 432
reference uses, with no unresolved references, LaTeX warnings, or
overfull/underfull boxes. All 63 selected pages were visually reviewed. After
the final coordinate-remainder explanation replaced a forward dependency in
the curve definition, the checks were rerun and the sole changed rendered
page (PDF page 181) was reviewed again.

The standard pdfLaTeX/latexmk workflow builds with SyncTeX for source-to-page
mapping. Checks verify label uniqueness, reference targets, balanced checked
environments, control characters, proof preservation, unchanged Appendix B,
first-use ordering, and the remaining norm subscripts. The extracted PDF is
searched for unresolved `??`.

Visual review uses pages mapped from edited source passages with surrounding
paragraph context, plus cover and contents. It covers the curve/polar displays,
standard norms, moved first-order material, higher-derivative type distinction,
bilinear remainder, curved-path example, cotangent definition, and polar
pullbacks. Unedited pages affected only by pagination are not individually
reviewed.

Local evidence is in `tmp/qa346.py`, `tmp/qa346/audit.json`, extracted text,
source comparisons and rendered pages under `tmp/qa346`, and
`tmp/build-346-final.txt`. Version metadata, README, and outline describe 3.4.6.

</details>

<a id="historical-pedagogy-3.10.0-audit"></a>
<details>
<summary>PEDAGOGY 3.10.0 AUDIT</summary>

# Version 3.10.0 pedagogical audit

September 14, 2026. Baseline: the current Version 3.9.0 manuscript, preserved
before editing. This remains a local revision draft; no Git tag or release
was created.

## Subsequent global numbering update

Theorem-style environments now share section-based numbering (for example,
Theorem 4.2.1); subsections are unnumbered, with their existing contents
entries retained. All 15 chapters/appendices have an unnumbered Exercises
heading. Exercises use an independent integer counter reset by chapter,
including exercises embedded earlier in that chapter. Subsection references
use linked titles rather than inherited section numbers.

The rebuild remains 343 pages and has no warnings, overfull/underfull boxes,
or unresolved `??`. Checked section-number resets in the main text and
appendices, 63 unnumbered subsection entries in the contents, and all 15
unnumbered exercise headings. Reviewed 34 representative rendered pages,
including the contents, numbered statements, title references, exercise
resets, and the five paragraphs affected by longer labels. The pedagogical
audit below records the preceding revision pass; this later change adjusts
numbering, cross-reference presentation, and line breaking, not mathematics.

## Coverage and counting

Reviewed **192 section/subsection openings** and revised **31**. Also reviewed
all 15 chapter/appendix openings, retaining them; where a chapter proceeds
directly into its first section, the pair was assessed together. The two
front-matter openings were separately reviewed and retained. Exercise headings
are included in the 192-heading inventory, with no extra prose required.

The formal-statement pass covered 513 definition, theorem, lemma, proposition,
and corollary environments. The proof pass covered all **349 existing proof
bodies**. **12 were expanded; 337 are byte-for-byte unchanged** relative to
3.4.6. No proof environment was added or removed. These counts distinguish
actual proof-body edits from introductions, examples, and explanations placed
outside proofs.

| Chapter or appendix | Section/subsection openings reviewed | Revised | Proofs reviewed | Expanded |
|---|---:|---:|---:|---:|
| Chapter 1 | 6 | 0 | 0 | 0 |
| Chapter 2 | 8 | 2 | 13 | 0 |
| Chapter 3 | 7 | 0 | 26 | 0 |
| Chapter 4 | 7 | 1 | 14 | 1 |
| Chapter 5 | 7 | 0 | 17 | 0 |
| Chapter 6 | 6 | 0 | 8 | 0 |
| Chapter 7 | 6 | 0 | 19 | 2 |
| Chapter 8 | 10 | 3 | 28 | 3 |
| Chapter 9 | 10 | 1 | 31 | 3 |
| Chapter 10 | 35 | 6 | 51 | 1 |
| Chapter 11 | 12 | 4 | 34 | 0 |
| Chapter 12 | 15 | 1 | 32 | 2 |
| Chapter 13 | 27 | 3 | 35 | 0 |
| Appendix A | 8 | 2 | 5 | 0 |
| Appendix B | 28 | 8 | 36 | 0 |

## Expanded proof mechanisms

1. Chapter 4, limit algebra: fix a positive bound before selecting product
   tolerances; isolate the denominator from zero and choose explicit quotient
   tolerances, including zero coefficients.
2. Chapter 7, limit comparison: use error L/2 to obtain two fixed positive
   multiples; explain the two comparison directions and finite initial terms.
3. Chapter 7, alternating series: display the parity differences, bound both
   subsequences, identify their common limit, and recover convergence of the
   full sequence with one stage.
4. Chapter 8, higher product rule: differentiate into two finite sums,
   reindex the first, combine interior coefficients with Pascal's identity,
   and account for the two endpoint terms.
5. Chapter 8, power-series differentiation: bound n q^(n−1) and display the
   summable, input-independent majorant for the derivative series.
6. Chapter 8, trigonometric addition identities: display the derivative of
   the conserved sum of squares and the cancelling terms.
7. Chapter 9, fine-mesh converse: approximate the supremum/infimum by tags,
   show the finite error η(b−a), and hold the partition fixed as η decreases.
8. Chapter 9, Newton–Leibniz: identify the MVT-generated tagged sum exactly,
   then apply the every-tag fine-mesh theorem to equal subdivisions.
9. Chapter 9, improper comparison: use a supremum argument for the real
   endpoint rather than silently treating it as a sequence index.
10. Chapter 10, equivalent norms: normalize a nonzero vector, combine the
    two Euclidean comparisons explicitly, and give the ball inclusions and
    sequence estimates underlying the topological conclusions.
11. Chapter 12, continuous Fubini: keep consistent product tags, group one
    finite sum, bound the inner-sum error, and explicitly bound the outer
    Darboux gap on that same grid before combining three errors.
12. Chapter 12, Jordan boundary criterion: identify the two relatively open
    pieces of a boundary-free cell, then use convexity and connectedness to
    force its indicator to be constant.

The ratio and root **limit versions** additionally explain the intermediate
choice ρ < r < 1 and the resulting eventual geometric estimate. Those new
paragraphs follow the existing proofs, so they are not counted as expanded
proof bodies.

## First encounters, examples, and consolidation

The revised openings introduce the question before the formal object:
repeated differentiation versus an evaluated number, convexity and slope,
contractions as a solver, inverse versus implicit unknowns, finite direct
sums, operator norms, permutation signs, local integration, and the
Appendix B transitions. The existing geometric motivation for alternating
forms already explains linearity, orientation, and degeneracy and was retained.

Additional statement motivation explains tail bounds for limsup/liminf,
open versus closed sets, the compact-interval hypotheses in the extreme-value
theorem, nonzero inverse slope, and local oscillation.

The analytic definition and its regularity/reconstruction discussion now
open the smooth-cutoff section **after** elementary curves and polar motion
at the end of the trigonometric section. The opening asks whether all Taylor
coefficients reconstruct a function; the subsequent discussion separates
fixed-order approximation from an infinite-series assertion.

Three small additions address exposed hypothesis failures: a smooth curve
whose nonnegative polar radius fails to be differentiable at the origin;
an integrable function supported on a face with a nonintegrable section;
and disjoint smooth bumps approaching zero whose pointwise finite sum is
discontinuous. The last example makes the whole-neighborhood requirement
of local finiteness concrete.

Nearby repetition was consolidated in the sequence opening, choice
discussion, higher-derivative discussion, analytic discussion, general
Stokes opening, and Appendix B's scalar-unit and symmetry passages.
No unrelated application or optional theory was added.

## Preservation and dependency checks

- All 26 Chapter 3 proof bodies and the real-number construction are
  unchanged. The completeness and uniqueness architecture is retained.
- Bernstein and Arzelà–Ascoli proofs, the determinant construction and
  expansion, and the higher-derivative type development are retained.
- Every Chapter 11 proof is unchanged, including bilinear differentiation,
  inverse and implicit functions. The full nonlinear change-of-variables
  proof and its supporting construction are unchanged.
- Every Chapter 13 proof is unchanged, including tangent-space construction,
  coordinate independence, refinement-based partition of unity, integral
  well-definedness, and general Stokes.
- All 36 Appendix B proofs are unchanged. Recursive tensors, exterior
  multiplication, Tensor–Hom currying and its full proof, the finite-dimensional
  tensor–map identification, and compatibility discussions retain their depth.
  Appendix B remains about vector spaces over a field, with finite direct
  sums only and no exactness or restriction/extension of scalars.
- New proofs use the stated hypotheses: no extra continuity is imposed on
  the fine-mesh, Newton–Leibniz, or improper-comparison statements; the Jordan
  argument does not assume the bounded set is closed; Fubini uses the existing
  positive-volume rectangle convention. The higher product rule uses only
  the derivative orders needed at the induction step.
- New explanatory references resolve to previously established results.
  The root/ratio explanation precedes its use in power-series differentiation;
  the curve warning needs only one-variable calculus; the face example follows
  null modification; the bump example uses the earlier smooth cutoff.
- Newly introduced shortcuts were checked: the reversed Fubini order is
  justified by explicitly exchanging the two factors; compactness uses the
  already proved compact sphere or compact rectangle results; equality of
  integrals follows the displayed error bounds, not an unexplained exchange
  of limits. No new unqualified “clearly” or “taking limits” step is used.

## Build and visual checks

Normal `latexmk -pdf -synctex=1 -interaction=nonstopmode -halt-on-error main.tex`
build: **343 pages**, **399 unique labels**, **434 reference uses**. The final
log has no LaTeX warnings, undefined references, duplicate-label warnings,
or overfull/underfull boxes. Extracted PDF text contains no unresolved `??`.
Source environment counts balance and no accidental control characters occur.

Visual review covers the cover and contents plus every page containing edited
source passages and surrounding context, selected by SyncTeX mapping of the
baseline diff. This is 89 pages, reviewed as rendered page sheets, with closer
inspection of the longer proof displays and their page transitions. Page
numbers below are physical PDF pages. Purely shifted pagination of unchanged
passages is not counted as a source edit.

1, 2, 3, 4, 5, 6, 22, 23, 24, 39, 40, 42, 43, 44, 45, 53, 54, 57, 58, 69, 70, 76, 77, 78, 87, 88, 89, 90, 92, 93, 96, 97, 98, 99, 100, 108, 109, 117, 118, 119, 120, 121, 132, 133, 135, 136, 137, 144, 145, 146, 157, 158, 159, 162, 163, 174, 175, 176, 199, 200, 201, 222, 223, 225, 226, 229, 230, 276, 277, 289, 290, 294, 295, 296, 308, 309, 310, 319, 320, 322, 323, 324, 327, 331, 332, 335, 336, 337, 338.

## Complete opening inventory

“Retained” means the existing introduction, concrete example, or immediately
following subordinate opening supplies the needed purpose; an exercise block
does not require a new motivational paragraph. Chapter numbers refer to the
main text; A and B are appendices.

| Location | Level | Opening | Decision |
|---|---|---|---|
| 1 | chapter | Motivation and the Transition from Calculus to Analysis | Retained |
| 1 | section | Why Calculus Needs Foundations | Retained |
| 1 | section | A First Look at Limits | Retained |
| 1 | section | The Structural Ideas of Analysis | Retained |
| 1 | section | Warnings That Motivate Hypotheses | Retained |
| 1 | section | Road Map | Retained |
| 1 | section | Exercises | Retained |
| 2 | chapter | Basic Set Theory, Logic, Functions, and Relations | Retained |
| 2 | section | Sets | Retained |
| 2 | section | Logic and Proofs | Retained |
| 2 | subsection | Writing Proofs | Retained |
| 2 | section | Relations and Functions | Retained |
| 2 | section | The Natural Numbers, Integers, and Rational Numbers | Retained |
| 2 | section | Countability | Revised |
| 2 | section | Choice | Revised |
| 2 | section | Exercises | Retained |
| 3 | chapter | The Real Number System | Retained |
| 3 | section | Ordered Fields and the Problem to Be Solved | Retained |
| 3 | section | Rational Numbers, Completeness, and Uniqueness | Retained |
| 3 | section | Cauchy Sequences of Rational Numbers | Retained |
| 3 | subsection | The construction in one picture | Retained |
| 3 | section | Order and Completeness | Retained |
| 3 | section | A Small Toolkit of Inequalities | Retained |
| 3 | section | Exercises | Retained |
| 4 | chapter | Sequences of Real Numbers | Retained |
| 4 | section | Convergence | Revised |
| 4 | subsection | Decimals are limits, not new numbers | Retained |
| 4 | section | Algebra and Order of Limits | Retained |
| 4 | section | Subsequences and Elementary Divergence | Retained |
| 4 | section | Completeness Consequences | Retained |
| 4 | section | Equivalent Completeness Principles | Retained |
| 4 | section | Exercises | Retained |
| 5 | chapter | Limits and Continuity of Functions | Retained |
| 5 | section | Limits at a Point | Retained |
| 5 | section | Asymptotic Notation | Retained |
| 5 | section | Continuity | Retained |
| 5 | section | Uniform Continuity | Retained |
| 5 | section | Intermediate Values | Retained |
| 5 | section | Compact Intervals | Retained |
| 5 | section | Exercises | Retained |
| 6 | chapter | Sequences and Families of Functions | Retained |
| 6 | section | Pointwise and Uniform Convergence | Retained |
| 6 | section | Continuous Limits | Retained |
| 6 | section | Polynomial Approximation | Retained |
| 6 | subsection | Reading the Bernstein weights | Retained |
| 6 | section | Equicontinuity | Retained |
| 6 | section | Exercises | Retained |
| 7 | chapter | Infinite Series | Retained |
| 7 | section | Series, Partial Sums, and the Cauchy Criterion | Retained |
| 7 | section | Nonnegative Series and Comparison | Retained |
| 7 | section | Absolute Convergence and Products | Retained |
| 7 | section | Ratio, Root, and Alternating Tests | Retained |
| 7 | section | Power Series | Retained |
| 7 | section | Exercises | Retained |
| 8 | chapter | Differentiation | Retained |
| 8 | section | Derivative and Differentiability | Retained |
| 8 | section | Chain Rule and Mean Value Theorems | Retained |
| 8 | section | Definitions of Elementary Functions | Retained |
| 8 | section | Differentiating Limits and Power Series | Retained |
| 8 | subsection | Repeated differentiation and Taylor polynomials | Revised |
| 8 | section | The Standard Elementary Functions | Retained |
| 8 | subsection | Parametrized Curves and Polar Coordinates | Retained |
| 8 | section | A Smooth Cutoff and the Limits of Taylor Series | Revised |
| 8 | section | Convexity and a Continuous Nondifferentiable Example | Revised |
| 8 | section | Exercises | Retained |
| 9 | chapter | Riemann Integration and the Fundamental Theorem of Calculus | Retained |
| 9 | section | Partitions and Riemann Sums | Retained |
| 9 | section | Continuous Functions Are Integrable | Retained |
| 9 | subsection | Tagged sums: the calculus meaning of the integral | Revised |
| 9 | section | Uniform Limits and Integration | Retained |
| 9 | subsection | Pointwise bounded convergence requires a different argument | Retained |
| 9 | section | The Fundamental Theorem of Calculus | Retained |
| 9 | section | Improper Integrals | Retained |
| 9 | section | The Lebesgue Criterion for Riemann Integrability | Retained |
| 9 | section | Limits of the Riemann Theory | Retained |
| 9 | section | Exercises | Retained |
| 10 | chapter | Topology and Linear Algebra | Retained |
| 10 | section | Distances, Balls, and Neighborhoods | Retained |
| 10 | section | Open and Closed Sets in an Ambient Space | Retained |
| 10 | subsection | Subspaces: change the universe before testing openness | Retained |
| 10 | subsection | Interior, closure, and boundary | Retained |
| 10 | section | Convergence, Completeness, and Metric Continuity | Revised |
| 10 | section | Topological Spaces and Finite Products | Retained |
| 10 | subsection | Why rectangles suffice | Retained |
| 10 | section | Compactness: From Local Pieces to Global Control | Retained |
| 10 | section | Sequential Compactness, Finite Nets, and a Common Scale | Revised |
| 10 | section | Connectedness and Paths | Retained |
| 10 | section | Vector Spaces, Bases, and Dimension | Retained |
| 10 | subsection | What can be added and rescaled? | Retained |
| 10 | subsection | Subspaces | Retained |
| 10 | subsection | Linear combinations and span | Retained |
| 10 | subsection | Independence means no redundancy | Retained |
| 10 | subsection | Coordinates: existence and uniqueness | Retained |
| 10 | subsection | Why dimension is a theorem before it is a number | Retained |
| 10 | section | Finite Direct Sums | Retained |
| 10 | subsection | External sums: keep the components in separate positions | Revised |
| 10 | subsection | Internal sums: uniqueness is an extra requirement | Revised |
| 10 | section | Linear Transformations, Kernels, and Images | Retained |
| 10 | section | Matrices as Coordinate Representations | Retained |
| 10 | section | Matrix Multiplication Comes from Composition | Retained |
| 10 | subsection | Solving Linear Systems and Row Reduction | Retained |
| 10 | section | Changing Coordinates while Keeping the Map | Retained |
| 10 | section | Inner Products and Norms | Retained |
| 10 | section | Operator Norms and Finite-Dimensional Estimates | Revised |
| 10 | subsection | Series of vectors and operators | Retained |
| 10 | section | Dual Spaces and Multilinear Maps | Retained |
| 10 | section | Determinants and Orientation | Retained |
| 10 | subsection | The permutation signs needed here | Revised |
| 10 | subsection | The coordinate formula follows from the structure | Retained |
| 10 | subsection | Minors, cofactors, and efficient computation | Retained |
| 10 | section | Perspective and Transition | Retained |
| 10 | section | Exercises | Retained |
| 11 | chapter | Differentiation in Finite-Dimensional Spaces | Retained |
| 11 | section | Limits, Continuity, and Families of Maps | Retained |
| 11 | subsection | Limits and continuity in finite dimensions | Retained |
| 11 | subsection | Pointwise and uniform convergence | Revised |
| 11 | subsection | Equicontinuity and compactness of families | Revised |
| 11 | section | Differentiability and the Derivative | Retained |
| 11 | section | Higher Derivatives and Local Estimates | Retained |
| 11 | subsection | Convexity and global minima | Retained |
| 11 | section | The Contraction Principle | Revised |
| 11 | section | Inverse and Implicit Functions | Revised |
| 11 | subsection | Consequences: Local Coordinates and Regular Level Sets | Retained |
| 11 | section | Exercises | Retained |
| 11 | section | Perspective and Transition | Retained |
| 12 | chapter | Multivariable Riemann Integration | Retained |
| 12 | section | Rectangles, Partitions, and Darboux Sums | Retained |
| 12 | subsection | Rectangular restriction, gluing, and translation | Retained |
| 12 | section | Iterated Integration | Retained |
| 12 | section | Jordan Sets and Integration over Bounded Regions | Retained |
| 12 | subsection | Simple planar regions and changing the order | Revised |
| 12 | subsection | Volumes in three dimensions by cross-sections | Retained |
| 12 | section | Linear Changes of Variables | Retained |
| 12 | section | Nonlinear Changes of Variables | Retained |
| 12 | subsection | Alternative Viewpoint: Pullbacks and Manifold Integration | Retained |
| 12 | subsection | Worked changes of variables | Retained |
| 12 | section | Convergence and Multiple Integration | Retained |
| 12 | subsection | Arzel\`a bounded convergence on rectangles | Retained |
| 12 | section | Exercises | Retained |
| 12 | section | Strategy for Multiple Integrals: Geometry, Coordinates, and Computation | Retained |
| 12 | section | Limits of the Riemann Theory | Retained |
| 13 | chapter | Differential Forms, Stokes' Theorem, and Calculus on Manifolds | Retained |
| 13 | section | Parametrized Curves and Line Integrals | Retained |
| 13 | subsection | A curve is a traversal, not just a set | Retained |
| 13 | subsection | Computing line integrals | Retained |
| 13 | section | Green's Theorem in the Plane | Retained |
| 13 | section | Parametrized Surfaces and Surface Integrals | Retained |
| 13 | subsection | A small parameter rectangle becomes a tangent parallelogram | Retained |
| 13 | subsection | Computing surface area and flux | Retained |
| 13 | section | Classical Stokes for a Parametrized Surface Patch | Retained |
| 13 | section | Beyond One Parametrization: Why Manifolds? | Retained |
| 13 | subsection | Why differential forms are the integrands | Retained |
| 13 | section | Alternating Multilinear Algebra | Retained |
| 13 | section | Differential Forms, Pullbacks, and Exterior Derivatives | Retained |
| 13 | subsection | One form through all its types | Retained |
| 13 | subsection | Pullback as a workflow, including a surface calculation | Retained |
| 13 | section | Integration and the Local Stokes Theorem | Revised |
| 13 | section | Smooth Manifolds, Tangent Spaces, and Orientation | Retained |
| 13 | subsection | Charts undo parametrizations | Retained |
| 13 | subsection | Deriving the tangent-coordinate rule from a moving point | Retained |
| 13 | subsection | The differential: intrinsic map, changing coordinate matrices | Retained |
| 13 | subsection | Pullbacks, wedge products, and exterior derivatives on manifolds | Retained |
| 13 | section | Partitions of Unity and Integration on Manifolds | Retained |
| 13 | subsection | Smooth Euclidean Domains and the Riemann Integral | Revised |
| 13 | section | The General Stokes Theorem | Revised |
| 13 | section | Classical Theorems Revisited | Retained |
| 13 | subsection | Computational practice | Retained |
| 13 | section | Exercises | Retained |
| 13 | section | Perspective and Further Directions | Retained |
| A | chapter | Permutations and Determinants over a Field | Retained |
| A | section | What Survives over an Arbitrary Field? | Retained |
| A | section | Cycles, Transpositions, and Parity | Retained |
| A | subsection | Reading and composing bijections | Retained |
| A | subsection | Following a permutation until it closes | Retained |
| A | subsection | Adjacent swaps and the parity question | Retained |
| A | subsection | Counting inversions instead of choosing swaps | Revised |
| A | subsection | Permutation matrices connect the notation to linear maps | Retained |
| A | section | Constructing the Determinant Form | Revised |
| B | chapter | Tensor Products and Exterior Powers | Retained |
| B | section | Quotient Vector Spaces and Universal Factorization | Retained |
| B | section | Bilinear Maps and Binary Tensor Products | Retained |
| B | subsection | Construction from formal symbols | Retained |
| B | subsection | Spanning is not surjectivity of the input map | Retained |
| B | section | Finite Associativity | Retained |
| B | section | Tensor Products and Finite Direct Sums | Retained |
| B | section | Symmetry over a Field | Revised |
| B | section | Finite Multilinear Tensor Products | Retained |
| B | subsection | Recursive existence from the binary product | Retained |
| B | subsection | The direct quotient realizes the same problem | Retained |
| B | section | Tensoring Linear Maps and Concrete Calculations | Revised |
| B | subsection | Induced maps in all the factors | Retained |
| B | subsection | The scalar unit | Revised |
| B | subsection | Tensor bases and coordinates | Revised |
| B | section | Tensor--Hom Correspondences | Retained |
| B | subsection | A map whose values are maps | Retained |
| B | subsection | A covector and a vector make a linear map | Revised |
| B | subsection | Compatibility with changing the inputs and output | Retained |
| B | section | Exterior Powers | Retained |
| B | subsection | Begin with two inputs | Retained |
| B | subsection | Expand, remove repeats, sort, and collect | Retained |
| B | subsection | Representations need not be unique | Retained |
| B | subsection | Exterior maps, minors, and determinants | Revised |
| B | subsection | Wedge products between exterior powers | Retained |
| B | section | The Exterior Algebra and Alternating Forms | Revised |
| B | subsection | First identification: factor an alternating map | Retained |
| B | subsection | Second identification: pair covector wedges with vector wedges | Revised |
| B | section | Exercises | Retained |

</details>

<a id="historical-pedagogy-3.11.0-audit"></a>
<details>
<summary>PEDAGOGY 3.11.0 AUDIT</summary>

# Version 3.11.0 pedagogical and proof-architecture audit

September 14, 2026. Baseline: Version 3.10.0, preserved before editing in the
session's temporary revision baseline. This is a local revision draft; no Git
tag or release was created.

## Scope and preserved conventions

The revision keeps the chapter architecture and mathematical scope of 3.4.7.
Theorem-style environments remain numbered within sections, subsections remain
unnumbered and listed in the contents, and each unnumbered Exercises section
uses an independent chapter or appendix exercise counter. Appendix B is byte
for byte unchanged, retaining its vector-space setting, finite direct sums,
and full Tensor–Hom correspondence while excluding exactness and restriction
or extension of scalars.

No Banach-space inverse theorem, infinite-dimensional calculus, Faà di Bruno
formula, constant-rank theorem, spectral theory, or manifold interpretation of
`GL(R^n)` was added. The Chapter 12 change-of-variables proof was not rewritten.

## Chapter 10 notation and analytic preparation

The first definition of `L(V,W)` now introduces `L(V):=L(V,V)` and records the
standard-basis identification `L(R^n) ≅ M_n(R)`. Chapter 11 treats
`GL(R^n)` as the open subset of invertible elements of `L(R^n)` and retains
the operator viewpoint even when matrices are mentioned.

The first Euclidean Cauchy–Schwarz proof now explains both strategic choices:
Cauchy–Schwarz is needed to control the cross term in the triangle inequality,
and `t=(x·y)/||y||²` minimizes the displayed nonnegative quadratic
`||x-ty||²`.

## Rebuilt Chapter 11 sequence

Immediately after the contraction mapping theorem, Corollary 11.4.3 traps a
strictly inward Euclidean open-ball contraction inside an invariant complete
closed subball. It proves the fixed-point bound and convergence from every
starting point in the open ball, explicitly explains why the incomplete open
ball cannot itself be fed into the contraction theorem, and records the sharp
boundary example `T(x)=(x+1)/2` on `(-1,1)`.

The perturbation proposition is retained with `A,B ∈ L(R^n)` and the same
geometric-series mechanism. The former adjugate proof of smooth inversion is
replaced by a differential proof on the finite-dimensional normed space
`L(R^n)`. It establishes openness of `GL(R^n)`, local boundedness and
continuity of inversion, the exact resolvent and quadratic-remainder
identities, the typed derivative

`D Inv(A):L(R^n)→L(R^n)`, `D Inv(A)[H]=-A^{-1}HA^{-1}`,

and smoothness by the bilinear composition bootstrap. No second adjugate proof
remains in Chapter 11.

The definition of a `C^k` diffeomorphism, including a local `C^k`
diffeomorphism, now precedes the inverse theorem. The main theorem directly
covers `1≤k≤∞`; its former higher-regularity corollary has been absorbed.
Its proof has seven visible stages:

1. construct `f̃(h)=Df(a)^{-1}(f(a+h)-f(a))` and verify the normalized data;
2. obtain a contraction estimate for `G(x)=x-f̃(x)`;
3. solve every nearby equation with the open-ball corollary;
4. prove injectivity and the quantitative inverse Lipschitz estimate;
5. convert the source remainder into an output remainder and differentiate;
6. bootstrap from the `C^1` core through exactly the derivatives available;
7. undo source translation, target translation, and linear normalization by
   writing the inverse explicitly.

The periodic exponential-polar example now follows the theorem, so its claim
of local invertibility depends only on a result already stated and proved.

The implicit theorem is likewise stated directly for `C^k` data. Its proof
uses `H(x,y)=(x,F(x,y))` to straighten the zero set to
`R^n×{0}`, displays the inverse of the block derivative, applies the `C^k`
inverse theorem, defines the implicit function immediately from `H^{-1}(x,0)`,
and only then shrinks to a product neighborhood and proves graph uniqueness.
Invertibility of nearby `D_yF` is derived from invertibility of `DH` by a
kernel argument in finite dimension. The derivative formula and its source
and target types come last, after the function exists. The former separate
higher-regularity corollary is removed.

## Focused local repairs

- Chapter 3 marks the `n>1/ε` supremum illustration as an explicit preview of
  the later Archimedean theorem.
- Chapter 8 explains subtraction of the secant line before applying Rolle's
  theorem and gives the exponential Cauchy-product calculation once, with
  absolute convergence as its justification.
- Chapter 9 moves the coarse/fine tagged-partition mechanism and diagram after
  the tagged-sum motivation. A `Needspace` guard keeps Theorem 9.3.1 from
  beginning with an isolated statement fragment.
- Chapter 12 moves the polar preview from the opening of Jordan theory to the
  polar change-of-variables example. Its integrable-sections Fubini lemma now
  defines `ℓ_R` and `u_R`, proves the full finite lower/upper-sum chain, and
  states the bound on the outer integrand.
- Chapter 13 calls `df` intrinsic and identifies `df=f'(x)dx` and
  `df=Σ_i ∂_i f dx_i` as coordinate expressions.
- Anthony W. Knapp, *Basic Real Analysis*, first edition, Birkhäuser Boston,
  2005, is added as a supplementary structural reference. Sheldon Axler is
  absent from the manuscript bibliography.

## Validation

Two final `pdflatex` passes complete with a clean log: no LaTeX, package,
undefined-reference, duplicate-label, overfull-box, or underfull-box warning
matches. The final PDF has 342 pages. Source analysis finds 399 labels, all
unique, and every comma-separated reference target resolves. Extracted PDF
text contains no `??`.

The destination audit covers the new open-ball corollary, perturbation
proposition, smooth-inversion lemma, inverse theorem, implicit theorem, and
Theorem 9.3.1. Each named PDF destination resolves to the physical page that
contains the corresponding theorem heading and statement.

Visual review covers every page containing a changed passage in Chapters 3,
8, 9, 10, 11, 12, and 13, plus the revised contents, cover metadata, and
bibliography. The review checks margins, theorem-heading placement, displayed
formula breaks, diagrams, headers and footers, and the continuity of each
multi-page proof. No clipped text, overlap, malformed glyph, stranded theorem
fragment, or other layout defect remains.

</details>

<a id="historical-polish-3.4.1-audit"></a>
<details>
<summary>POLISH 3.4.1 AUDIT</summary>

# Focused finishing audit — Version 3.4.1 (revision draft)

Revision date: September 12, 2026. Local finishing patch to Version 3.4.0.
No Git tag or GitHub release was created.

## Baseline and editorial reference

The actual Version 3.4.0 working-tree manuscript, PDF, and revision metadata
were saved under `tmp/revision-341-baseline/`. Existing uncommitted work and
unused “Copy” files were preserved. The available sibling Algebra Chapter 8
sources were consulted, especially the staged exterior-map construction in
`chapters/exterior-algebra.tex`. The adaptation concerns displays, proof stages,
and explanatory pacing, and retains the analysis appendix's field/vector-space
scope. It does not claim consultation of an unavailable newer remote edition.

## Changes by request

| Request | Implemented change |
|---|---|
| 11: affine-approximation figure | Replaced the nearly edge-on view by a broad oblique TikZ view with distinct orange plane and blue mesh, marked contact, x/y/z direction key, input displacement, and vertical remainder. Preserved exact and numerical remainder calculations; explained quadratic scaling of the error. |
| 11: level-set mechanism | Added the chain-rule derivation from f composed with a level curve being constant to gradient–velocity orthogonality. Retained the directional, ellipse, and hyperbola calculations. |
| 11: circle placement | Moved the circle picture inside the circle implicit-function example, after its equation and local derivative calculation. It no longer visually belongs to the y+sin y=x example. |
| 11: exercises | Consolidated the two headings under one Exercises section, preserving the continuous numbering and every exercise. |
| 12: theorem-driven slices | Defined the horizontal section and its area, then displayed volume as the integral of 1, the iterated section integral, and the integral of section area. Explicitly used the integrable-sections Fubini lemma for zero-extended indicators. |
| 12: cylinder/cone/ball | Displayed domains, section geometry, area functions, integral setup, antiderivatives, endpoint substitution, and interpretation. The cone's linear-radius/quadratic-area mechanism precedes its evaluation. |
| 12: Jordan bookkeeping | Displayed the cylinder and cone parameter maps and applied bounded derivatives/Lipschitz images to their compact parameter rectangles. No cone-apex surface regularity is required. Retained disk/plane and sphere-patch checks. |
| 12: polar and cylindrical logic | Reworded polar area as a second method, preserving central/seam box bounds independent of the known disk area. Displayed the truncated cylindrical source, including z≤h(1−epsilon/R), and bounded its omitted source integral by πh epsilon²+eta hR². |
| 12: Fubini–Tonelli | Specified Lebesgue integration on Euclidean product spaces without adding measure-space formalism or proofs. |
| 12: exercise transfer | Replaced the already-solved normalized quadratic ellipse integrand by x². Preserved coordinate, scaling, and exceptional-set justification requirements. |
| 13: work notation | Corrected the segment-work example to F·dr. |
| 13: surface computations | Added the actual nested cylinder area and flux integrals, their inner evaluations, and the two-injective-patches meaning of the compact angular notation. |
| 13: plane density/flux | Evaluated the scalar surface integral of z, showing the inner antiderivative, and compared it with upward flux of (0,0,z). Distinguished area, weighted area, and flux. |
| 13: exercise/reference | Changed the promoted plane-patch exercise to density x² and field (0,0,y²). Updated the later pullback comparison to refer to the worked flux calculation. |
| 13: classical Stokes layout | Reserved space for the introductory sentence and four-integral comparison table. The manifold preview remains after patch Stokes. |
| B: central maps | Displayed the finite-product input and linear factorization, the parenthesization comparisons and both inverse identities, and the induced exterior map with its defining values, identity, composition, and inverse formulas. |
| B: proof staging | Separated exterior-map Stage 1 (tuples), Stage 2 (tensor map), and Stage 3 (relations and quotient), followed by a distinct shorter-proof paragraph and a distinct identities/composition/inverses paragraph. |
| B: repeated mechanisms | Shortened scalar-unit bilinearity verification while retaining reverse map and both composites. Derived the other-slot distributivity map by the existing symmetry isomorphisms, preserving finite double distributivity. |
| B: parenthesization | Reset block and direct/nested notation; separated induction, first-block factorization, second-block factorization, evaluation, universality, and comparison stages; added a concise concluding explanation. |
| B: local notation | Removed the tab-corrupted S:W→X arrow, reset X in the direct three-factor comparison, and stated the types of the further factor maps S_r. Displayed the determinant identity for arbitrary vector inputs. |

## Preservation and focused audit

Only Chapters 11, 12, 13, and Appendix B differ from the saved baseline chapter
files. All other chapter sources, Appendix A, preface, references, and manuscript
input order are unchanged. The quotient prelude, detailed first tensor construction,
first canonical-isomorphism proof, and first nested associativity proof remain intact.
The exterior basis/minors/nonvanishing/determinant/multiplication/algebra/duality
sequence is unchanged. Chapter 13's covector construction remains independent of
Appendix B. No new theorem scope or overall chapter reorganization was introduced.

All baseline proof bodies in Chapters 11–13 are unchanged: 22, 29, and 35,
respectively. This includes the protected extremum, half-space, boundary,
support/cutoff, partition, common-refinement, manifold–Riemann, and Stokes arguments.
Appendix B changes only the requested proof exposition and local notation.

Exercise counts remain 19 in Chapter 11, 11 in Chapter 12, 29 in Chapter 13,
and 17 in Appendix B. The modified exercises test transfer rather than repeating
the promoted calculations. Existing labels are retained; the source audit verifies
349 distinct labels and 381 reference uses, with no duplicate or missing targets.
It also checks for control-character corruption such as the malformed arrow.

The source/target direction of every substitution remains explicit. The cone's
truncated height bound ensures nonempty radial intervals, and its omitted apex
portion is covered by the r<epsilon source estimate. Unsigned scalar integration
retains absolute Jacobians; work/flux retain orientation. The repeated angular
seam is handled by the two injective surface patches, not treated as global
injectivity. The later polar proof no longer claims disk area is unknown.

## Validation

The requested `latexmk -pdf main.tex` command was run through installed MiKTeX,
with `-interaction=nonstopmode -halt-on-error` diagnostic flags. The stabilized
build produces 307 pages. Its final log has no LaTeX warnings, undefined references,
duplicate labels, or overfull/underfull boxes. MiKTeX's launcher emits a harmless
Perl locale fallback, while latexmk completes successfully.

Evidence: `tmp/build-341-final.txt`, `main.log`, and
`tmp/qa341/source-audit.json`. Rendered-page inventory and final visual-review
results are recorded in `tmp/qa341/pages.json` and below.

Visual review covered 79 selected pages in the contact sheets, including the
entire Appendix B and references (PDF pages 279–307), plus the tangent-plane
figure on PDF page 172: 80 distinct pages in total. Reviewed material includes
the worked volume and substitution examples, classical surface calculations,
the manifold transition, and all revised appendix map constructions.
The final circle layout was re-rendered and inspected on PDF pages 186–187:
its equation, diagram, and adjacent explanation now share page 186, and its
labels are separated. The final tangent-plane rendering was also inspected
at full-page size. These final images are `tmp/qa341/circle-final-186.png`,
`tmp/qa341/circle-final-187.png`, and `tmp/qa341/tangent-final.png`.
No clipping, overlapping labels, or separated figure explanations remain in
the reviewed changes. No Git tag or GitHub release was created.

</details>

<a id="historical-proof-architecture-audit"></a>
<details>
<summary>PROOF ARCHITECTURE AUDIT</summary>

> Current revision: Version 3.4.1 (revision draft), September 12, 2026.
> The record below is historical. See [historical validation record](#historical-polish-3.4.1-audit)
> for the focused finishing patch and its validation.

# Major pedagogical and proof-architecture revision

Version 3.0.0 (revision draft), September 12, 2026.

This pass started from the latest local 2.0.0 manuscript, including its
uncommitted revisions. The starting sources and PDF were preserved in
`tmp/pre-architecture-2026-09-12/`; the existing `- Copy` files were not used
as the starting manuscript or overwritten. This is a local review draft.

## Request coverage

The numbers below refer to the numbered sections of the revision request.
Locations use section names rather than obsolete theorem numbers.

| Request | Revised location and mechanism |
|---|---|
| 0–1, 48, 81 | The reading guide identifies construction, existence, uniqueness, and the order of choices as separate tasks. The first-use proofs listed below expose those tasks; later uses can refer to them. The current bibliography is retained. |
| 2–6 | Chapter 10 begins with distances on the line and Euclidean space, illustrated balls, ambient and relative openness, interior/closure/boundary examples, convergence and completeness. Metric continuity precedes topological continuity. Topology and finite-product continuity are developed from inverse images. |
| 3, 11, 24 | Metric, topology, vector-space, linear-map, inner-product, norm, multilinearity, and alternation conditions have displayed formulas. The eight vector-space axioms stay together on one page. |
| 7–8 | Compactness starts with explicit covers and noncompact examples. Separate proofs handle closed subsets, continuous images, and compact subsets of Hausdorff spaces. The finite choices, finite intersection, finite nets, common cover scale, and increasing subsequence indices are visible. |
| 9 | Connectedness is defined through separation; interval/path examples, continuous images, and the path-connected implication have explicit arguments. |
| 10–15 | Coordinate and function-space examples precede abstract vector spaces. Span, independence, and bases are separate. Coordinate and synthesis maps are constructed and composed in both orders before exchange and dimension. A numerical exchange illustrates the abstract replacement step. |
| 16 | The new finite-direct-sums section treats external tuples, injections/projections, internal uniqueness, the summation map, dimension, and the criterion using each subspace against the sum of the others. Three lines in the plane show why pairwise trivial intersections do not suffice. |
| 17–19 | A map from prescribed basis values is constructed before matrices. Kernel, image, rank, and nullity are separated, with worked examples. Rank–nullity has distinct spanning and independence arguments. The inverse of a bijective linear map is proved linear. |
| 20–23 | Matrices come from basis images, including differentiation and rectangular maps. Row and column multiplication are compared numerically. Actual composition precedes the product formula. Coordinate-conversion maps explain change of basis and its diagram. |
| 25–27 | Appendix B starts with cosets, their equality criterion, the equivalence relation, representative-independent operations, the quotient map, universal factorization, and the first isomorphism theorem with explicit inverse. A boxed explanation says what a universal property does. |
| 28–30 | Tensor universality displays the target/map/existence/uniqueness quantifiers. Uniqueness constructs the two comparison maps separately and uses uniqueness twice to prove both composites. A boxed working rule distinguishes constructing a map from comparing existing maps on a spanning set. |
| 31–33 | The formal-symbol construction first extends from a formal basis, then checks all four relation types, then factors through the quotient. Existence and the basis theorem are separate. A quotient argument proves that universality itself forces spanning; the text distinguishes spanning from surjectivity of the elementary-tensor map. |
| 34–37 | The scalar identification, symmetry, induced maps, binary distributivity in either slot, and finite two-sided distributivity have concrete maps. Inverse formulas and both composites are checked after the maps exist. |
| 38–39 | Products of finitely many different spaces are constructed before tensor powers. Coordinate detectors prove the basis formula. Associativity constructs both nested maps in stages and compares them with the directly constructed three-factor product. |
| 40 | Tensor–Hom currying checks the inner linear-map type, outer linearity, reverse bilinear input, and both inverse identities. The finite-dimensional covector–vector identification constructs its inverse using a finite basis sum and explains why it is canonical. |
| 41–43 | The repeated-input subspace R_2 appears before its quotient. General exterior universality separates tensor factorization, relation annihilation, quotient factorization, and the two uniqueness clauses. The exterior-basis proof includes the nine-term three-dimensional expansion and determinant detectors. Induced maps are compared in a quotient square. |
| 44–47 | Exterior multiplication is constructed in two alternating-factorization stages through a space of linear maps. An equality-on-spanning-tuples lemma applies only to existing maps. Associativity, graded signs, graded sums, the two distinct dual identifications, both inverse composites, and the top exterior-power determinant follow. The non-elementary wedge example remains valid in characteristic two. |
| 49–52 | Chapters 2–3 construct both inverse-function identities and uniqueness before inverse formulas, expand representative checks for integers/rationals, construct the reverse ordered-field comparison, and explain the square-root perturbation choice. |
| 53 | Chapters 4–5 justify the successive subsequence indices, choose a late tail before an almost-extremal term, display negated epsilon–delta quantifiers, and use the same subsequence indices in the uniform-continuity contradiction. |
| 54 | Chapter 7 compares finite rearranged sums before taking limits and writes the rectangle-minus-triangle Cauchy-product error before bounding tails. |
| 55–58 | Chapter 8 constructs the chain-rule auxiliary function, freezes a sufficiently late derivative index before taking the increment limit, derives Taylor's auxiliary coefficient with the endpoint fixed, and separates convexity/secant/mean-value inequalities. |
| 59–63 | Chapter 9 proves its interval Lebesgue-number and finite-cover tools before Arzelà uses them. Nested open sets are handled through closed compact subsets and summable errors. Arzelà fixes the point before its late index; Dini freezes the comparison index; the first FTC treats positive and negative increments; absolute improper convergence uses Cauchy tails. |
| 64–66 | Chapter 11 fixes the testing unit functional during the one-variable mean-value argument, substitutes the full multivariable remainder, and proves smooth matrix inversion before higher inverse and implicit regularity. |
| 67–68 | Chapter 12 separates image-boundary control, retained versus boundary cells, and finite integral sums with error estimates. Polar truncation uses independent Cartesian central-square and seam bounds. |
| 69–70 | Chapter 13 constructs transition derivatives, proves the cocycle and inverse identities, proves equivalence, transfers vector operations independently of representatives, and constructs inverse coordinate maps. Coordinate conjugation proves that the differential is intrinsic. Boundary tangent spaces still contain all coordinate directions. |
| 71–73 | Pullback composition is checked by scalar evaluation; the graded Leibniz proof tracks the sign past the first wedge block; local Stokes computes the upper/lower face orientations and the resulting endpoint signs. |
| 74–76 | A local-finiteness lemma precedes its uses. Manifold integration is compared through compactly supported overlap pieces and a finite double sum. Explicit smooth weights on two circle charts recover the integral 2π. |
| 77 | Appendix A expands only the orbit-following, nonoverlap, and uniqueness steps in disjoint-cycle decomposition. |
| 78 | Removed the stale later Jordan introduction and duplicate Chapter 13 direct-sum definition. Chapter 13's contents and opening titles agree, with a separate short running header. Cross-references and numbering were regenerated. The trigonometric-series example asserts the continuity actually proved, without an uncited nowhere-differentiability claim. |
| 79 | Added focused method exercises in Chapter 10, Chapter 13, and Appendix B: negation and bad sequences, cover mechanisms, direct-sum criteria, coordinate changes, quotient/tensor map construction, invalid elementary rules, equality of already constructed maps, and tangent-chart comparisons. |
| 80 | No additional general topology course, spectral linear algebra, or module theory was introduced. Finite epsilon-nets mean finite metric approximating sets, not generalized sequences. Appendix B remains over fields. |
| 82 | The full PDF was compiled, references checked, every page rendered, and the layout reviewed as recorded below. README, outline, and revision history are updated. |

## Preserved arguments and dependencies

- The metric compactness proof retains the correct closed tails
  `F_N = closure({x_n : n >= N})`; the revision explains their use and the
  later increasing-index selection.
- The nonlinear local volume lemma retains its maximum on the compact
  closure of the neighborhood. It was not changed into an unsupported
  maximum on an open neighborhood.
- The determinant-first conceptual order remains: normalized alternating
  form, structural laws, and then the coordinate formula. Appendix B's top
  exterior power is retrospective and is not a prerequisite for Chapter 10.
- The single explicitly imported manifold-refinement theorem remains
  identified and attributed. This pass does not claim to prove general
  paracompactness.
- Source-order checks confirm metric continuity before topological
  continuity, Chapter 9's interval cover tool before its open-length use,
  finite direct sums before later uses, and quotient factorization before
  tensor universality.

## Reference consultation

The neighboring Algebra manuscript was consulted selectively: the determinant
construction in `chapters/modules.tex`, permutation development in
`chapters/groups-foundations.tex`, binary and multivariable universality,
associativity, and direct sums in `chapters/tensor-products.tex`, and exterior
multiplication in `chapters/exterior-algebra.tex`. This was a targeted source
comparison, not a full rereading of the Algebra manuscript or the reference
books. The existing analysis bibliography was preserved. No external theorem
about nowhere differentiability was imported to justify the weakened example.

## Validation record

- Final output: `main.pdf`, 265 pages. Final repeated pdfLaTeX passes stabilized
  numbering and contents with no LaTeX, pdfTeX, overfull-box, underfull-box, or unresolved
  reference warnings. Final logs are `tmp/architecture-build7.txt` and
  `tmp/architecture-build8.txt`.
- Source checks: 19 active TeX files, 307 unique labels, 313 resolved reference
  occurrences; checked proof/theorem/definition/exercise/diagram environments
  and display delimiters are paired.
- Existing exact checks were retained and run for determinant examples,
  all six Leibniz-table terms, coordinate changes, pullback/flux calculations,
  and the exterior coefficient obstruction. Additional exact-arithmetic
  checks cover the new derivative matrix, rectangular matrix evaluation,
  kernel generator and explicit target lifts, nonstandard coordinates,
  and rectangular and square composition.
- All pages were rendered with PDFium at 1.5 scale. All 23 contact sheets
  were visually inspected. The final render was compared by page-image hash
  with the first reviewed render: 231 final pages were identical images;
  the 34 changed page images were reviewed again. Review at contact-sheet
  scale covers page flow; detailed review at full-page scale covers the
  selected formulas and diagrams listed next.
- Detailed inspection included all four contents pages; the preface and
  reading guide; compactness proofs; the vector-space axioms; representative
  matrices and coordinate diagrams; the Leibniz table; compact-Jordan-region
  estimates; local Stokes signs; tangent transitions and the differential;
  common-refinement integration and the circle example; and every Appendix B
  commutative diagram. The multivariable tensor, associativity, Tensor–Hom,
  exterior-product, and exterior-duality proof pages were also examined at
  full-page scale.
- Layout repairs included fitting the contents in four pages, keeping the
  vector-space axioms together, keeping the compactness definition together,
  removing the overwide example heading and running header, and keeping the
  canonical-isomorphism explanation with its revised two-way diagram.

The machine-readable source report, exact checks, render manifest, image
hashes, and rendered pages are in `tmp/architecture-qa/`. They are local QA
artifacts excluded by the existing `tmp/` ignore rule. The final PDF SHA-256 is
`63f3d5111d83503f17823caab930af1ea5b6b91a4c16ffa2dd5a7adc0d89a3c9`.

These checks establish the recorded build, layout, reference consistency,
and selected exact calculations; they are not a formal proof verification
of the entire manuscript.

</details>

<a id="historical-revision-3.12.0-audit"></a>
<details>
<summary>REVISION 3.12.0 AUDIT</summary>

# Version 3.12.0 revision audit

**Date:** September 14, 2026
**Starting point:** the local Version 3.11.0 manuscript, including its existing
uncommitted changes. A starting snapshot is retained under
`tmp/revision350/baseline`. Copy-named files are not inputs to `main.tex` and
were not edited. No commit, tag, release, or remote publication was made.

This revision has three independent components: the FTC extensions in
Chapters 8–9, refinement of the existing higher-order theory in Chapter 11,
and a manuscript-wide prose pass. The prose pass does not expand the
mathematical scope of other chapters.

## 1. FTC locations

Page numbers below are the printed manuscript numbers, not PDF viewer indices.

| Addition or preserved result | Exact location | Printed page |
|---|---|---:|
| Darboux's theorem for derivatives | §8.2, Theorem 8.2.4, immediately after the ordinary MVT proof | 75 |
| Newton–Leibniz with an integrable derivative | §9.4, Proposition 9.4.12 | 110 |
| Three distinct assertions and the two counterexamples | §9.6, “How Far Can Newton–Leibniz Be Extended?”, Examples 9.6.12–13 | 119 |
| Finite modifications and finite-exception FTC | §9.6, preparatory paragraph and Theorem 9.6.14 | 119–120 |
| Countable-exception FTC, complete four-step proof | §9.6, Theorem 9.6.15 | 120 |
| Finite versus countable modifications | §9.6, immediately after Theorem 9.6.15 | 121 |
| Lipschitz/a.e. Riemann statement, proof deferred | §9.6, Theorem 9.6.16 | 121 |
| Cantor-function warning | §9.6, Remark 9.6.17 | 121 |
| Absolute continuity and its elementary implication hierarchy | §9.7, Definition 9.7.2 and following paragraph | 122 |
| Both directions of the Lebesgue FTC, proof deferred | §9.7, Theorem 9.7.3 | 123 |
| FTC hierarchy with hypotheses and proof status | §9.7, “The hierarchy of FTC statements” | 123 |
| Targeted finite-modification and countability exercises | Chapter 9, Exercises 10–11 | 124 |

The stronger hierarchy is an unnumbered subsection at the end of §9.6,
after the existing Lebesgue criterion and Dirichlet–Thomae discussion.
It adds no numbered section and introduces no forward dependency into §9.4.
The only changes at Proposition 9.4.12 are a reference label and a short
forward-reference paragraph after its proof. A comparison with the starting
snapshot verifies that its statement and entire proof are otherwise identical,
including the partition-dependent MVT tags and exact tagged sum.

The unbounded-derivative example computes the derivative at zero directly
and uses `x_n=(2πn)^(-1/2)` and its negative to cover both one-sided cases.
Its conclusion explicitly excludes degenerate intervals. The step-function
example computes the accumulation function and its two one-sided derivatives.

## 2. Countable-exception mathematical audit

All the following requirements are met within Theorem 9.6.15:

1. **Countability:** every nondegenerate interval contains a nonexceptional
   point. The proof explicitly invokes uncountability of real intervals.
2. **Darboux:** a derivative value outside the bounds of `f` would force
   a nondegenerate interval of values into the countable image `F'(E)`.
   This is an argument about values of the derivative, not merely density
   of the nonexceptional points.
3. **Boundedness first:** the upper and lower bounds for `F'` are established
   before the Lebesgue criterion is applied.
4. **Continuity comparison:** the same reasoning on an open subinterval
   proves a local range bound for `F'`. At a continuity point `x` of `f`,
   shrinking the bound proves `F'(x)=f(x)`, including exceptional `x`.
   The neighborhood estimate then proves continuity of `F'` at `x`.
5. **Endpoints:** an extension `g` has endpoint values `f(a),f(b)`.
   Its discontinuities are contained in `Disc(f)∪{a,b}`; the proof does
   not require endpoint differentiability or endpoint continuity of `g`.
6. **Lebesgue criterion:** boundedness and negligibility of this
   discontinuity set give Riemann integrability of `g`.
7. **Equality of integrals:** tags are chosen in the interior of each cell
   outside `E`. The two tagged sums are equal, and both converge because
   both integrands have already been proved integrable. Equality of integrals
   is not inferred from countability alone.

The finite theorem instead uses the elementary finite-modification argument
and Proposition 9.4.12 directly. The Dirichlet example explains why the
countable proof cannot be replaced by arbitrary countable modification.

The Lipschitz theorem explicitly requires existence of the derivative outside
the negligible set. Its discussion reduces the result to the deferred theorem
that a Lipschitz function with derivative zero a.e. is constant. The Cantor
function is described as continuous and nondecreasing, not Lipschitz. The
absolute-continuity preview clearly distinguishes the later Lebesgue integral
from the Riemann integrals in the preceding statements.

## 3. Every materially revised higher-derivative passage in Chapter 11

All of these passages are in §11.3 unless indicated otherwise. Existing
results are refined in place; the sole new numbered higher-order example is
Example 11.3.12.

| Passage | Revision | Printed page |
|---|---|---:|
| Opening of “Higher Derivatives and Local Estimates” | Directly connects restriction to a segment with one-variable estimates and evaluation of multilinear derivatives | 186 |
| Definition 11.3.5, Higher derivatives | Displays the operator-valued types and the canonical bilinear identification in both directions, without choosing a basis | 188 |
| Example 11.3.10, Two directions versus a repeated direction | Adds the full first-derivative linear map to the existing Hessian and two-direction computation | 190 |
| “Higher orders: arrays represent multilinear maps” | Displays permutation symmetry and explains mixed-partial symmetry as a statement about the intrinsic bilinear map | 191 |
| “Second-order objects at a glance” | Replaces the boxed workflow with distinctions among the map, matrix, mixed partials, two-direction evaluation, repeated evaluation, and second directional derivative | 191 |
| Example 11.3.12, A vector-valued second derivative | Computes the linear first derivative, vector-valued bilinear second derivative, component Hessians, and repeated-direction value | 192 |
| Remark 11.3.13, Symmetric and alternating multilinearity | Retains the mathematical comparison, with a small prose refinement | 192 |
| Proposition 11.3.15 and following discussion | Uses explicit evaluation brackets; explains outer curvature and inner nonlinear variation, the scalar chain rule, and input-group partitions at higher orders | 192–193 |
| Existing curved-path and line-restriction discussion | Retained as the bridge into Taylor; read together with the new object comparison and chain-rule explanation | 193 |
| Theorem 11.3.17 and Corollaries 11.3.18–19 | Retains the segment theorem, vector norm bound, and Peano proofs; clarifies the regularity comparison and keeps short statements/proofs together | 194–195 |
| “Coordinate expansion of the Taylor polynomial” | Moves the modest multi-index definitions before analyticity; derives the finite expansion from repeated multilinear inputs and the multiplicity `j!/α!` | 195 |
| “Smoothness and real analyticity” | Reuses the established finite coordinate identity to explain grouping of the analytic series; preserves all analytic estimates | 195–196 |
| “Higher derivatives of local inverses and implicit graphs” | Adds the first-derivative formula, smooth operator inversion, the inductive composition step, and graph construction through `(x,F(x,y))` | 196 |
| §11.5, inverse proof step 5 | Removes one redundant lead-in sentence; the `C^1` core, bootstrap, and normalization argument remain intact | 203 |

The regularity explanation avoids the misleading shortcut of composing
with an inverse whose higher regularity has not yet been proved. It first
establishes regularity of `x↦[DF(x)]^(-1)`, then raises regularity of the
inverse one order at a time. It also distinguishes operator inversion from
differentiation of the inverse function.

The existing higher-order, Hessian, and Taylor exercises already cover the
requested computations. They are retained rather than supplemented by
duplicates. No Banach-space theory, manifold tensor calculus, jets, or full
Faà di Bruno theorem has been added.

## 4. Manuscript-wide prose audit

The pass covers all files included by `main.tex`: thirteen chapters, both
appendices, preface, and reference annotations. It includes more than 80
individually considered replacements, followed by contextual corrections,
section-opening review, a complete source phrase scan, repeated-phrase
checks, and a rendered prose spot-check in every chapter. A mechanical scan
examined 1,291 text-containing paragraph blocks; this is a search inventory,
not a substitute for reading the selected passages in context.

Representative changes:

| Area | Before | After or treatment |
|---|---|---|
| Chapter 1 | “The precision is not a bureaucratic replacement for intuition.” | Explains directly how hypotheses make calculations reliable and help locate errors |
| Chapter 2 | “Why should analysis care? Choice packages…” | States simultaneous selection and its countable-union application directly |
| Chapter 3 | “The preceding theorem makes this definition…” | Names the uniqueness theorem, preserving the distinction between characterization and construction |
| Chapter 4 | “The limsup records the eventual ceiling” | “The limsup is the eventual ceiling” |
| Chapter 5 | “The following compact notation records…” | “We use the following notation…” |
| Chapter 6 | “The general lesson is…” | Specifies the different estimates needed for integration and differentiation |
| Chapter 7 | “fixed positive multiples … are the mechanism” | States directly that fixed positive multiples control the tail |
| Chapter 8 | “The correct workflow is…” | Explains why differentiation rules apply away from zero and the definition is needed at zero |
| Chapter 9 | “This is why sampled values…” | States the mesh-controlled approximation independently of sample choices |
| Chapter 10 | “This equation is the mechanism…” | States preservation of the old span and why inserted vectors remain available |
| Chapter 11 | “Use one sufficiently late continuous map as a bridge” | “Choose one sufficiently late continuous map” |
| Chapter 12 | “The workflow is: sketch the solid…” | Gives the slicing instructions as direct sentences |
| Chapter 13 | “Pullback as a workflow…” | “Computing pullbacks on a surface” |
| Appendix A | A short proof strategy repeats the following sentence | Removes the repeated narration, leaving the proof argument |
| Appendix B | “This is why the product construction…” | States that the construction must respect relations among decompositions |

Repeated wording in the actual compiled inputs was checked again:

| Phrase | Before | After |
|---|---:|---:|
| “the mechanism” | 9 | 0 |
| “this is why” | 7 | 0 |
| “the preceding theorem” | 2 | 0 |
| “the general lesson” | 1 | 0 |
| “workflow” | 7 | 0 |
| “this is exactly” | 3 | 1 |
| “supplies” | 80 | 65 |
| “records” | 34 | 30 |

Remaining contrasts explain substantive distinctions: the order of choosing
indices, normalized errors, the role of a defining function, and local
finiteness rather than pointwise finiteness. Repeated quantifier language,
standard hypotheses, and mathematical terminology are retained. The pass
does not make every paragraph conform to a single template.

## 5. Preservation and validation

- **Build:** final MiKTeX `pdflatex -synctex=1 -interaction=nonstopmode
  -halt-on-error main.tex` passes succeed. The `.aux`, `.toc`, and `.out`
  files stabilize. The final PDF has **348 pages**.
- **Log:** no LaTeX/package warning, undefined reference, duplicate-label
  warning, overfull box, or underfull box. Extracted PDF text has no `??`.
- **References:** **412 distinct source labels**, all unique; **438 reference
  uses**, including named subsection references, all resolve.
- **Proof preservation:** mathematical-expression sequences in all **348
  pre-existing proof bodies** are retained. All original formal statement
  expressions outside Chapters 8, 9, and 11 remain unchanged. The only
  altered formal-statement prose there names Chapter 3's uniqueness theorem
  instead of saying “the preceding theorem.”
- **Architecture:** exact comparison protects Proposition 9.4.12. Mathematical
  expressions in the contraction and inverse/implicit sections remain in
  their original order. The normalized fixed-point construction, inverse
  derivative remainder proof, regularity induction, undoing normalization,
  and implicit graph through `H(x,y)=(x,F(x,y))` remain intact.
- **Types:** scalar versus vector output, operator-valued derivatives,
  bilinear evaluation, component Hessians, and the two chain-rule outputs
  were checked. The general vector Taylor proof still avoids asserting one
  common Lagrange point for all components.
- **Visual review:** source-to-page mapping selected **118 pages** containing
  edits and neighboring context, including cover/contents. These were rendered
  and inspected in contact sheets; the new FTC and higher-derivative
  passages were also inspected at enlarged full-page resolution. The final
  checks cover margins, displays, diagrams, theorem breaks, and proof flow.
  Short examples and statements received page-space guards where needed.
- **Hyperlinks:** all **15 selected theorem/example destinations** land on
  pages containing their headings. Guards repair preceding-page destinations
  for the higher-derivative definition, segment Taylor theorem, and Lebesgue
  FTC preview. The inverse and implicit theorem destinations also pass.
- **Versioning:** `preamble.tex` provides Version 3.12.0 and the revision date
  to the existing title-page macros. The cover, README, and this audit agree.

Reproducible local evidence is retained under `tmp/revision350`: baseline
snapshot, edit scripts, prose replacement inventory, build logs, preservation
results, per-file diffs, source-to-page map, extracted PDF text, and rendered
QA pages. The primary manuscript remains `main.tex` with compiled `main.pdf`.

</details>

<a id="historical-revision-3.13.0-audit"></a>
<details>
<summary>REVISION 3.13.0 AUDIT</summary>

# Version 3.13.0 Focused Dependency Revision Audit

Date: September 15, 2026

## Scope

Version 3.13.0 is a focused Chapter 10--11 dependency and
inverse-function-theorem refinement. It does not enlarge the manuscript's
subject scope. The Version 3.12.0 FTC additions, higher-derivative theory, and
other settled proofs remain in place except for the requested local cleanup
and dependency repairs.

## Chapter 10

- Introduced Euclidean length, Euclidean distance, and the default notation
  `||x|| = ||x||_2` at the start of the metric-space discussion. The text calls
  the formula a length until Cauchy--Schwarz proves its triangle inequality,
  then records the induced norm and metric.
- Defined closed balls with dedicated notation and proved directly that they
  are closed. Added the closed-ball-inside-an-open-set proposition.
- Consolidated interior, closure, boundary, limit points, and isolated points.
  Proved `cl(E) = E union E'` and `cl(E) = int(E) union boundary(E)` before
  deriving the five equivalent closed-set characterizations and the disjoint
  neighborhood formulation.
- Gave separate theorem status to the sequential closure/limit-point criteria
  and to the sequential characterization of closed sets.
- Collected uniqueness of limits, subsequence inheritance, convergent-implies-
  Cauchy, completeness, the sequential limit criterion for maps, and the
  sequential continuity criterion in arbitrary metric spaces.
- Promoted completeness of closed subsets to a proposition and derived
  completeness of closed balls as a corollary, with the open-ball contrast.
- Added finite-product convergence and its Euclidean coordinatewise
  specialization.
- Consolidated the bounded-linear-map equivalences and all operator-norm
  formulas, including the optimal Lipschitz constant and the
  finite-dimensional maximum on the unit sphere.

## Chapter 11

- Replaced the repeated general metric-limit setup with citations to Chapter
  10 while retaining finite-dimensional coordinate estimates, path tests,
  uniform convergence, equicontinuity, and Arzela--Ascoli.
- Explained why the Frechet derivative is defined on an open domain, used
  openness explicitly in uniqueness, and added the lower-dimensional-domain
  warning and tangent-space remark.
- Reordered the local second-derivative discussion to place scalar and vector
  examples before the second-order summary, followed by general higher-order
  symmetry, while removing a repeated operator-valued expansion.
- Rewrote the inverse function theorem proof in eleven explicit stages:
  translation, linear normalization, fixed-point equation, operator-norm
  derivative control, convex-segment mean-value estimate, invariant complete
  closed ball, open source/target neighborhoods, inverse Lipschitz estimate,
  nearby derivative invertibility, direct inverse differentiation, regularity
  bootstrap, and normalization reversal.
- The normalized contraction constant is fixed at `1/2`; the target is the
  open ball `B(0,r/2)`; the contraction acts on the complete closed ball
  `closed B(0,r)`; and the inverse derivative is written unambiguously as
  `D(F^{-1})`.

## Residual cleanup and documentation

- Chapter 9 now distinguishes failure of `F' = f` on an exceptional set from
  possible failure of differentiability itself in the Lipschitz/a.e. theorem.
- The Lebesgue preview now states precisely what the Dirichlet and Thomae
  examples show, without describing the rationals as sparse.
- Local references accompany the unproved Lipschitz/a.e., Lebesgue FTC, and
  Cantor-function previews. The preface and attribution note identify these
  as unproved, non-prerequisite previews.
- The preamble, README, and outline identify the draft as Version 3.13.0 and
  describe it as a focused dependency refinement.

## Validation

- Two final MiKTeX `pdflatex` passes completed successfully.
- Final artifact: 354 pages.
- Build log: zero LaTeX errors; zero LaTeX/package, undefined-reference,
  duplicate-destination, overfull-box, or underfull-box warnings.
- Source audit (excluding archival `- Copy` files): 424 labels, all unique;
  453 `ref`/`cref`/`Cref` uses, with zero missing labels.
- Operator-norm notation in Chapters 10--11 uses `op` consistently; no
  ambiguous `DF^{-1}` notation or closure-of-open-ball notation remains in the
  revised material.
- Poppler render review covered 39 affected physical PDF pages: cover page 1;
  preface page 8; Chapter 9 pages 128--130; Chapter 10 pages 135--145 and
  167--169; Chapter 11 pages 182--186, 198--204, and 213--219; and references
  page 354. No clipping, overlap, broken glyph, hierarchy, or page-flow defect
  was found.

No Git tag or release was created.

</details>

<a id="historical-revision-3.13.1-audit"></a>
<details>
<summary>REVISION 3.13.1 AUDIT</summary>

# Version 3.13.1 Finishing Revision Audit

Date: September 15, 2026

## Scope and preservation

Version 3.13.1 is a focused finishing pass on dependency order,
affine/linear notation, proof naturalization, and hidden proof mechanisms.
It preserves the Version 3.13.0 metric-space foundations, closed-set and
sequential theory, operator-norm characterization, higher-derivative
development, complete-ball inverse-function argument, direct inverse
differentiation, and higher-regularity bootstrap.

## Dependency and notation repairs

- Chapter 10 now introduces open and closed balls without using topological
  terminology. After open and closed subsets are defined, one proposition
  proves both that open balls are open and closed balls are closed.
- The distinction between the closed ball `\overline B(a,r)` and the closure
  `\overline{B(a,r)}` is retained, with the discrete metric showing that the
  two need not agree.
- Chapter 8 now records why convex combinations of points in an interval stay
  in that interval. Chapter 11 defines convex subsets before the multivariable
  mean-value theory and proves that open and closed normed-space balls are
  convex.
- The notation `\mathcal L(V,W)` and convention
  `\mathcal L(V):=\mathcal L(V,V)` now accompany the first definition of a
  linear map. The later result establishes the vector-space structure and
  dimension rather than reintroducing the notation.
- Affine maps, their linear and translation parts, their base-point form, and
  invertible affine changes of coordinates are defined before affine
  approximations are used.
- The operator-norm proposition now has the correct bounded-map scope, and the
  continuity-at-zero scaling proof concludes with a uniform weak inequality.

## Proof naturalization

- All literal `Proof. Strategy.`, `Proof. Idea.`, and `Proof. Roadmap.`-style
  openers in the active manuscript were reviewed. Their useful mathematical
  mechanisms remain, but repetitive labels were integrated into ordinary
  proof prose.
- Checklist language in the inverse- and implicit-function arguments was
  replaced by short mathematical headings and declarative transitions.
- Appendix B retains construction-before-evaluation, quotient
  well-definedness, map-valued linearity, and spanning safeguards without
  proof-auditor narration.

## Representative hidden mechanisms made explicit

- In the continuous-partials criterion, the coordinate polygonal path is kept
  inside the derivative neighborhood by
  `||p_j-a||_2 <= sum_i |h_i| <= sqrt(n)||h||_2`, so
  `||h||_2 < r/sqrt(n)` controls every segment.
- Openness of `GL(R^n)` now displays
  `||A^{-1}(B-A)||_op <= ||A^{-1}||_op ||B-A||_op` and the concrete radius
  `1/(2||A^{-1}||_op)` before invoking the perturbation theorem.
- The rectangular change-of-variables proof constructs a positive compact-to-
  open-set margin from finitely many doubled balls and an explicit minimum of
  radii before defining a uniform derivative bound.
- The half-space change-of-variables proof expands its thin-image claim into a
  sequential contradiction: source heights tend to zero, compactness produces
  a boundary limit, and continuity plus boundary preservation forces target
  heights to tend to zero. The remaining integral error is bounded by height
  times strip volume.
- The manifold/Riemann comparison constructs finitely many coordinate
  rectangles from doubled-radius balls and a grid whose cell diameter is below
  the least selected radius.
- The inverse-function proof retains the inverse Lipschitz estimate
  `||Delta x|| <= 2||h||`, the quotient comparison for
  `R(Delta x)=o(||h||)`, and the bounded-operator estimate for applying
  `Df(x)^{-1}` to that remainder.

## Inverse and implicit functions

- Translations are proved directly to have derivative `I`, zero remainder,
  vanishing higher derivatives, inverse translation, and therefore global
  `C^infinity` diffeomorphism status.
- The normalized proof uses `\widetilde U,\widetilde f` only during
  normalization, then uses `U,f,U_0,V_0,g` throughout the contraction
  argument. The contraction constant remains `q=1/2` on a complete closed
  ball, and the target remains `B(0,r/2)`.
- Returning to the original coordinates uses the normalized neighborhoods
  directly, without superscripted normalization notation, and retains the
  order reversal `[Df(h)]^{-1}=[DF(x_0+h)]^{-1}A`.
- The implicit-function proof preserves construction, graph uniqueness,
  invertibility, and differentiation in that order, with the block derivative
  beginning in its own paragraph.

## Validation

- The final two-pass build produces a 356-page PDF.
- The active manuscript contains 428 labels and 464 reference targets, with
  no duplicate labels and no unresolved targets.
- The final log contains no LaTeX or package warnings, box warnings, undefined
  references, PDF warnings, or compilation errors.
- A destination-level audit checked 27 high-risk theorem and proposition
  links; every target page contains the referenced numbered statement. This
  includes the reverse-triangle, alternation, contraction, closure,
  sequential-closure, operator-norm-characterization, and finite-exception
  anchors.
- Forty representative pages were rendered and inspected, covering the title
  page, Chapter 8 convexity, Chapter 9 endpoint material, the Chapter 10
  topology/linear-algebra repairs, the Chapter 11 inverse- and
  implicit-function spreads, the strengthened Chapter 12 and 13 mechanisms,
  both appendices, and the final references page.
- `git diff --check` reports no patch-format errors; its only messages are the
  repository's existing line-ending normalization notices.
- No Git tag or release was created.

</details>

<a id="historical-revision-3.14.0-audit"></a>
<details>
<summary>REVISION 3.14.0 AUDIT</summary>

# Version 3.14.0 Revision Audit

Date: September 15, 2026

## Outcome

Version 3.14.0 expands the finite-dimensional local theory in Chapter 11 and
reorganizes nonlinear change of variables in Chapter 12 around primitive
substitutions and finite Euclidean localization. Chapter 13 retains the
locally finite manifold theorem and its external topological refinement.
The final PDF has **365 pages**.

## Preservation and corrections

- The Chapter 10 metric/topological architecture, sequential criteria,
  completeness, operator norms, and `L(V) := L(V,V)` are retained.
- The affine base-point formula now fixes `y_0 = F(x_0)` for the chosen
  `x_0` and the already fixed affine map.
- Chapter 11 cross-references Chapter 10's Euclidean convexity definition
  when extending convexity to arbitrary real vector spaces.
- The inverse-function proof retains smooth translations, the fixed
  contraction constant `1/2`, the complete closed ball, segment containment,
  inverse Lipschitz bound, direct little-o differentiation, the `C^k`
  bootstrap, and explicit reversal of normalization.
- The estimate on `(Df(x)-I)v` now uses a weak inequality, including `v=0`.
- The residual basis-image proof instruction is ordinary explanatory prose.
  Exercise instructions and explicitly labeled computational checklists
  retain their pedagogical role.
- The vague Chapter 9 sentence about discontinuities being distributed
  throughout an interval was removed; the Dirichlet–Thomae distinction remains.

## Chapter 11: local differential structure

The end of the chapter is organized as §11.5 Inverse and Implicit Functions,
§11.6 Rank and Local Normal Forms, and §11.7 Perspective and Transition.
Existing inverse-function examples remain adjacent to that theorem.

| Result | Final number | Verification |
| --- | --- | --- |
| Linear implicit theorem | 11.5.6 | Direct-sum kernel graph, typed graph map, elementary equivalence; no redundant surjectivity hypothesis |
| Nonlinear implicit theorem | 11.5.8 | Retained straightening proof; block derivatives and explicit linear/nonlinear comparison precede it |
| Analytic Lagrange inversion | 11.5.12 | Optional stated analytic result, locally referenced; convergence is not attributed to smooth IFT |
| Rank and persistence | 11.6.1–2 | Rank is defined first; nonzero-minor determinant kept within half its nonzero value |
| Constant Rank Theorem | 11.6.3 | Full Euclidean proof, including rank zero and empty blocks; extra columns vanish by their zero top block |
| Immersion/submersion | 11.6.4 | Defined after rank; maximal rank persists and gives inclusion/projection forms |
| Regular level sets | 11.6.6 | Direct graph proof, curve-velocity tangent directions, `T_a F^{-1}(c) = ker DF(a)`, scalar gradient case |
| Dimension consequences | 11.6.11–13 | Maximal-rank noninjectivity proof; nonsurjectivity forward reference; direct chain-rule dimension equality |
| Primitive maps/factorization | 11.6.14–15 | One changed coordinate, determinant condition; actual local diffeomorphisms `H_j H_{j-1}^{-1}` with explicit domains |
| Euclidean cutoff/finite POU | 11.6.17–18 | Finite ball cover from Chapter 8; compact supports and globally smooth normalized weights |

The finite partition proof includes an outer cutoff on `{sum chi_i > 0}`.
This makes zero extension smooth where the denominator would otherwise
vanish, while retaining the usual quotient formula near the compact set.
The old `cor:compact-cutoff` label is an alias on the earlier Euclidean lemma,
so existing references continue to resolve to the result that now proves it.

The Lagrange example `w = z(1+w^2)` gives
`z + z^3 + 2z^5 + 5z^7 + ...`; initial coefficients are independently derived
by substitution, and its explicit square-root solution demonstrates
convergence in this example. Analytic existence and the general coefficient
formula are clearly marked as optional external results.

## Chapter 12: structural substitution

The principal order is:

1. Primitive substitution (12.5.1): each fiber component is an interval,
   the derivative has constant nonzero sign on it, and compact support
   meets only finitely many components for a fixed parameter. Ordinary
   substitution and continuous zero-extension Fubini give the formula.
2. Composition and restriction (12.5.2): transformed supports remain compact,
   and the chain rule supplies the determinant product.
3. Local factorization (12.5.3): primitive factors and coordinate permutations
   give local substitution.
4. Compact-support theorem (12.5.4): finite Euclidean source weights produce
   target functions `f_i = (rho_i o Phi^{-1}) f`; their compact supports lie
   inside the corresponding target neighborhoods. Both finite sums are checked.
5. Jordan-null and boundary control (12.5.5): a derivative bound on a compact
   neighborhood controls images of fine cubes. Homeomorphism invariance of
   boundary supplies Jordan measurability separately.
6. Compact-region recovery (12.5.6): interior cutoffs discard only thin
   boundary neighborhoods and their small-volume images. This proof works
   for `f` given only on `Phi(E)` and assumes no extension theorem for it.
7. Rectangular form (12.5.7): compactness and local injectivity give one
   diffeomorphism neighborhood of the rectangle, even though the original
   hypotheses require injectivity only on the rectangle.
8. Optional local Jacobian distortion (12.5.8): normalization by `D Phi(a)`
   and a derivative estimate for the inverse give inner and outer cube
   bounds. There is no second contraction argument or duplicated long main proof.

The rectangular integration, Fubini, Jordan-set algebra, linear substitution,
and half-space toolkit remain. The old long nonlinear cube-based proof has
been replaced, not retained as a competing main proof.

Theorem 12.3.18 completes the full lower-dimensional nonsurjectivity proof.
A compact source cube has image covers of total volume `O(k^(n-m))`.
Countably many rational cubes cover an arbitrary open source; covers with
budgets `epsilon 2^{-j}` cannot cover a positive-volume compact target cube,
since a finite subcover would contradict finite volume comparison. This
proves empty interior without Baire category, Lebesgue measure, or a false
countable-union assertion about Jordan content.

Schwartz's 1954 remark describes the one-sided inequality plus inverse-map
principle. The separate Lebesgue preview identifies the source measure
`nu(E)=m(Phi(E)) = ((Phi^{-1})_*m)(E)` and its Jacobian density, explicitly
without developing or proving measure theory.

## Chapter 13 and references

- The manifold POU proof reuses the Euclidean cutoff. It concentrates on
  locally finite refinements, chart supports, smooth local sums, and regrouping.
- The general manifold POU theorem and the explicitly external
  paracompactness/refinement theorem remain.
- Coordinate invariance still uses Chapter 12's Euclidean substitution;
  manifold integration is downstream of both.
- Chapter 8, the preface, outline, README, version macro, and attribution note
  now describe the new dependency chain.
- Selective comparisons included Knapp's Chapter III finite localization and
  primitive reduction, Munkres §§18–19 (including the stronger one-coordinate
  exercise), Rudin's primitive mapping treatment, and the geometric volume
  viewpoints in Pugh and Bartle. The proofs are independently written with
  the manuscript's hypotheses and Riemann conventions. Existing Zorich,
  Spivak, Apostol, Lee, and Tu references remain in their respective roles.
- Added Gessel and Sokal for the optional analytic result, and J. Schwartz,
  *The American Mathematical Monthly* 61(2) (1954), 81–85,
  DOI `10.1080/00029890.1954.11988420`. Bibliographic data were checked against
  the journal/author records. No source was reproduced wholesale.

## Build, reference, hyperlink, and visual validation

- MiKTeX `pdflatex -interaction=nonstopmode -halt-on-error main.tex`
  completed successfully. The final consecutive builds have identical
  SHA-256 hashes for `main.aux`, `main.toc`, and `main.out`.
- The final log contains no LaTeX/package warnings, undefined references,
  duplicate destinations, overfull boxes, underfull boxes, or compilation errors.
- Active sources contain **449 labels**, **468 reference uses**, and
  **20 bibliography entries**: no duplicate label keys, unresolved references,
  or missing citation keys.
- All **406 labeled statement destinations** were checked against the numbered
  statement on the destination PDF page. All pass, including the earlier
  audit's contraction, closure, sequential, operator-norm, reverse-triangle,
  alternation, and finite-exception targets, and every new statement.
- The expanded audit initially detected **40 one-page-early targets**.
  Reserving six lines before theorem-like environments, before the anchor is
  created, fixes their page-break behavior throughout the manuscript.
- All **726 internal PDF links** point to existing named destinations.
- **52 pages** were rendered and visually inspected, including every page of
  the new local-structure and nonlinear-substitution material, the complete
  preserved IFT proof, finite Euclidean POU, dimension covering proof,
  manifold POU and integration bridge, new exercises, title/contents,
  Chapter 8 cutoff bridge, affine wording, and bibliography. No clipping,
  overlaps, or broken mathematical displays were found.
- `git diff --check` passes; only pre-existing line-ending normalization
  notices appear. Existing unrelated workspace changes were retained.
- Machine-readable checks and page renders are in `tmp/revision360/`.
- No Git tag, release, or commit was created.

</details>

<a id="historical-revision-3.14.1-audit"></a>
<details>
<summary>REVISION 3.14.1 AUDIT</summary>

# Version 3.14.1 revision audit

Date: September 15, 2026

## Scope

Focused finishing proof-naturalization and dependency patch to Version 3.6.0.
The Chapter 11–13 architecture and the existing foundational proofs are
preserved. No exercises, external references, Git tags, or releases were added.

## Mathematical changes and checks

- **Proposition 10.17.8, rank and nonzero minors:** defines rectangular minors,
  including the empty determinant. The proof uses independent columns,
  rank–nullity to establish row spanning, and determinant/invertibility
  equivalence. It follows Theorem 10.17.7 (determinant laws) and precedes
  every Chapter 11 use. Rank persistence cites it. The constant-rank proof's
  references to an invertible minor now correctly say invertible submatrix.
- **Proposition 11.3.6, differentiating limits:** displays the uniform error
  e_k and the triangle-inequality comparison. The proof first takes k to
  infinity for fixed h, then h to zero, using continuity uniformly along
  the shrinking segment.
- **Definition 11.6.14 and the following explanation:** constant derivative
  sign gives strict fiber monotonicity, hence injectivity on the product
  box. The inverse function theorem gives open image neighborhoods; inverse
  branches agree on overlaps by injectivity and form the C^k inverse.
- **Theorem 11.6.15:** replaces the leading-principal-minor pre-proof with
  successive coordinate replacement. The nonzero vector DF_(j-1)e_j has
  zero first j-1 components, so a remaining output detects e_j. The proof
  defines G_j as the permuted residual before forming P_j, making the
  replacement and residual identities consistent. It tracks basepoints,
  finite shrinking and pullback restrictions, and the final permutation
  sigma = tau_n ... tau_1. Expanding the residual identity gives
  F_n = sigma F P_1^(-1) ... P_n^(-1) = id, hence sigma F = P_n ... P_1.
- **Lemma 12.5.1:** keeps the finite-component/support argument and supplies
  actual fiber endpoints alpha, beta and their minimum/maximum images.
  Theorem 9.4.6 is cited; the decreasing case explicitly reverses the limits
  via the absolute derivative.
- **Example 11.5.13:** the finite binomial coefficient bound c_j <= 4^j and
  a geometric series prove convergence for |z| < 1/2. No general infinite
  binomial theorem is invoked. Analytic Lagrange inversion remains an
  explicitly unproved optional analytic result.
- **Proposition 13.10.9:** identifies the central face of R' x [-delta,delta],
  its relative boundary neighborhood under the straightening chart, and
  convexity of the rectangle for the Lipschitz estimate.
- Selected drafting prose is repaired in Chapters 3, 7, 10, 11 and Appendix B.
  The Appendix B constructive argument is retained.
- Both README standing dependency sections distinguish the manifold
  refinement actually used in Chapter 13 from the optional unproved
  Chapter 9, 11 and 12 previews. The manuscript attribution note already
  states these distinctions and remains consistent. Version/date metadata
  and the README revision summary are synchronized.

No revised proof relies on later material. The finite Euclidean partition
of unity retains its extra eta cutoff. The inverse-function, constant-rank,
structural substitution, Jordan-boundary and Stokes proof architectures are
unchanged. Optional normed-target commentary and a new exercise were omitted.
The open-set length proof already contains the finite endpoint-sorting
argument, so no extra lemma was needed.

## Build and reference validation

- Three pdfLaTeX passes completed successfully; final PDF: **365 pages**.
- SHA-256 hashes of main.aux, main.toc and main.out agree across the final
  two passes.
- **450 labels**, **472 reference uses**, **20 bibliography entries**.
- No duplicate labels, unresolved references or undefined citations.
- No LaTeX/package warnings, missing PDF destinations, or overfull/underfull boxes.
- Numeric theorem-link audit: **407 of 407** labeled statement destinations
  land on a page containing the correct statement type and number. This
  includes the previously repaired targets; the existing anchor safeguards
  are preserved.
- All **730 internal links** have existing named destinations.

## Visual review

Rendered and inspected 20 physical PDF pages:
1, 2, 178, 179, 205, 206, 228, 229, 230, 232, 233, 234, 235,
263, 264, 265, 317, 318, 364, 365.

These include the title/version, rank–minor proposition, differentiating
limits, Lagrange inversion example, primitive-map explanation and complete
factorization proof, finite Euclidean localization, primitive substitution,
smooth-domain Jordan measurability, and attribution/dependency material.
No clipping, overlap, broken equations or displaced theorem headings was
observed. README version and standing dependency sections were reviewed in
source form.

Machine-readable checks and rendered review sheets are retained under
`tmp/revision361/`; the corresponding audit scripts are under `tmp/`.

</details>

<a id="historical-revision-audit"></a>
<details>
<summary>REVISION AUDIT</summary>

> Current revision: Version 3.4.1 (revision draft), September 12, 2026.
> The record below is historical. See [historical validation record](#historical-polish-3.4.1-audit)
> for the focused finishing patch and its validation.

# Pedagogical revision and verification

For the September 12, 2026, Version 2.0.0 revision, see
[historical validation record](#historical-major-pedagogical-audit).
The audit below records the earlier revision.

Revision: September 9, 2026, Version 1.3.0 (revision draft).

The revision preserves the two-part introductory course and its substantial
proofs. Changes concentrate on the construction of the reals, preparation
for multivariable analysis, and the route from classical integration to
general Stokes. The tracked chapter sources are authoritative; pre-existing
untracked backup copies and the older Part I/II audit files were left alone.

## Required mathematical corrections

| Original location or issue | Revised treatment and verification |
|---|---|
| Chapter 3, strict tail bounds | `lem:tail-estimates-classes` proves weak class bounds. The sequence 1-1/(n+1) exhibits the failure of strictness. Representative convergence reserves a rational half-tolerance. |
| Chapter 3, rational density | Both integer-part arguments now use the weak middle inequality. |
| Chapter 3, completeness | `thm:real-cauchy-complete` selects rational approximations within 1/j, proves rational Cauchyness, and uses convergence of representatives at the same index. A fixed enumeration makes the selections explicit. |
| Chapter 6, bounded uniform limit | Every approximating function is required to be bounded; the proof chooses a late one. The early-zero/later-identity counterexample explains the old failure. |
| Chapter 8, reciprocal | Direct difference quotient establishes reciprocal differentiability before the quotient rule. |
| Chapter 11, reciprocal | An exact algebraic remainder identity gives reciprocal differentiability without assuming it. |
| Chapter 10, composition | The composite is (2x+y,x+y); the expanded matrix product agrees. |
| Chapter 10, compactness | The existing proof already uses closures of tails and the finite-intersection argument correctly. It was audited and preserved. |
| Elimination dependency | `lem:elementary-factorization` proves the required factorization by induction and is cited in the linear-volume proof. |
| Boundary tangent spaces | Coordinate-pair equivalence gives the full n-dimensional tangent space, including outward vectors. Curve velocities are interpreted separately at interior points. |
| Open-overlap integration | `cor:compact-support-change-variables` localizes to finitely many cubes; `prop:open-form-invariance` applies it to arbitrary compact support on overlaps. |
| Half-space integration | `cor:halfspace-change-variables` uses interior cutoffs and vanishing strip errors. The manifold definition distinguishes artificial zero extension from genuine-boundary smooth extension. |
| Cantor dependency | Chapter 2 is explicitly an informal preview. `thm:cantor-formal` follows decimal existence and ambiguity in Chapter 4. Both later Thomae citations use it. |
| Cross-references | Symbolic labels are retained where possible. New dependencies use labels; source checks find no undefined or duplicate labels or unresolved bibliography keys. |

Additional corrections include distinct endpoint/sequence notation in
Bolzano–Weierstrass, a nonempty-space hypothesis for contraction, the
positive-cone math delimiter, explicit square-root existence before its
formal sequence uses, and fixed-degree hypotheses for the graded Leibniz rule.

## Pedagogical and dependency changes

- Foundations: a construction roadmap, finite-change lemma, explicit
  multiplication and reciprocal tolerances, positivity counterexample,
  bisection roadmap, and a distinction between first-pass understanding and
  reproducing every equivalence-class verification.
- Sequences and functions: decimal limits and ambiguity, immediate squeeze
  proof, consistent completeness-condition letters, localize-then-estimate
  example, monotone-inverse continuity, moving spikes, finite-binomial
  Bernstein examples, and explicit diagonal subsequence indexing.
- Series and calculus: M-test after absolute convergence with a geometric
  first example, alternating remainder/accuracy practice, endpoint synthesis,
  smooth cutoff with proof, tagged sums, and FTC extensions within Riemann theory.
- Linear algebra and derivatives: matrix computations, operator norms beside
  the other norms, permutation signs beside determinants, elimination,
  readiness checkpoint, polynomial remainder example, stronger directional
  counterexample, multilinear higher derivatives, Hessian caveats, and staged
  inverse/implicit-function arguments.
- Multiple integrals: clear Jordan section, countable versus finite null
  covers, integrable-section Fubini, graph-bounded regions, two intrinsic
  diagrams, explicit change-of-variables error roles, compact Jordan/open/
  half-space corollaries, and transfer exercises.
- Chapter 13: curves and two kinds of line integrals; Green for an explicitly
  restricted elementary class; patches, area, and flux; classical patch
  Stokes with the chain-rule calculation; only then exterior algebra, worked
  pullbacks, manifolds, partitions, and general Stokes. Coordinate and
  partition independence use the new analytic bridge. Classical consequences
  return as instances of the same theorem. Closed/nonexact forms remain a
  short perspective.

The critical dependency chain is now:

1. Chapter 8 smooth cutoff and Chapter 10 finite-dimensional estimates.
2. Chapter 11 chain rule, higher derivatives, contraction, inverse/implicit functions.
3. Chapter 12 Jordan integration and open/half-space changes of variables.
4. Chapter 13 classical patch calculus, pullbacks, local Stokes, coordinate invariance.
5. Explicit external refinement input, internal smooth partition construction,
   well-defined manifold integration, and general Stokes.

## Scope of the classical bridge

Green is proved for regions having both specified graph descriptions and
finite decompositions with cancelling shared arcs. Patch Stokes uses those
parameter regions and a regular injective C2 patch. The global smooth
surface and curved-boundary divergence statements are obtained only after
general Stokes. Boxes are treated facewise; a theory of manifolds with
corners or a separate surface-measure theory is not imported.

## References and unavailable material

The bibliography includes the requested Tao, Abbott, Ross, Pugh, Zorich,
Munkres (*Analysis on Manifolds*), Spivak (*Calculus on Manifolds*), Tu, and
Lee entries with short reading guidance. Lee's existing entry is broadened,
not duplicated. The attribution note continues to separate the one imported
refinement theorem from internally proved results.

Accessible reference checks included [Tao's book information](https://terrytao.wordpress.com/books/analysis-i/),
[Lee's author page](https://sites.math.washington.edu/~lee/Books/ISM/),
[Tu's text, especially the boundary and partition discussions](https://luis.impa.br/aulas/anvar/Tu_AnIntroductionToManifolds.pdf),
[Lebl's scope and reading material](https://www.jirka.org/ra/), and publisher
information for [Abbott](https://link.springer.com/book/10.1007/978-1-4939-2712-8),
[Ross](https://link.springer.com/book/10.1007/978-1-4614-6271-2), and
[Pugh](https://link.springer.com/book/10.1007/978-3-319-17771-7).
These checks are not a claim that every listed reference was available in
full. Arguments and exposition were worked out in the manuscript's notation.
The previously uploaded Chinese notes were not present among the accessible
repository or attachment files, so this revision does not claim to have
consulted them.

## Validation

- Repeated pdfLaTeX builds completed successfully; final PDF: 194 pages.
- Final auxiliary-reference stability checked across a further build.
- No undefined references, duplicate labels, unresolved citations, overfull
  boxes, or underfull boxes in the final build checks.
- Representative pages inspected from the Cauchy construction, decimals,
  cutoff, linear algebra, higher derivatives and inverse function theorem,
  graph-region/change-of-variables development, and each major new Chapter 13
  section. Visual inspection also caught and corrected the long Chapter 12
  running header and a diagram-label placement.
- Mathematical verification checked the changed hypotheses and proof
  dependencies, including tolerance choices, region regularity, chart support,
  orientation signs, and strip limits. This is mathematical review, not a
  machine-checked formal proof.
- README, outline, errata, bibliography, and cover metadata updated together.
- No tag, release, push, or publication performed.

Local build logs, reference-check output, and page renders are under the
ignored `tmp/` directory; they are not manuscript build dependencies.

## Subsequent focused pass

The September 11, 2026 revision supersedes the validation and foundation
organization above where affected. See [historical validation record](#historical-focused-revision-audit)
for the Chapter 5/10–13 changes, algebra-note adaptation, and final build checks.

</details>

<a id="historical-correction-record"></a>
<details>
<summary>Historical corrections formerly recorded in ERRATA</summary>

# Errata

## Focused proof-and-dependency patch — version 3.1.1, September 12, 2026

Added early continuity of composition; corrected the reciprocal example's
sequence domain and the elementary-series proof at zero. Infinite L'Hôpital
variants now use finite thresholds with a fixed auxiliary endpoint. Improper
limit comparison explicitly assumes finite-interval Riemann integrability.
The determinant proof's map definition is grammatical, and linear volume
scaling establishes intermediate measurability through inverse elementary
maps before using volumes (including degenerate rectangles).

Chapter 12's heading now matches its contents title. Chapter 13 constructs
one ambient extension near a compact coordinate support and proves that
smooth Euclidean domains are Jordan measurable and that their manifold and
Riemann integrals agree. Classical corollaries cite this bridge; the area
exercise assumes such a domain. Local prose fragmentation was reduced.
See [historical validation record](#historical-patch-3.1.1-audit) for validation and preservation checks.

## Focused dependency-and-exposition revision — version 3.1.0, September 12, 2026

- Replaced the implicit domain in the smooth-manifold-map definition with
  local charts and explicit image containment; continuity now follows visibly.
- Constructed manifold pullback, wedge, and exterior derivative, including
  chart and boundary-extension independence, before manifold integration.
  Added the zero-form-space convention above the dimension.
- Repaired lower/upper step-function values on shared grid faces. The
  integral proof still uses closed cells and Jordan-null modifications.
- Replaced the discarded-strip closure assertion with the covering and
  null-overlap properties valid even for exact multiples of the grid size.
- Added Jordan-set algebra for unions, intersections, and differences.
- Defined matrix addition/scaling and general-dimensional flux before use.
- Changed the operator-norm example to exhibit unequal exact norms, and
  updated duplicated exercises and separated surface definitions.
- Added concrete tensor applications and compatibility of the abstract
  exterior product with the shuffle product; retained their construction proofs.
- Corrected specific power-series references and harmonized attribution.
  Convergence remarks now acknowledge the proved one-dimensional Arzelà
  theorem without asserting its multivariable counterpart.
- Verified the closed sequence tails and compact-closure derivative maximum
  directly in the source; neither required mathematical alteration.

See [historical validation record](#historical-focused-dependency-audit) for implementation and validation details.

The following defects in the 1.2.0 source are corrected in the 1.3.0 revision
draft (2026-09-09). Locations below name results because numbering changes
in the revision. See [historical validation record](#historical-revision-audit) for the broader dependency audit.

| Location in 1.2.0 | Error | Correction |
|---|---|---|
| Chapter 3, tail-estimate lemma | Eventual strict bounds incorrectly passed to strict class bounds. | Prove weak bounds and reserve a margin for representative approximation. |
| Chapter 3, both rational-density arguments | Middle integer-part inequality was incorrectly strict. | Use the weak inequality. |
| Chapter 3, Cauchy completeness | Fixed-index argument did not ensure its anchor was in the Cauchy tail. | Use rational approximations within 1/j and the triangle inequality at the same index. |
| Chapter 6, uniform boundedness | One arbitrary early bounded function does not imply a bounded limit. | Require every approximating function bounded; select a sufficiently late one. |
| Chapters 8 and 11, quotient rules | Differentiability of the reciprocal was assumed while proving it. | Direct difference-quotient/remainder proofs precede the product rule. |
| Chapter 10, composition example | Composite disagreed with the displayed product matrix. | Composite is (2x+y,x+y). |
| Chapter 13, boundary tangent vectors | Two-sided curves inside the manifold do not realize the full boundary tangent space. | Define vectors by coordinate pairs and transition derivatives. |
| Chapter 13, chart integration | Rectangular reparametrization did not justify arbitrary compact support on chart overlaps. | Prove open-set and half-space compact-support change of variables, then coordinate independence. |

## Entry format

| Version affected | Location | Error | Correction | Date corrected |
|---|---|---|---|---|
| | | | | |

Use one row for each verified correction. Preserve earlier entries so that
readers can determine which versions are affected.

## Focused foundations revision — September 11, 2026

- Defined topological continuity before proving its metric equivalence;
  moved metric limit/completeness terminology before first use.
- Separated finite-net and cover-radius mechanisms in metric compactness;
  generalized the Lebesgue-number statement to arbitrary open covers.
- Closed linear-algebra dependencies: subspaces, span, exchange, coordinates,
  kernel/image, rank/nullity, coordinate changes, duality, and multilinearity.
- Replaced permutation-first determinant introduction with normalized
  alternating-form existence/uniqueness; added cofactors and efficient computation.
- Stated the zero-value condition for composed little-o remainders explicitly.
- Moved direct sums to Chapter 13; added elementary wedges before general
  wedge products. Kept tensor constructions optional and field-valid.


## September 12, 2026 — major pedagogical revision

- Replaced the early rationalization example's forward continuity dependency
  with a direct estimate and added function-limit laws.
- Strengthened the equicontinuity limit proposition to pointwise convergence.
- Proved both radius inequalities for power-series differentiation.
- Added the pointwise Arzelà bounded-convergence theorem, including absolute
  error integrals and the required integrability-of-limit hypothesis.
- Removed the repeated continuous-FTC proof and corrected lettered proof labels.
- Corrected the rectangle domain in the former Example 12.8.
- Rebuilt Jordan boundary/zero-extension arguments with open covers, compact
  margins, and fine grids; used the same mechanism for Jordan-null supports.
- Verified that the small-cube lemma takes maxima on the compact closure of N.
- Replaced the boundary-chart orientation definition with intrinsic tangent
  orientations and explicit coordinate signs, including both interval endpoints.

Result numbers change in this revision. Source labels and the regenerated PDF
provide the current references; the numbers above identify the earlier draft.


## Major proof-architecture revision — version 3.0.0, September 12, 2026

- Moved the interval Lebesgue-number and finite-subcover proofs before the
  open-set-length lemma used by Arzelà bounded convergence.
- Defined the repeated-input subspace R_2 before forming the second exterior
  quotient; quotient vector spaces now precede tensor constructions.
- Replaced the unreferenced nowhere-differentiability claim with the
  trigonometric-series continuity assertion actually proved in the text.
- Removed the stale Jordan-volume introduction after the multiple-integration
  limit theorems. Chapter 13's TOC title and chapter title now agree; its short
  running header is set separately.
- Moved finite direct-sum foundations to Chapter 10; Chapter 13 refers back
  instead of defining them again.
- Added smooth inversion of matrices and higher inverse/implicit regularity
  before the smooth-manifold transition.
- Preserved the correct closures-of-sequence-tails compactness argument and
  the compact-closure maximum in the nonlinear local change-of-variables lemma.
  Neither was an error requiring correction.

Other changes in this pass expand pedagogy and proof construction rather than
claiming the earlier formulas were false. See [historical validation record](#historical-proof-architecture-audit).

</details>


<a id="historical-revision-3.18.0-audit"></a>
<details>
<summary>Prior topology revision: preserved validation record</summary>

# Version 3.18.0 revision audit

Date: September 16, 2026. Baseline: the user's authoritative Version 3.17.0 working manuscript, including its pre-existing uncommitted changes. Final artifact: `main.pdf`, 398 pages.

## Preservation and scope

The pass changes existing chapter source only in Chapters 9, 10, and 13, adds Appendix C, and updates the main input list, version metadata, outline, and revision record. A source comparison against the working baseline confirms that all **388 existing proof environments** and all **585 existing theorem, lemma, proposition, corollary, and definition environments** remain verbatim. In the three edited chapters this includes all 137 original proofs. Other chapters, Appendices A and B, the preface, and references are unchanged.

Nine of the ten existing standalone figure sources are byte-for-byte unchanged. Only `torus-parameter-square.tex` is replaced, as requested. Seven new standalone vector figures explain Darboux gaps, relative balls, cylinder gluing, Möbius gluing and its single boundary, Klein-bottle gluing and the drawing's crossing, annular boundary orientation, and circle endpoint gluing.

Chapter 10 contains no quotient-topology development. The formal torus construction remains the product of circles. Appendix C is explicitly outside the main dependency route, and no existing main-route theorem or proof acquires an appendix dependency. The optional forward/backward vector/covector schematic was omitted because the existing prose and diagrams already explain that directionality.

## Mathematical and pedagogical checks

- Hausdorff motivation precedes the new diagonal criterion and the existing compact-subset theorem. Both directions of the diagonal proof explicitly use open product rectangles.
- The Darboux panels use the same function and partition. The marked oscillation and width multiply to the contribution to the upper-minus-lower gap.
- Relative openness is illustrated with a planar ball intersecting a line; the text requires fixing the ambient space.
- Torus edges use translation identifications. The angular rescaling, unit-square fibers, all-four-corner class, and product torus agree.
- Cylinder seams use `(x,t) -> (x+1,t)`; Möbius seams use `(x,t) -> (x+1,-t)`. The Klein bottle uses `(0,y) ~ (1,y)` and `(x,0) ~ (1-x,1)` throughout the text, figures, appendix, and orientation discussion.
- Identification arrows are explicitly distinguished from induced boundary-orientation arrows. Cylinder/Möbius boundary counts are two/one; torus/Klein have none.
- Non-orientability is justified by a sign reversal around a closed central loop, not by one negative transition in an arbitrary atlas. The torus has an explicit product-circle nowhere-vanishing top form independent of the appendix.
- Boundary and orientability are compared as independent properties. An orientable Möbius boundary circle is distinguished from an orientation induced by an oriented surface.
- The annulus shows outer counterclockwise and inner clockwise traversal, with outward transverse vectors pointing respectively away from the annulus and into the hole.
- The quotient universal property has the correct topology and continuity hypotheses. Compactness is obtained from compact domains or compact sets of representatives; Hausdorff targets are established before applying the continuous-bijection criterion.
- Cylinder/Möbius separation is proved using their explicit band distance. Small relative disks give seam, interior, and boundary charts; locally affine transitions and a countable basis are checked.
- The Klein-bottle construction checks a metric, small-disk charts, the four corner pieces, affine transitions, and a countable basis. The self-intersecting drawing is clearly labeled as a representation rather than an embedding.
- Projective-space representatives, open chart domains, normalized inverses, rational transition domains, the symmetric-idempotent trace-one projection model, compactness, Hausdorffness, and second countability are checked.
- No general quotient-manifold, covering-space, proper-action, orbifold, or bundle theory is introduced. The General Topology perspective refers to Appendix C and no longer duplicates its definition and circle argument.

## Compilation and document checks

The entire manuscript was compiled with the installed MiKTeX pdfLaTeX using `-interaction=nonstopmode -halt-on-error`. Repeated passes stabilized `main.aux`, `main.toc`, and `main.out`; their hashes remained unchanged after the final diagram-spacing build.

Final whole-document checks:

| Check | Result |
|---|---:|
| PDF pages | 398 |
| Source labels | 499 |
| Source reference occurrences checked | 519 |
| Duplicate labels | 0 |
| Missing references | 0 |
| Extracted-text unresolved `??` | 0 |
| LaTeX/package/PDF warnings | 0 |
| Overfull/underfull boxes | 0 |
| Internal links checked | 797 |
| Broken internal links | 0 |
| Numbered theorem/exercise destinations checked | 424 |
| Incorrect numbered destinations | 0 |

Rendered-page review covered every new or revised figure, the Hausdorff page, the gallery and orientation pages, every Appendix C page, the contents, and the preserved standalone geometric figures in their resulting placements. The Darboux oscillation marker was enlarged, the Klein crossing annotation and stage arrow were separated from labels, and the annulus orientation frame was moved away from its boundary. Captions remain attached and the new figures are referenced in surrounding prose.

Audit evidence and baseline snapshots are under [two historical path literals unavailable in the surviving intact record]. The automated checks establish structural and rendering consistency; the mathematical audit above is a direct review of the added arguments and their interfaces with the preserved manuscript. No Git commit, tag, or release was created.

</details>

### Historical release summaries consolidated from OUTLINE.md

Version 3.17.0 (originally 3.9.0) adds a peak-index monotone-subsequence theorem before
Bolzano–Weierstrass and uses one completeness cycle. The Part II geometry
thread connects affine hyperplanes, tangent and level planes, adapted
coordinates, spherical ball volume, sphere charts, and the product torus.
Section 13.17 retains additional unproved preview theorems; these are not
dependencies of the main development.

Version 3.19.0 makes Appendix C's constructions and proofs visibly staged,
adds local seam/corner diagrams and six exercises, and defines trace before its
projective-space use. Section 13.17 separates Algebraic Topology (after General
Topology) from De Rham Theory (after Differential Geometry). Homotopy, fundamental
groups, CW complexes, Euler characteristic, real singular homology/cohomology,
and the de Rham comparison remain optional previews, independent of Stokes.
See README.md for the corrected version-history mapping and all validation notes.

### Additional historical errata wording preserved during copy cleanup

The following wording supplements the consolidated correction record; obsolete
audit filenames below are historical references, not additional maintained files.

From `tmp/pre-architecture-2026-09-12/ERRATA.md`:

The following defects in the 1.2.0 source are corrected in the 1.3.0 revision
draft (2026-09-09). Locations below name results because numbering changes
in the revision. See REVISION-AUDIT.md for the broader dependency audit.

From `tmp/pre-focused-3.1.0/ERRATA.md`:

Other changes in this pass expand pedagogy and proof construction rather than
claiming the earlier formulas were false. See PROOF-ARCHITECTURE-AUDIT.md.


From `tmp/pre-focused-3.2.0/ERRATA.md`:

Chapter 12's heading now matches its contents title. Chapter 13 constructs
one ambient extension near a compact coordinate support and proves that
smooth Euclidean domains are Jordan measurable and that their manifold and
Riemann integrals agree. Classical corollaries cite this bridge; the area
exercise assumes such a domain. Local prose fragmentation was reduced.
See PATCH-3.1.1-AUDIT.md for validation and preservation checks.
