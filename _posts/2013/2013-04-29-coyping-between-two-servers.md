---
layout: post
title: "Copying between two Servers"
description: ""
category: tech 
tags:
- computing 
---
 
   
Copy  a file or folders between two Servers. Rsync copies folders scp files

{{ more }} 

{% highlight bash html linenos %}
rsync -azvu --rsh='ssh -p32' basedir/ server2:destdir/
{% endhighlight %}
 
{% highlight bash html linenos %}
scp -P32 <file>  server2:destdir/
{% endhighlight %}
