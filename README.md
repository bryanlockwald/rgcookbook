# rgcookbook

![R Graphics Cookbook Cover](cover.jpg)

Source code for the R Graphics Cookbook, 2nd edition.

* [Read online](http://r-graphics.org)
* [Buy on Amazon](https://www.amazon.com/dp/1491978600)

## About this fork

This is a fork of [wch/rgcookbook](https://github.com/wch/rgcookbook) that converts the source from R Markdown / bookdown to Quarto. 

- All `.Rmd` files have been renamed to `.qmd`
- Cross-references use Quarto syntax (`@fig-*`, `@tbl-*`, `@sec-*`) instead of bookdown's `\@ref()` syntax
- Chunk options use the `#|` YAML style instead of inline knitr options
- The project builds with `quarto render` rather than `bookdown::render_book()`
- A `_quarto.yml` project file replaces `_bookdown.yml` and `_output.yml`

The book content itself is unchanged. Any additions are my own personal notes.

I keep this fork in my Obsidian vault so the rendered HTML book lives on my local machine as a searchable reference while I work in R. If you want to do the same, clone the repo into your vault, open the folder in RStudio, and run `quarto render` from the terminal.

The original book citation: Chang, Winston. 2018. _R Graphics Cookbook: Practical Recipes for Visualizing Data_. Second edition. Beijing; Boston: O'Reilly.
