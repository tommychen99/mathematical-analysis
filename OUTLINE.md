# Manuscript outline and prerequisite map

Current revision: Version 3.33.0 — September 20, 2026.

## Front matter

1. Cover
2. Contents
3. Preface and AI-assisted-preparation disclosure
4. How to Read These Notes
5. Notation and Conventions

## Part I

### 1. Motivation and transition to analysis

1. Why informal infinitesimals and infinite sums require definitions
2. Preview: limits, completeness, continuity, derivative, integral
3. Failure examples and the role of hypotheses

Prerequisites: none.

### 2. Basic set theory, logic, functions, and relations

1. Sets, subsets, operations, and Cartesian products
2. Propositions, predicates, quantifiers, and negations
3. Methods of proof and induction
4. Relations, equivalence classes, and orders
5. Functions, images, inverse images, and inverse functions
6. The number-system chain \(\mathbb N\to\mathbb Z\to\mathbb Q\)
7. Cardinality; finite, countable, and uncountable sets
8. Axiom of choice and selected equivalents

Prerequisites: Chapter 1 only.

### 3. The real number system

1. Ordered fields, ordered-field maps, and complete ordered fields
2. The canonical ordered copy of $\mathbb{Q}$ in every ordered field
3. The Archimedean property and rational density in a complete ordered field
4. Uniqueness of complete ordered fields and the abstract characterization of $\mathbb{R}$
5. Cauchy sequences of rationals and their equivalence relation
6. Construction of addition, multiplication, order, and the rational embedding
7. Field and order axioms, Cauchy completeness, and the least-upper-bound property
8. Greatest lower bounds, nested intervals, and the link to equivalent completeness principles in Chapter 4
9. Decimal truncations and endpoint ambiguity; why Cauchy sequences anticipate completion

Prerequisites: Chapter 2. This construction must precede all uses of real completeness.

### 4. Sequences of real numbers

1. Definition and uniqueness of limits
   Revisiting Chapter 3's decimals through sequence convergence and the formal diagonal argument
2. Limit algebra and order preservation
3. Subsequences and monotone sequences
4. Monotone convergence and the sequential construction
   \(e=\lim_{n\to\infty}(1+1/n)^n\)
5. Cauchy sequences and completeness
6. Bolzano--Weierstrass
7. Limsup and liminf

Prerequisites: Chapter 3.

### 5. Limits and continuity of functions

1. Metric preliminaries on subsets of the real line
2. Limit points, isolated points, function limits, and sequential criteria
3. Asymptotic notation: meaning, vanishing, O/o calculus, and derivative remainders
4. Continuity at limit and isolated points; algebraic operations
5. Lipschitz continuity and uniform continuity
6. Intermediate values; general roots, elementary AM--GM, root laws, and positive rational powers
7. Compact intervals, extreme values, and uniform continuity

Prerequisites: Chapters 2--4.

### 6. Sequences and families of functions

1. Pointwise and uniform convergence
2. Uniform Cauchy criterion and uniform-limit theorem
3. Algebra and boundedness under uniform convergence
4. Counterexamples to unjustified interchange and Dini's theorem
5. Weierstrass approximation and the Stone--Weierstrass perspective
6. Equicontinuity and Arzelà--Ascoli on a compact interval

Prerequisites: Chapters 4--5; integration-dependent results await Chapter 9.

### 7. Infinite series

1. Numerical series with real terms
2. Canonical harmonic and square-reciprocal examples; positivity, comparison, ratio, root, and condensation tests; rational \(p\)-series using Chapter 5 powers
3. Absolute and conditional convergence; absolute invariance and conditional rearrangement
4. Power series and radius of convergence
5. Uniform convergence inside the radius; termwise differentiation in Chapter 8

Prerequisites: Chapters 3--6.

### 8. Differentiation

1. Derivative and basic rules
2. Local extrema, critical points, derivative tests, Rolle and mean-value theorems, implicit differentiation, and monotone discontinuities
3. Differentiating limits and power series
4. Higher derivatives and Taylor approximation: derivative matching, the MVT bridge, remainders, quantitative bounds, and the second derivative test
5. Continuous exponential/logarithm/real-power development: exp(1)=e, rational-power compatibility, hidden exponential limits, and hyperbolic functions
6. Analytic construction of \(\pi\), special-angle values, tangent, and inverse trigonometric functions with explicit domains and ranges
7. Elementary curves, ellipse and hyperbola parametrizations, and polar coordinates
8. Analyticity introduced at the smooth-cutoff opening: C^k and C^infinity versus real analyticity
9. Convexity, concavity, inflection points, Jensen, weighted AM--GM, Young, finite Hölder, and finite Cauchy--Schwarz

Prerequisites: Chapters 3--7. Elementary functions are constructed by power series; the smooth cutoff later supplies manifold bump functions.

Chapter 8 also introduces elementary plane curves, coordinatewise velocity
and speed, polar coordinates and quadrant selection, and the polar-motion
speed formula after trigonometry and inverse functions.

### 9. Riemann Integration

1. Partitions, Riemann sums, upper and lower sums; bound integration variables
2. Integrability criteria and algebra
3. Continuous and monotone functions; tagged fine-mesh sums; integral Hölder and Cauchy--Schwarz; uniform integration and Arzelà bounded convergence
4. Fundamental Theorem, inverse-trigonometric and inverse-hyperbolic antiderivatives, substitution, one trigonometric substitution, integration by parts, and the integral mean-value theorem
5. Improper integrals, the Integral Test, and an analytic rederivation of the real \(p\)-series test
6. Lebesgue criterion for Riemann integrability
7. Limits of Riemann theory; stated Lebesgue MCT and DCT, comparison with
   Dini and Arzelà bounded convergence, and absolute continuity/Lebesgue FTC

Prerequisites: Chapters 3--8.

## Part II

### 10. Necessary topology and linear algebra

1. Euclidean length and the default norm; distances, open and closed balls, and neighborhoods
2. Interior, closure, boundary, limit points, and the full closed-set characterization
3. Metric convergence, sequential characterizations, completeness of closed subsets, limits of maps, and continuity
4. Topological spaces, bases (including the I-adic example), second countability,
   neighborhood limits, first countability, sequential tests and their limitations,
   finite products, and componentwise convergence
5. Compactness: From Local Pieces to Global Control; Hausdorff uniqueness,
   closed points, the Zariski affine line, and the closed-diagonal criterion
6. Sequential Compactness, Total Boundedness, and a Common Scale
7. Connectedness and Paths
8. Vector Spaces, Bases, and Dimension
9. Finite Direct Sums
10. Linear Transformations, early `L(V,W)`/`L(V)` notation, affine maps, Kernels, and Images
11. Matrices as Coordinate Representations
12. Matrix Multiplication Comes from Composition; linear systems, row reduction, elementary matrices, and inversion
13. Changing Coordinates while Keeping the Map
14. Inner Products and Norms; standard coordinate norms and the Euclidean default
15. Bounded linear maps, equivalent operator-norm formulas, and finite-dimensional estimates
16. Covectors and Dual Spaces, Kronecker Delta and Dual Bases, Covector Pullback, and Multilinear Maps
17. Determinants and Orientation
18. Perspective and Transition

Prerequisites: Part I. No topology or linear algebra course is assumed.

### 11. Differentiation in finite-dimensional spaces

1. Chapter 10 metric results specialized through coordinate estimates; recalled Chapter 8 polar coordinates for radial limits; path tests; pointwise and uniform convergence; finite-dimensional Arzelà–Ascoli
2. Fréchet derivative and the role of an open domain; coordinates, directional derivatives, Jacobian columns as basis images, affine prediction, and the chain rule
3. Convex subsets and convex balls; mean-value estimates and differentiating limits; computable Hessians and higher symmetric multilinear derivatives, second-order chain rule, Taylor error bounds, smooth versus analytic regularity, and convex functions
4. Contraction method, the Euclidean open-ball trapping argument, operator-series perturbation, and smooth inversion on `GL(R^n)`
5. Normalized `C^k` inverse functions on invariant complete closed balls; linear and nonlinear implicit graph theorems; optional analytic Lagrange inversion
6. Rank persistence and the Constant Rank Theorem; immersions, submersions, regular level sets, multipliers, and dimension consequences
7. Primitive local factorization and finite Euclidean cutoffs and partitions of unity
8. Perspective and transition to structural integration

Coordinate projections define dx_i; Df(p) is the Euclidean derivative and
(df)_p is its value as an exact differential form.
The gradient represents it using the Euclidean inner product. Recalled curves,
curve chain rules, and level-set velocities stay in the first-order section.
Higher derivatives vary the base point; the proved bilinear rule supports
the second-order chain rule and its curved-path specialization.

Prerequisites: Chapter 10 and one-variable differentiation.

### 12. Riemann integration in several variables

1. Concrete grids, Darboux approximation, common refinement, continuous integrability, then owned-cell step functions
2. Continuous Riemann–Fubini first; lower/upper Darboux section integrals, general Darboux–Fubini, and the Thomae–Dirichlet exceptional-section example; coordinatewise FTC and integration by parts with face integrals
3. Jordan sets, finite versus countable null covers, and zero extension
4. Integrable-section Fubini and continuous graph-bounded planar regions
5. Linear change of variables; primitive substitution, composition, local factorization, and finite localization for compact support
6. Separate Jordan boundary control and compact-region recovery; optional inverse-map volume comparison and Schwartz perspective; half-space changes of variables
7. Polar coordinates and the orientation viewpoint
8. Uniform interchange, multivariable Arzelà bounded convergence, Dini, and comparison with Lebesgue theory

Prerequisites: Chapters 9--11.

### 13. Differential forms, Stokes' theorem, and manifolds

1. Parametrized curves and line integrals
2. Green's theorem in the plane
3. Parametrized surfaces and surface integrals
4. Classical Stokes for a parametrized surface patch
5. Beyond one parametrization: why manifolds? Visual vocabulary tour of charts, transitions, tangent/cotangent spaces, boundary, orientation, and smooth localization
6. Pointwise alternating multilinear algebra: covectors, elementary wedges, the coordinate basis proof, shuffles, and exterior algebra
7. Why differential forms? Scalars and differentials, general 1-forms and curve integration, flux 2-forms, general forms, pullbacks, and exterior derivatives
8. Integration and the local Stokes theorem
9. Charts, atlases, and smooth manifolds
10. Manifolds with boundary and smooth maps
11. Tangent and cotangent spaces
12. Differentials and differential forms on manifolds
13. Orientation and boundary orientation; nowhere-vanishing top forms
14. Partitions of unity and integration on manifolds; completion of the top-form equivalence
15. The general Stokes theorem
16. Classical theorems revisited
17. Perspective and further directions, including differential topology,
geometric topology, geometric analysis, and navigation to Appendices E–H

Prerequisites: Chapters 10--12. The partition-of-unity proof must precede global integration on manifolds.

## Structural appendices and continuations

Appendices A and B collect optional foundational and categorical language;
Appendices C–H provide optional mathematical extensions. None is intended
to be read before Chapter 1 or required for the main analysis-to-Stokes route.

### Appendix A: Foundations: Natural Numbers, Induction, and Choice
Peano structure on N₀; induction and recursion; the natural-number
well-ordering principle; choice, Zorn, and the Well-Ordering Theorem;
basis existence by maximal independent sets.

### Appendix B: Categories and Functors
Objects, morphisms, composition, isomorphisms, familiar categories,
covariant functors, contravariance and opposite categories, commutative
diagrams, and natural transformations. Forms and exterior differentiation
provide the central examples; cohomology points forward to H.

### Appendix C: Permutations and Determinants over a Field
Field distinctions, cycles, transpositions, parity, sign, inversions,
permutation matrices, determinant construction, Laplace expansion,
and characteristic-two alternation. Chapter 10 is independent of this appendix.

### Appendix D: Tensor Products and Exterior Powers
Quotient spaces, bilinear universal properties, binary construction,
associativity and symmetry, finite sums and products, induced maps, bases,
Tensor–Hom, exterior powers, determinant detectors, wedge multiplication,
duality, and agreement with Chapter 13. No category theory is required.

### Appendix E: Quotient Spaces, Gluing, and Classical Manifolds
Quotient topology and its universal property; compactness and separation;
circle, sphere, torus, cylinder, Möbius strip, Klein bottle, and projective
space, including seam/corner charts and local coordinate diagrams.

### Appendix F: Submanifolds
Adapted charts, graphs, immersions, submersions, embeddings, manifold rank,
regular values, tangent kernels, matrix constraints, intrinsic multipliers,
and the unproved Whitney perspective. Dependencies: Chapters 11 and 13.

### Appendix G: Lie Groups and Lie Algebras
Smooth groups, matrix examples, invariant fields, brackets (including a
nonzero computation), matrix tangent algebras, exponentials, and SO(2).
Dependencies: Appendix F and the analytic core; no general flow theorem.

### Appendix H: de Rham Cohomology
Chain/cochain complexes and maps; closed/exact quotient; induced pullbacks;
degree zero; star-shaped Poincaré lemma; puncture, circle and torus periods;
integration on cycles; exactness, Snake and Five Lemmas, long exact
sequences, Mayer–Vietoris, singular cohomology, and de Rham's theorem.
Dependencies: Chapter 13; examples connect to E, independently of F and G.
The categorical interpretation uses B; structural external theorems are marked.

### Appendix I: Hints for Selected Exercises
Optional hints organized by chapter and current exercise number. A superscript
asterisk links from the exercise to its hint; each entry links back. Early
proof chapters receive more guidance, with selective hints in Chapters 6–9.
This appendix adds no prerequisites and does not change Part II.

## Back matter

1. References and further reading
2. Errata maintained in the repository


Release history and validation records are maintained only in README.md.
