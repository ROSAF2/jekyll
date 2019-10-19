---
layout: post
title:  "Jekyll Review"
permalink: http://localhost:4000/Jekyll/
---

>---

## *Basic commands*

{% highlight shell %}
jekyll new blog
{% endhighlight %}
*creates website*

>---

{% highlight shell %}
bunfle exec jekyll serve
{% endhighlight %}
*serves up the website to view on browser*

>---

## *Front Matter*

> This is the information about the post/page such as title, layout, date, author, etc. for example:  
{% highlight yaml %}
---
layout: post  
title:  "Welcome to Jekyll!"  
date:   2019-10-16 19:55:43 +1300  
categories: jekyll update  
---
{% endhighlight %}

>---

## *File Naming Convention Structure*

> 2019-08-01-welcome-to-jekyll.md  
  year-month-day-title.md

>---

## *Variables*
{% highlight yaml %}
categories: one two
{% endhighlight %}
*use the colon "**:categories**" in order to cast the variable*
{% highlight yaml %}
layout: post
{% endhighlight %}
*is the skeleton of the post*

>---

## *Permalinks*
{% highlight yaml %}
permalink: /my-new-url/
permalink: /:day/:month/:year/:title
{% endhighlight %}

>---

## *Uploading a Jekyll site to GitHub*

* Create Jekyll local site and a new GitHub repo

* Initiate Git repository and modify "config.yml" file (baseurl: "name of GitHub repo")

{% highlight shell %}
git checkout -b gh-pages
{% endhighlight %} 

{% highlight shell %}
git add . / git commit -m "initial commit"
{% endhighlight %}

{% highlight shell %}
git remote add origin "url from GitHub"
{% endhighlight %}

{% highlight shell %}
git push origin gh-pages
{% endhighlight %}

>---

## *Drafts (optional)*
> To make a drat:

1. Make a folder called "_drafts" inside the root folder
1. Create a draft e.g. "My-First-Draft.md"
1. Then, run the next command:
{% highlight shell %}
jekyll serve --draft
{% endhighlight %}  

* *when naming drafts, the date is not required*
* *when the draft is ready, the draft can be used by putting it inside the post folder using an appropiate date*
