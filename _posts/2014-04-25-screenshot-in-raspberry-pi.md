---
layout: post
title: "Taking Screenshots in the Raspberry Pi"
date: 2014-06-04 14:05:00
categories: open-source raspberry-pi
image: http://www.raspberrypi.org/wp-content/uploads/2012/03/Raspi_Colour_R.png
---

To take screenshots in the Raspberry Pi you'll need to install the gracefully named utility `scrot`. Not to be confused with a [Scrot](http://www.urbandictionary.com/define.php?term=scrot&defid=6803287).

To install:

{% highlight bash %}
sudo apt-get install scrot
{% endhighlight %}

To use take a screen shot of the current screen:

{% highlight bash %}
sudo scrot
{% endhighlight %}

The image will be stored in the current working directory as a `.png` file with the name of the current date and time.

To select the screenshot area with the mouse:

{% highlight bash %}
sudo scrot -s
{% endhighlight %}

To add a 5 second delay:

{% highlight bash %}
sudo scrot -d 5
{% endhighlight %}

For a full list of commands:

{% highlight bash %}
sudo scrot -h
{% endhighlight %}
