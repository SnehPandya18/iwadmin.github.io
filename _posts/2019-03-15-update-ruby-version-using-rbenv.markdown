---
layout: post
title:  "Update Ruby version using Rbenv"
date:   2019-03-15 19:15:25 +0530
tags: ruby
author: Harshal Bhakta
---

Follow the below steps to update Ruby version. When upgrading Ruby, always check the latest version available on the [official website](https://www.ruby-lang.org/en/downloads/).

## Update ruby-build

<hr style="margin-bottom: 10px;">

Pull the latest version of ruby-build since that version would support installing the latest version of Ruby. When new versions of Ruby are released you need to update ruby-build to install those versions.

{% highlight bash %}

$ cd ~/.rbenv/plugins/ruby-build && git pull && cd -

{% endhighlight %}

## Install Ruby by specifying version number

<hr style="margin-bottom: 10px;">

{% highlight bash %}

$ rbenv install 2.6.2

{% endhighlight %}

## Set the new version as global version

{% highlight bash %}

$ rbenv global 2.6.2

{% endhighlight %}

## (Optional) Install bundler

If you are using Rails, you would want to install the latest version of bundler for the new Ruby version you just installed.

<hr style="margin-bottom: 10px;">

{% highlight bash %}

# Check the currently active Ruby version. If it's correct, proceed.
$ ruby --version
ruby 2.6.2p47 (2019-03-13 revision 67232) [x86_64-darwin18]
$ gem install bundler

{% endhighlight %}

## Reference Links

<hr style="margin-bottom: 10px;">

* [Ruby Official Website](https://www.ruby-lang.org)
* [Rbenv](https://github.com/rbenv/rbenv)
* [Ruby Build](https://github.com/rbenv/ruby-build)