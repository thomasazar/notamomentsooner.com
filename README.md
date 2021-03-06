# notamomentsooner.com

[![Netlify Status](https://api.netlify.com/api/v1/badges/07c4efd5-cc31-410e-9968-e812486f3703/deploy-status)](https://app.netlify.com/sites/vigilant-northcutt-2faf9d/deploys)

The website for Not a Moment Sooner, dedicated to promoting the future health and viability of the Upstate theatre community and its artists.

## Project Organization

This site is built using [Hugo](https://gohugo.io/), a static site generator written in Go.

- **assets** include SCSS/CSS, Javascript, SVGs, and image files that use Hugo's [image processing functions](https://gohugo.io/content-management/image-processing/).
- **content** are the individual pages, written in Markdown.
- **data** contains a single YAML file with collected signatures for the letter.
- **layouts** are where a lot of the heavy lifting occurs:
  - **_default** contains the basic HTML templates of the pages
  - **partials** are called within templates to execute certain pieces of logic, most notably the sorting of names (by last name for invididuals, first letter for organizations)
  - **shortcodes** are called within Markdown files to insert smaller template pieces, like forms and signature lists
- **resources** are compiled CSS and Javascript automatically generated by Hugo; they are included in the repo to speed up build time
- **static** contains webfonts and images that do not use Hugo image processing features

The project is built and hosted using [Netlify](https://www.netlify.com/).
