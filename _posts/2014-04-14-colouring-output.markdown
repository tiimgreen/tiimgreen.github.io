---
layout: post
title: "Colouring Outputs to the Console in Ruby"
date: 2014-04-14 17:47:00
categories: ruby open-source
image: https://camo.githubusercontent.com/be9fb8e0e5ff44513676a3e9f0941dd183da3ee6/687474703a2f2f692e696d6775722e636f6d2f4234546b3362302e706e67
dark: true
---

# The Console - Enlightened

[Toc](http://github.com/tiimgreen/toc) is a simple, lightweight gem to colour outputs to the console.

It can be installed by running:

{% highlight bash %}
$ gem install toc
{% endhighlight %}

Admittedly, Toc isn't that good. It's my first Ruby Gem and I didn't really have a clue, but it works. And it looks nice. It works like this:

Colours available:

- Black
- Red
- Green
- Yellow
- Purple
- Pink
- Light Blue

To make the current text coloured:
{% highlight ruby %}
puts 'Hello World'.red
{% endhighlight %}

If you want to add a background:
{% highlight ruby %}
puts 'Hello World'.red_on_black
{% endhighlight %}

And it's as simple as that, the code can be found [here](https://github.com/tiimgreen/toc)
