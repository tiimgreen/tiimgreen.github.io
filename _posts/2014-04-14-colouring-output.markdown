---
layout: post
title: "Colouring Outputs to the Console in Ruby"
date: 2014-04-14 17:47:00
categories: ruby open-source gem
image: /assets/images/dark_items.jpg
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

À la:

![Toc](http://i.imgur.com/QraO0h9.png)

And it's as simple as that, the code can be found [here](https://github.com/tiimgreen/toc).

Making Toc was the first time I used the `define_method` function in Ruby. Indeed, it was the first time I had used meta-programming at all. In the future, I hope to use something like [Slop](https://github.com/leejarvis/slop) to add more functionality to my gems and take inputs from the user.
