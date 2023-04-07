---
layout: default
title: Site Maintenance
---

We use Git and Github. Clone the [website], make edits, commit, and submit a pull request to have it merged.



### Building Locally

The main GEA site and Wiki are built with Jekyll. Since just-the-docs, the template used to build the wiki, requires ruby you can skip installing Jekyll and just install ruby.[^1] On a mac:

```
brew install ruby
```

Navigate to the website's parent directory, get dependencies, and build. Be sure to specify both `_config.yml` files to build both the main site and Wiki.

```
bundle install
bundle exec jekyll serve  --config _config.yml,docs/_config.yml
```



-------

[^1]: I think one needs ruby because the just-the-docs theme is distributed as a ruby gem. Have not tried running `jekyll serve` directly without ruby.

[website]: https://github.com/uclaGEA/uclaGEA.github.io
