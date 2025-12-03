# Quarto Reveal.js CAU Theme

A Quarto Reveal.js presentation template for Chung-Ang University (CAU).

Based on [quarto-revealjs-ubd](https://github.com/haziqj/quarto-revealjs-ubd) by Haziq Jamil.

## Features

- CAU branding (logo, background images)
- Multiple authors with affiliation footnotes
- Slide numbering (hidden on title slide)
- Table of contents support
- MathJax for equations
- Atkinson Hyperlegible font

## Installation

```bash
quarto use template namenguiin/quarto-revealjs-cau
```

This will create a new directory with the template files.

## Usage

### Basic YAML Header

```yaml
---
title: "Your Presentation Title"
subtitle: "Subtitle"
author:
  - name: Author Name
    affiliations:
      - ref: affil-1
affiliations:
  - id: affil-1
    name: Your Institution
advisor: "Prof. Advisor Name"
date: today
format:
  cau-revealjs:
    toc: true
---
```

### Multiple Authors with Affiliations

```yaml
author:
  - name: First Author
    affiliations:
      - ref: cau
  - name: Second Author
    affiliations:
      - ref: cau
      - ref: other
affiliations:
  - id: cau
    name: Department of Physics, Chung-Ang University
  - id: other
    name: Another Institution
```

Result: First Author¹, Second Author¹ˑ² with footnotes below.

## Preview

```bash
quarto preview template.qmd
```

## License

MIT License - see [LICENSE](LICENSE) for details.

## Credits

- Original theme: [haziqj/quarto-revealjs-ubd](https://github.com/haziqj/quarto-revealjs-ubd)
- Modified by: Hyungkeun Nam
