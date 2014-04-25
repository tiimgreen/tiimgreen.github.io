---
layout: post
title: "Git Aliases"
date: 2014-04-25 21:35:00
categories: open-source git
image: /assets/images/mac_and_glasses.jpg
dark: true
---

Git provides tonnes of useful features, one of which being git aliases. This allows you to type:
{% highlight bash %}
$ git ac -m 'Initial Commit'
$ git p
$ git ph
{% endhighlight %}

Instead of:
{% highlight bash %}
$ git add .
$ git commit -m 'Initial Commit'
$ git push
$ git push heroku master
{% endhighlight %}

Which may not seem like a huge amount of time shaved off, but when a lot of commits/pushes are being made it is very useful.

My git aliases include:

.gitconfig
{% highlight text %}
[alias]
  co = checkout
  st = status -sb
  cm = commit
  p = push
  ph = push heroku master
  a = add -A .
  ac = !git add -A && git commit
  slog = log --all --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit --date=relative
{% endhighlight %}

For more information on Git Aliases take a look at my [GitHub Cheat Sheet](https://github.com/tiimgreen/github-cheat-sheet#aliases).
