# Lecture Notes on Mathematical Analysis

Repository: <https://github.com/tommychen99/mathematical-analysis>

## Single and Multivariable Calculus

**Author:** Tommy Chen  
**Current version:** Version 1.0.2
**Revision date:** August 23, 2026  
**Status:** Version 1.0.2 public release.

These notes give a rigorous introduction to real analysis and rebuild the
central ideas of calculus from modern foundations. Part I develops the real
numbers, sequences, limits, continuity, series, differentiation, and Riemann
integration. Part II develops the finite-dimensional topology and linear
algebra needed for multivariable analysis, followed by multivariable
integration, differential forms, manifolds, and the general Stokes theorem.

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
examples and explicitly labelled informal previews. Chapter 13 uses one
clearly marked external manifold-refinement theorem; all other principal
results are proved within the stated scope of the notes.

## Build

The project is designed for **pdfLaTeX**. From the repository root, run:

```text
latexmk -pdf main.tex
```

Alternatively, run `pdflatex main.tex` repeatedly until the table of contents,
cross-references, and bibliography stabilize. The project uses standard AMS
packages, `hyperref`, `cleveref`, `enumitem`, `xcolor`, and Latin Modern fonts.
The bibliography is written directly in LaTeX; no BibTeX or Biber step is
required. No absolute local paths, generated figures, or external downloads
are required to build the PDF.

## References and external dependencies

The document contains a short bibliography. The Chapter 13 refinement theorem
is explicitly identified as an external theorem used without proof and cites
John M. Lee's *Introduction to Smooth Manifolds*. The remaining bibliography
entries are further-reading references, not assertions that particular proofs
or prose were adapted from those works.

## AI-assisted preparation

OpenAI Codex was used extensively in drafting, revising, proofreading, and
preparing the LaTeX source for these notes. The author determined the scope
and mathematical organization, made the final decisions about retained
content, and is responsible for approving and verifying the correctness of the
published version. Codex is not listed as a coauthor.

Before publication, the author should verify any AI-authorship or disclosure
policy imposed by the intended university, repository, publisher, or platform.

## License and copyright

Copyright © 2026 Tommy Chen. This work is licensed under the
[Creative Commons Attribution 4.0 International License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).
You may share and adapt the notes under the terms of that license, with
appropriate attribution.

## Errors and errata

The notes may contain errors. Please report them through
[GitHub Issues](https://github.com/tommychen99/mathematical-analysis/issues)
or record them in [`ERRATA.md`](ERRATA.md).

## Release notes and versioning

Version 1.0 was released on August 23, 2026.

Version 1.0.1 expands L'Hopital's Rule to include the
infinity-over-infinity indeterminate form. Version 1.0.2 clarifies the
notation and basic terminology for suprema and infima.

For subsequent versions, use approximately `1.0.1` for minor corrections,
`1.1` for meaningful additions or improvements, and `2.0` for substantial
restructuring.
