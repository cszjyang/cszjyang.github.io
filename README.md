# Zhijun Yang's Academic Homepage

Static source for <https://cszjyang.github.io/>. The homepage is maintained in
`index.html`.

## Repository layout

```text
index.html                       Homepage and publication links
publications/                    Downloadable publication materials
  2026/
    forge/
      OSDI26-FORGE-paper.pdf
      OSDI26-FORGE-slides.pdf
    xtra/
      SOSP26-XTRA-paper.pdf
      SOSP26-XTRA-slides.pdf
resume_en/                       English CV source and compiled PDF
resume_cn/                       Chinese CV source and compiled PDF
```

## Publication naming convention

Keep all materials for a publication together under its publication year and
project name:

```text
publications/<year>/<project-slug>/<VENUE><yy>-<Project>-<type>.pdf
```

- Use the publication year, rather than the upload year: four digits in the
  directory and two digits after the venue abbreviation in the filename.
- Keep project directory names lowercase, such as `forge` and `xtra`.
- Use uppercase venue abbreviations and preserve the project's original case in
  filenames, such as `OSDI26-FORGE`, `SOSP26-XTRA`, or `FAST27-CloverRec`.
- Use ASCII letters, numbers, and hyphens in names. Avoid spaces, underscores,
  and non-ASCII names. Match filename case exactly in homepage links.
- Use `paper` for the paper and `slides` for the presentation. Additional material
  can use a descriptive type such as `poster` or `supplement`.
- Include the year, venue, project, and type in each filename so that downloaded
  files remain identifiable outside this repository.
- When replacing a document with a revised version, keep its published path
  stable. Git preserves previous versions; avoid suffixes such as `final` or `v2`.

## Adding or updating a publication

1. Create `publications/<year>/<project-slug>/` and place the PDFs there using the
   naming convention above.
2. Update the publication entry in `index.html`. Use paths relative to the
   repository root, and list available links in the order `Paper`, `Slides`,
   `Code`. For example:

   ```html
   [<a href="publications/2026/forge/OSDI26-FORGE-paper.pdf">Paper</a>]
   [<a href="publications/2026/forge/OSDI26-FORGE-slides.pdf">Slides</a>]
   [<a href="https://github.com/cszjyang/forge">Code</a>]
   ```

3. Preview from the repository root with `python3 -m http.server 8000`, open
   `http://localhost:8000/`, and check that each new link opens the intended PDF.
4. Review the changes, then commit and push the PDFs and homepage links together.
