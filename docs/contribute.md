---
layout: default
title: How to Contribute
---

### Downloading and Uploading your Edits

We use Git and Github. Clone the [repo](https://github.com/uclaGEA/uclaGEA.github.io/), make edits, commit, and submit a pull request to have it merged.

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
