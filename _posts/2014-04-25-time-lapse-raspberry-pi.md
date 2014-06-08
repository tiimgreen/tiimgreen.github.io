---
layout: post
title: "Time Lapse Photography with the Raspberry Pi"
date: 2014-06-05 14:05:00
categories: open-source raspberry-pi
image: /assets/images/raspberry_pi_time_lapse_setup.jpg
---

A recent project I have been working on is Time Lapse Photography with my Pi. I set my Pi to take 1 picture a minute over the course of 24 hours.

To do this I made a custom script in Python, which can be found [here](https://github.com/tiimgreen/pi_lapse).

What you'll need:

- Raspberry Pi (Really?)
- Raspberry Pi Camera Module ([Amazon UK](http://www.amazon.co.uk/Raspberry-Pi-100003-Camera-Module/dp/B00E1GGE40) or [Amazon US](http://www.amazon.com/Raspberry-5MP-Camera-Board-Module/dp/B00E1GGE40/))
- Internet Connectivity (Ethernet or Wireless Adaptor)

Before you start the script you'll want to disable to Pi's LED light to prevent reflection. To do this:

{% highlight bash %}
sudo nano /boot/config.txt
{% endhighlight %}

And paste the following at the bottom of the file:

{% highlight text %}
# Pi Camera LED
disable_camera_led=1
{% endhighlight %}

### Getting the script

To get the pi_lapse script onto your local machine navigate to your desired folder in the command line and type:

{% highlight bash %}
git clone https://github.com/tiimgreen/pi_lapse pi_lapse
{% endhighlight %}

To run:

{% highlight bash %}
cd pi_lapse
python pi_lapse.py
{% endhighlight %}

The setup can be seen below:

![Raspberry Pi Setup](/assets/images/raspberry_pi_time_lapse_setup_uncropped.jpg)
![Raspberry Pi](/assets/images/raspberry_pi_time_lapse_console.jpg)
![Raspberry Pi Taking Image](/assets/images/raspberry_pi_time_lapse_image.jpg)

Whilst Sellotape will do, I would have preferred a more solid stand, something which I hope to make in the future.

The final result can be seen here: [YouTube video](https://www.youtube.com/watch?v=iARVERJb2K0).
