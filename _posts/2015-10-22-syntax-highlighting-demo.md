---
layout: single 
header: 
  overlay_image: splash2.jpg
  caption: "Photo credit: [**Unsplash**](https://unsplash.com)" 
title: "Syntax Highlighing Demo"
category: programming
tags: [static-site-generators,github, github-pages, jekyll, pygments, milwaukee-code-camp-2015]
author_profile: true
read_time: true
comments: true
share: true
related: true
---

This post is a demonstration of syntax highlighting in Jekyll using Pygments, for my presentation  on Static Website Generators at [Milwaukee Code Camp](http://www.milwaukeecodecamp.com)
October 24, 2015 [](http://www.milwaukeecodecamp.com)

[Pygments supports many languages a list of the can be found here.](http://haisum.github.io/2014/11/07/jekyll-pygments-supported-highlighters)

Here is a bunch of [Pygment themes for Jekyll.](http://jwarby.github.io/jekyll-pygments-themes/languages/javascript.html)

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

C#
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

Javascript
{% highlight js linenos %}
function loadScript(script, element) {
        var scr = document.createElement("script");
        scr.async = true;
        scr.src = script;
        (element || document.body).appendChild(scr);
}
{% endhighlight %}

F#
{% highlight fsharp linenos %}
open System

[<EntryPoint>]
let main argv = 
    printfn "Hello World" 
    Console.ReadLine() |> ignore
    0 
{% endhighlight %}

