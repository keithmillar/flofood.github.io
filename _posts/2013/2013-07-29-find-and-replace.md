---
layout: post
title: "Find and Replace"
description: ""
category: tech
tags:
- linux
---

{% highlight bash %}
find . -name '*.html' | xargs perl -pi -e 's/oldtext/newtext/g'
{% endhighlight %}

\n adds a new line

 finds  any text and replaces it with <!--start excerpt-->

{% highlight bash %}
find . -name '*.md' | xargs perl -pi -e 's/any text/<!--start excerpt--> /g'
{% endhighlight %}
finds any text and replaces it with a new line and <!--more tag--> (\n being new line)

{% highlight bash %}
find . -name '*.md' | xargs perl -pi -e 's/any text/\n<!--more tag-->/g'
{% endhighlight %}
