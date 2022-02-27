---
layout : post
title : "Create your own Jekyll Website!"
date : 2022-02-22 12:25:00 -0500
categories : Installations
tags : [Installations, Linux]
---

Environment : Ubuntu 20.04

You finally decided to create your own blog! Hopefully you're not Creed, but oh well lets get to it!

Install Jekyll dependencies:

{% highlight console %}
sudo apt install ruby-full build-essential zlib1g-dev
echo 'export GEM_HOME="$HOME/.gems"' >> ~/.bashrc
echo 'export PATH="$HOME/.gems/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc

{% endhighlight %}

Install Jekyll itself and other dependencies:

{% highlight console %}
gem install --user-install jekyll bundler webrick
{% endhighlight %}

Note that the `--user-install` line is pretty useful since you don't want to install this via root.

Finally head to the location where you want to create your project and enter:

{% highlight console %}
jekyll new name_of_your_awesome_blog
{% endhighlight %}

And thats it!
