# greenpaper
Green Paper: A Community-Driven Technical Specification for Neo Blockchain

## document format
The base document started as pure LaTeX, as usual in academic publications, however the syntax is not considered as friendly as Markdown. So, why not merge both? :)
In order to facilitate the contributions to the document, we decided to adopt pandoc format, which allows hybrid LaTeX + Markdown syntax.

### base structure
The structure of the document consists of four files:
- green_paper.md : main document in Mardown + LaTeX (contributors should focus on this file)
- metadata.yaml : document metadata (authors, abstract, ...)
- greenpaperstyle.pandoc : document style (LaTeX headings)
- template.tex : base LaTeX template (pandoc default LaTeX template with small changes)

## build instructions
Install pandoc and LaTeX base. On debian-based linux, you can simply run `make install`, and all dependencies will be installed.

After pandoc and LaTeX base are available, you can simply run `make`, which will generate the green paper pdf.

## How to contribute
If you know Neo technology and want to contribute, feel free to directly submit a Pull Request with the desired changes.
Initially, the idea is to create a broad and complete initial version of the document, which will be polished in the future.

## License
This repository is currently MIT Licensed, but will soon migrate to a corresponding Creative Commons license (since it's more about text than code).

Copyleft 2018-2019
