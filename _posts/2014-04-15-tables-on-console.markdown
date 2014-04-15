---
layout: post
title: "Writing Tables in the Console"
date: 2014-04-15 12:39:00
categories: ruby open-source gem
image: /assets/images/desk.jpg
dark: true
---

# Formatted Tables in the Console

[Tabbit](http://github.com/tiimgreen/tabbit) is my second RubyGem. It allows you to write simple tables in the console as shown below:

![Tabbit](http://i.imgur.com/IckpkJZ.png)

To initialize a table create a new instance of `Tabbit`, passing in the name of the headers:

{% highlight ruby %}
require 'tabbit'

table = Tabbit.new('Name', 'Email', 'Phone No.')
{% endhighlight %}

Adding a row is as simple as:
{% highlight ruby %}
10.times do |n|
  table.add_row("Tim Green #{n}", "tiimgreen-#{n}@gmail.com", "123-456-789")
end
{% endhighlight %}

And to output the table:
{% highlight ruby %}
puts table.to_s
{% endhighlight %}

Tabbit was created purely as a means of learning Ruby and RubyGems, I learned a lot making it and to some, it might actually come in useful.
