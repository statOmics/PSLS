# Rmd-website

<!-- Badge to show GHA rendering status: adapt URL to your own repo! -->

[![Render and Deploy](https://github.com/statOmics/Rmd-website/workflows/Render%20and%20Deploy/badge.svg)](https://github.com/statOmics/Rmd-website/actions)


An RMarkdown-based website rendered using GitHub Actions

https://statomics.github.io/Rmd-website/


## Getting started

1. Create a new repository on GitHub based on this [template][GH-template] (press the big green button __"Use this template"__)
2. Clone the repository locally
3. Add content in [R Markdown](http://rmarkdown.rstudio.com) format
4. Commit changes and push to GitHub
5. The website will be deployed at `https://<username>.github.io/<repo-name>/`

## Managing the R enviromnent with `renv`

This project uses [__*renv*__](https://rstudio.github.io/renv) to maintain a consistent environment of R packages.
For the full documentation, see https://rstudio.github.io/renv.

Briefly:

1. Install necessary packages with `renv::install()` and use them somewhere in the project as usual
2. Call `renv::snapshot()` to save the state of the project library to the lockfile (called `renv.lock`)
3. Continue working on your project, installing and updating R packages as needed
4. Call `renv::snapshot()` again to save the state of your project library if your attempts to update R packages were successful, or call `renv::restore()` to revert to the previous state as encoded in the lockfile if your attempts to update packages introduced some new problems

## Examples

- [High Dimensional Data Analysis course](https://github.com/statOmics/HDA2020)
- [StateSpaceCrypto talk](https://github.com/statOmics/StateSpaceCrypto)

## Getting help

- <https://github.com/r-lib/actions#where-to-find-help>
- For open questions, suggestions, ideas,...: use [GitHub discussions](https://github.com/statOmics/Rmd-website/discussions)
- For technical issues: [post an issue](https://github.com/statOmics/Rmd-website/issues)

## More info

- [R Markdown: The Definitive Guide](https://bookdown.org/yihui/rmarkdown/)
- [GitHub Actions for R](https://www.jimhester.com/talk/2020-rsc-github-actions/)
- [GitHub Actions: workflows and examples by r-lib](https://github.com/r-lib/actions)
- [rstudio4edu](https://rstudio4edu.github.io/rstudio4edu-book/)

[GH-template]: https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/creating-a-repository-from-a-template
