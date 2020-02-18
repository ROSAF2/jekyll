---
layout: post
title:  "Git Review"
permalink: /Git/
---
## *Git Commands*

>---

{% highlight shell %}
git init
{% endhighlight %}
*initializes folder* 

>---

{% highlight shell %}
git add
{% endhighlight %}
*adds files to the staging area*

>---

{% highlight shell %}
git status
{% endhighlight %}
*displays the status of the files*

>---

{% highlight shell %}
git add .
{% endhighlight %}
*adds everything in the current directory*

>---

{% highlight shell %}
git add -A
{% endhighlight %}
*adds everything in the root directory from anywhere*

>---

{% highlight shell %}
git rm --cached 
{% endhighlight %}
*unstages files*

>---

{% highlight shell %}
git commit -m "message"
{% endhighlight %}
*commits what's in the staging area*

>---

{% highlight shell %}
git commit -am "message"
{% endhighlight %}
*adds and commits*

>---

{% highlight shell %}
git push
{% endhighlight %}
*pushes changes to remote repo*

>---

{% highlight shell %}
git pull
{% endhighlight %}
*pulls what's on the remote server*

>---

{% highlight shell %}
git remote -v
{% endhighlight %}
*displays information about the repository*

>---

{% highlight shell %}
git remote add origin
{% endhighlight %}
*serves up local repo to the web*

>---

{% highlight shell %}
git push origin 
git push -u origin master
{% endhighlight %}
*pushes branch to remote repo*

>---

{% highlight shell %}
git pull origin 
{% endhighlight %}
*pulls branch to local repo*

>---

{% highlight shell %}
git branch
git branch -a
git branch --merged
{% endhighlight %}
*creates new branch or displays existing branches*

>---

{% highlight shell %}
git checkout -b
{% endhighlight %}
*creates branch and moves inside it*

>---

{% highlight shell %}
git checkout
{% endhighlight %}
*Switches between branches*  
*Checks out (inspects) specific commits by using their "hash"*  
*converts a file back to the version previously staged*

>---

{% highlight shell %}
git merge
{% endhighlight %}
*merges a branch with the master branch*

>---

{% highlight shell %}
git branch -d
{% endhighlight %}
*deletes branch*

>---

{% highlight shell %}
git checkout -- file
git restore file
git reset head file
{% endhighlight %}
*this needs revision*

>---

`.gitignore` *a file which contained names are ignored by Git*

>---

{% highlight shell %}
git diff
{% endhighlight %}
*displays the differences between the previous commited version and the latest one*
