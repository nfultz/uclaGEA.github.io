---
layout: default
title: How to Contribute
---


The site is hosted on Github. Clone the [repo](https://github.com/uclaGEA/uclaGEA.github.io/), make edits, commit, and submit a pull request to have it merged.
All pages are written in markdown and use Just The Docs (JTD) for formatting. JTD uses particular YAML headers.
You can either find these on other pages or use the [Just The Docs documentation](https://just-the-docs.github.io/just-the-docs/). 
To start a new page, create a new markdown file. You can use another page as a template. Put the page in a folder if you want it to have a parent.

```
git clone https://github.com/uclaGEA/uclaGEA.github.io/
# make your edits...
git add --all
git commit -a -m 'write your commit message'
git push
git request-pull
```


### Building Locally

Before pushing to github, you can run the site on your computer to make sure your contributions look as you'd expect. The main GEA site and Wiki are built with Jekyll. Since just-the-docs, the template used to build the wiki, requires ruby you can skip installing Jekyll and just install ruby.[^1] On a mac:

```
brew install ruby
```

Navigate to the website's parent directory, get dependencies, and build. Be sure to specify both `_config.yml` files to build both the main site and Wiki.

```
bundle install                                                    # get dependencies
bundle exec jekyll serve  --config _config.yml,docs/_config.yml   # build
```




-------

[^1]: I think one needs ruby because the just-the-docs theme is distributed as a ruby gem. Have not tried running `jekyll serve` directly without ruby.

[website]: https://github.com/uclaGEA/uclaGEA.github.io
