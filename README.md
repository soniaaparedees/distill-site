# ECON 650 Distill Website

Personal course website and presentation for ECON 650 at San Diego State University.

**Live site:** https://soniaaparedees.github.io/distill-site/

## Pages

- `index.Rmd` - Home page
- `about.Rmd` - About page
- `slides.Rmd` - Distill wrapper for the embedded presentation
- `in_class_exercise_8_paredes_sonia.Rmd` - In-class exercise
- `presentation_paredes_sonia.qmd` - Quarto Reveal.js presentation source

## Project layout

- `_site.yml` - Distill website configuration and navigation
- `styles.css` - Shared presentation and site styling
- `images/` - Images and GIFs used by the source documents
- `references.bib` and `chicago-author-date.csl` - Presentation references and citation style
- `docs/` - Generated website published by GitHub Pages
- `presentation_paredes_sonia_files/` - Generated Quarto presentation dependencies

The `docs/` directory is the deployment output and should be committed so GitHub Pages can serve it. Most project files in the repository root are authoring sources.

## Build the website

Open `distill-site.Rproj` in RStudio, then run:

```r
install.packages("distill")
distill::render_site()
```

Render the standalone Reveal.js presentation from the terminal with:

```bash
quarto render presentation_paredes_sonia.qmd
```

After rendering, commit and push the updated source and `docs/` output files.
