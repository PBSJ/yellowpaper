# greenpaper
Green Paper: A Community-Driven Technical Specification for Neo Blockchain

## document format
The base document started as pure LaTeX, as usual in academic publications, however the syntax is not considered as friendly as Markdown. So, why not merge both? :)
In order to facilitate the contributions to the document, we decided to adopt pandoc format, which allows hybrid LaTeX + Markdown syntax.

### base structure
The structure of the document consists of four files:
- green_paper.md : main document in Mardown + LaTeX (this file is automatically generated by `merge_sections.sh`)
- metadata.yaml : document metadata (authors, abstract, ...)
- greenpaperstyle.pandoc : document style (LaTeX headings)
- template.tex : base LaTeX template (pandoc default LaTeX template with small changes)

Green Paper sections are separated on `sections/` folder (these are used as source to generate `green_paper.md` file).

## build instructions
Install pandoc and LaTeX base. On debian-based linux, you can simply run `make install`, and all dependencies will be installed.

After pandoc and LaTeX base are available, you can simply run `make`, which will generate the green paper pdf.

### building specific section
Any section can be build using command `make section` and passing `SECTION` parameter.
For example: `make section SECTION=08_dBFT` will build section 08.

## How to contribute
If you know Neo technology and want to contribute, feel free to directly submit a Pull Request with the desired changes.
Initially, the idea is to create a broad and complete initial version of the document, which will be polished in the future.

## License
This repository is currently MIT Licensed (for text and code), and Free Culture license Creative Commons 4.0 International (CC BY 4.0) for all figures and externally copyrighted material.

Please, when contributing, be careful to only add figures covered by Creative Commons licenses, and give proper references to original sources.
When adding new original material to this project, contributor agrees that it will be covered by Free Culture license Creative Commons [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).

Copyleft 2018-2019

From Neo Community to You
