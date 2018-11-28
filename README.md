<p align="center">
  <img width="300" src="assets/haarlem-open-source-logo.svg">
</p>

# [`haarlem.github.io`](https://haarlem.github.io/)

[![Powered by Jekyll](https://img.shields.io/badge/powered_by-Jekyll-blue.svg?style=flat-square)](https://jekyllrb.com/)
[![Published on GitHub pages](https://img.shields.io/badge/published_on-GitHub_pages-green.svg?style=flat-square)](https://pages.github.com/)

> A showcase of Gemeente Haarlem's Open Source, a guide on how to contribute and our vision how software should be built.

The goal of this project is to enable other local governments to learn from, reuse and contribute to the software maintained by us.

Using built-in-to-GitHub static site generator Jekyll the content of this repostitory automatically builts into the website that can be found at [`haarlem.github.io`](https://haarlem.github.io/). This means updating this page means just updating the files in this repository through standard pull requests.

---

## Adding content

Feel free to make pull requests, we'll review and merge them as soon as we can. Feel free to edit the MarkDown files, if you are unfamilliar with this, the [Mastering MarkDown](https://guides.github.com/features/mastering-markdown/) guide is pretty good

Be sure to read the [CONTRIBUTING.md](CONTRIBUTING.md) for more information on contributing.

### Adding a Guide

We believe that sharing our knowledge will help the development of great Open Source software for Haarlem and the world.

Our guides are for everyone, whatever their affiliation. They should be general, understandable for ‘beginners’ and not contain too much technical detail. The content of this website should be broadly applicable to every one of our projects, and thus not feature 'style guides' etc, those are better at home with projects in their repositories.

To add a guide just make a new markdown file in `/guides/`. In order to give your guide the right subtitle on the guides page you should add the `explains` in the [Jekyll front matter](https://jekyllrb.com/docs/frontmatter/). Keep the `explains` short and simple to understand.

```yaml
---
explains: How to add guides, add pages and change this website
---
```

### Adding a Project

To add a project just make a new markdown file in `/projects/`. Add an `abstract` in the front matter as a short description of what the product is.

You can either make a new Project page on this site or link directly to an external repo or product page by adding a `link` property to the front matter.

```yaml
---
title: Zaakregistratiecomponent
abstract: Component for storing and serving 'cases' compliant with the GEMMA RGBZ, RSGB and ImZTC standards.
tags: hlm # Add HLM for it to be added to the HLM overview on the HLM page
hlmLayers: 4 5 # The layers in the HLM architecture that this project touches seperated by spaces
---
```

---

## Installing, running and building

This site and it's contents are served over [GitHub pages](http://pages.github.com) and built by it's native static site generator [Jekyll](http://jekyllrb.com).

More on [Jekyll as a static site generator with GitHub](https://help.github.com/articles/using-jekyll-as-a-static-site-generator-with-github-pages/).

### Installing locally

[Install Ruby and it's package manager Bundler](https://help.github.com/articles/setting-up-your-github-pages-site-locally-with-jekyll/) with 

```bash
gem install bundler
```

Install the dependencies and Jekyll using 

```bash
bundle install
```

### Running and serving locally

Run Jekyll, generate the site, watch for changes and serve over a local webserver with 

```bash
jekyll serve --livereload
```
