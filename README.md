README
================

Broken pkgdown link example for [pkgdown](https://github.com/r-lib/pkgdown) issue [763](https://github.com/r-lib/pkgdown/issues/763).

To reproduce.

1.  Create new project (this) in RStudio
2.  Create this README.Rmd file
3.  Edit DESCRIPTION file and .Rbuildignore
4.  Create directory and file extras/example.md
5.  Set pkg docs in Github.
6.  knit README.Rmd
7.  Run pkgdown::build\_site() in R.

Observed: this link <https://github.com/JohnMount/BrokenLinkExample/blob/master/extras/Untitled.md> works in [README.md](https://github.com/JohnMount/BrokenLinkExample/blob/master/README.md) but is broken in [docs/index.html](https://johnmount.github.io/BrokenLinkExample/).

Expected: link to work both places (i.e. not be re-written from *.md to *.html).
