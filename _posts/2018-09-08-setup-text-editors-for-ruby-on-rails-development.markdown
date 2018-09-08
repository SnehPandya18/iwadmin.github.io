---
layout: post
title:  "Setup text editors for Ruby on Rails development"
date:   2018-09-08 10:24:25 +0530
tags: sublime atom visual-studio-code
author: Harshal Bhakta
---

Below are the configurations we use to setup our favorite text editors for [Ruby on Rails](https://rubyonrails.org/) development.

## Sublime Settings

<hr style="margin-bottom: 10px;">

Open your settings file by cliking on Preferences ▶ Settings menu item. Place the below configurations in the right-hand pane.

{% highlight json %}

{
  "tab_size": 2,
  "translate_tabs_to_spaces": true,
  "trim_trailing_white_space_on_save": true
}

{% endhighlight %}

## Visual Studio Code Settings

<hr style="margin-bottom: 10px;">

{% highlight json %}

{
  "editor.tabSize": 2,
  "editor.insertSpaces": true,
  "files.trimTrailingWhitespace": true
}

{% endhighlight %}

## Atom Settings

<hr style="margin-bottom: 10px;">

{% highlight yml %}

Settings -> Editor
  Tab Length: 2
  Tab Type: soft
Settings -> Packages -> Whitespace
  Remove trailing whitespace: Checked

{% endhighlight %}

## Reference Links

<hr style="margin-bottom: 10px;">

### Sublime

* [Main Website](https://www.sublimetext.com)
* [Settings](https://www.sublimetext.com/docs/3/settings.html)

### Atom

* [Main Website](https://atom.io/)
* [Settings](https://flight-manual.atom.io/getting-started/sections/atom-basics/)

### Visual Studio Code

* [Main Website](https://code.visualstudio.com)
* [Settings](https://code.visualstudio.com/docs/getstarted/settings)