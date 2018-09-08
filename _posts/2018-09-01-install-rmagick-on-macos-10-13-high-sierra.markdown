---
layout: post
title:  "Install RMagick on macOS (10.13) High Sierra"
date:   2018-09-01 10:24:25 +0530
tags: ruby rmagick ruby-on-rails
author: Harshal Bhakta
---

## Installation

<hr style="margin-bottom: 10px;">

Follow the below steps to successfully install [RMagick](https://rubygems.org/gems/rmagick) on macOS High Sierra. Enter all below commands into the Terminal.

### Install Homebrew

Check if brew is already installed by executing "$ brew -v". If you get "-bash: brew: command not found", execute the below command to install brew. Else, skip to the next step.

{% highlight bash %}

/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

{% endhighlight %}

### Install pkg-config

Check if pkg-conf is already installed by executing "$ pkg-config --version". If you get "-bash: pkg-conf: command not found", execute the below command to install pkg-conf. Else, skip to the next step.

{% highlight bash %}

brew install pkg-config

{% endhighlight %}

### Install imagemagick@6

{% highlight php %}

$ brew uninstall imagemagick
$ brew uninstall imagemagick@6
$ echo 'export PATH="/usr/local/opt/imagemagick@6/bin:$PATH"' >> ~/.bash_profile
$ source ~/.bash_profile

{% endhighlight %}

### Install RMagick

{% highlight php %}

$ gem install rmagick

{% endhighlight %}

## Reference Links

<hr style="margin-bottom: 10px;">

* Homebrew: [https://brew.sh/](https://brew.sh/)
* pkg-config: [https://www.freedesktop.org/wiki/Software/pkg-config/](https://www.freedesktop.org/wiki/Software/pkg-config/)
* ImageMagick: [https://www.imagemagick.org](https://www.imagemagick.org)
* RMagick: [https://rmagick.github.io/](https://rmagick.github.io/)