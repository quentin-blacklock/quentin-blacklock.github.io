---
layout: post  
title: "Syntax Highlighing Demo"
category: programming
tags: [github, github-pages, jekyll]
---
This post is a demonstration of syntax highlighting in Jekyll using Pygments, for my presentation at Milwaukee Code Camp
October 24, 2015 [](http://www.milwaukeecodecamp.com)


HTML
{% highlight html linenos %}
<div id="topbar" class="pure-menu pure-menu-open pure-menu-horizontal">
        <ul>
          <li><a href="/">Home</a></li>
          <li><a href="/downloads">Downloads</a></li>
          <li><a href="/archive">Archive</a></li>
          <li><a href="/about">About</a></li>
        </ul>
      </div>
      <div class="left">
        {{ content }}
      </div>
</div>
{% endhighlight %}

c#
{% highlight csharp linenos %}
// A Hello World! program in C#.
using System;
namespace HelloWorld
{
    class Hello 
    {
        static void Main() 
        {
            Console.WriteLine("Hello World!");

            // Keep the console window open in debug mode.
            Console.WriteLine("Press any key to exit.");
            Console.ReadKey();
        }
    }
}
{% endhighlight %}

{% highlight js linenos %}
function loadScript(script, element) {
        var scr = document.createElement("script");
        scr.async = true;
        scr.src = script;
        (element || document.body).appendChild(scr);
      }
{% endhighlight %}