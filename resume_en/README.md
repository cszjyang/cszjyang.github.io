# Zhijun Yang — Academic Resume

This directory contains the one-page English academic resume intended for
conference scholarships and similar academic applications.

## Files

- `resume.tex`: resume source.
- `resume.pdf`: compiled submission copy.
- `Makefile`: reproducible PDF build.
- `LICENSE`: license for the adapted layout.

## Build

Run:

```bash
make
```

The build uses XeLaTeX and runs it twice so that PDF metadata and hyperlinks
are finalized.

## Content conventions

- Publications use full author lists, with Zhijun Yang in bold.
- Accepted camera-ready papers are marked `to appear`.
- Published papers link to their official publication pages and code.
- The resume intentionally omits phone number, photo, Google Scholar,
  publication acceptance rates, performance figures, and generic skill lists.

## Template

The single-column layout is adapted from
[Jake's Resume](https://github.com/jakegut/resume), which is distributed under
the MIT License. The academic sections and publication layout are customized
for this resume.
