---
layout: post  
title: "YAML is Fussy About Formating"
category: programming
tags: [static-site-generators, github, github-pages, jekyll, yaml]
---

YAML, a markup language, is used in GitHubPages, Jekyll and many other static website generators for configuation information, front matter in posts, and defining data. 

YAML is fussy about formating and can be the cause of build errors in GitHub Page sites and Jekyll sites.

Bad YAML Example
{% highlight yaml linenos %}
--- # Tags for posts
- slug: github
   name: GitHub

 - slug: github-pages
    name: GitHub Pages

 - slug: jekyll
   name: Jekyll
  
 - slug: that-conference-2015
   name: That Conference 2015
   
 - slug: yaml
   name: YAML
{% endhighlight %}

The miss-alignment of the indents in the first two tags can be the cause Page Build Failure emails from GitHubPages, or
this error when perfoming a jeykyll build command:

>jekyll 2.5.3 | Error:  (/_data/tags.yml): 
>mapping values are not allowed in this context at line 3 column 8

Fortunalty there are a couple of YAML "Linting" tools online to help.

[YAML Lint](http://www.yamllint.com/)

[YAML Validator](http://codebeautify.org/yaml-validator)

Corrected YAML Example
{% highlight yaml linenos %}
--- # Tags for posts
- slug: github
  name: GitHub

- slug: github-pages
  name: GitHub Pages

- slug: jekyll
  name: Jekyll
  
- slug: that-conference-2015
  name: That Conference 2015

- slug: yaml
  name: YAML   
{% endhighlight %}

YAML is fussy about formating and can be the cause of build errors. Hard lesson learned. Hopefully this helps.