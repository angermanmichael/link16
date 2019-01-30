#### Projects Michael is Working on in 2019

Michael Angerman Projects
http://stormasm.github.io/link16/

##### Part Zero

January 30, 2019

For now, stick with Ruby 2.5.3 as version 2.6.X is
broken with the new bundler...

Notes on how to use Ruby correctly

```
ruby --version
rvm list
rvm use 2.5.3
rvm current
rvm gemset list
rvm gemset create jekyll
rvm gemset use jekyll
rvm current
```

* On MacOs ruby comes preinstalled at */usr/bin/ruby*


##### Part I

```
git checkout gh-pages
rvm gemset use jekyll
rvm current

alias jekgo='jekyll serve -P 3000'
```

##### Part II

These are my jekyll github websites...

To run any one of them cd into one of these directories and type:

```
rvm gemset use jekyll
jekgo
```

assuming the jekyll gem is already installed...

If not then....

```
rvm gemset list
rvm gemset create jekyll
rvm gemset use jekyll
gem install bundler
bundle install
rvm current
```

##### Part III

If you want to start from scratch with just jekyll and not this repo.

We will keep the **jekyll** gemset in place and
create a new one called **jekyll2**

```
rvm gemset list
rvm gemset create jekyll2
rvm gemset use jekyll2
gem install bundler jekyll
jekyll new myblog
```

Then to run this web site simply type this command:

```
jekyll serve -P 3000
```
