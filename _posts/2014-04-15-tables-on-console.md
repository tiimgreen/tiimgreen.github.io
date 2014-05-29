---
layout: post
title: "Writing Tables in the Console"
date: 2014-04-15 12:39:00
categories: ruby open-source gem
image: /assets/images/desk.jpg
---

# Formatted Tables in the Console

[Tabbit](http://github.com/tiimgreen/tabbit) is my second RubyGem. It allows you to write simple tables in the console as shown below:

![Tabbit](http://i.imgur.com/IckpkJZ.png)

tabbit.rb
{% highlight ruby %}
require 'tabbit'

# Pass headers as parameters:
table = Tabbit.new 'Name', 'Email', 'Phone No.'

# To add a row call the .add_row function, with each parameter being a column:
10.times do |n|
  table.add_row "Tim Green #{n}", "tiimgreen-#{n}@gmail.com", '123-456-789'
end

# To output the table to the console:
puts table.to_s
{% endhighlight %}

Tabbit was created purely as a means of learning Ruby and RubyGems, I learned a lot making it and to some, it might actually come in useful.

To install:
{% highlight bash %}
$ gem install tabbit
{% endhighlight %}
