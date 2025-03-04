# RUB-ML Publications

This repository contains all publications by the [Chair for Machine Learning at the Ruhr University Bochum](https://informatik.rub.de/ml/).

## How to add publications
1. Fork this repository.
2. Add your publication to `publications.bib`.
3. If there is not yet a macro defintion for the conference/journal of your publications, add it to `macros/conferences.bib` or `macros/journals.bib`.
4. Create a pull request.

## Formating guidelines
Each entry should contain (only) the following fields:
- `author` (always use the same spelling)
- `title` (to enforce a certain capitalization, use double curly braces, e.g. `{{ImageNet}}: A Large-Scale Hierarchical Image Database`)
- `year`
- `booktitle/journal` (always use a macro)
- `url` (preferably `https://doi.org/...`)

Of course, other entry types (e.g., `@techreport`) might require different fields. However, always try to keep it minimal. See if the type you need already exists in `publications.bib` and use the same formatting.

The following formatting is automatically applied when pushing your changes, so you don't have to take care of it:
- macro definitions are sorted alphabetically
- publications are sorted by year and author
- citation keys are constructed from first author, year, and the beginning of the title
- fields are ordered
- the file `publications_expanded.bib` is created, which contains expanded macro definitions

## Other recommendations
- if a paper is already published, use the URL to the published version (instead of a preprint)