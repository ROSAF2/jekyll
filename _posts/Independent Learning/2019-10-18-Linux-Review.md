---
layout: post
title:  "Linux Review"
permalink: https://rosaf2.github.io/jekyll/Linux/
---
## *Basic Commands*

>---

{% highlight shell %}
pwd
{% endhighlight %}
*displays the current working directory* 

>---

{% highlight shell %}
pwd > File.txt
{% endhighlight %}
*creates a new text file and writes the current working directory address in it* 

>---

{% highlight shell %}
cat
{% endhighlight %}
*displays the contents of a file* 

>---

{% highlight shell %}
ls
{% endhighlight %}
*list the files of the current directory* 

>---

{% highlight shell %}
ls > File.txt
{% endhighlight %}
*creates a new text file and writes the list of files of the current working directory* 

>---

{% highlight shell %}
ls -l
{% endhighlight %}
*gives more detail*

>---

{% highlight shell %}
ls -a
{% endhighlight %}
*shows hidden files also*

>---

{% highlight shell %}
ls -la
{% endhighlight %}
*details files including hidden ones*

>---

{% highlight shell %}
clear
{% endhighlight %}
*clears the screen*

>---

{% highlight shell %}
cd
{% endhighlight %}
*change directory*

>---

{% highlight shell %}
cd ..
{% endhighlight %}
*goes back*

>---

{% highlight shell %}
mkdir
{% endhighlight %}
*creates a new directory*

>---

{% highlight shell %}
rmdir
{% endhighlight %}
*removes empty directory*

>---

{% highlight shell %}
touch
{% endhighlight %}
*creates new file*

>---

{% highlight shell %}
rm
{% endhighlight %}
*removes file*

>---

{% highlight shell %}
rm -d
{% endhighlight %}
*removes empty directory*

>---

{% highlight shell %}
rm -r
{% endhighlight %}
*removes directory with all its contents*

>---

{% highlight shell %}
cp
{% endhighlight %}
*copy files*

>---

{% highlight shell %}
mv
{% endhighlight %}
*moves/renames files*

>---

{% highlight shell %}
grep
{% endhighlight %}
*searchs for words in files*

>---

{% highlight shell %}
grep -i
{% endhighlight %}
*ignores Caps e.g.:*  
*`grep -i FILE.txt` (searchs for all the text files with the word "file" in their names)*
>---

{% highlight shell %}
ls | grep file
{% endhighlight %}
*lists all file names with the word "file"*

>---

{% highlight shell %}
diff
{% endhighlight %}
*displays the difference between files*

>---

{% highlight shell %}
passwd
{% endhighlight %}
*change password*

>---

{% highlight shell %}
echo
{% endhighlight %}
*displays on screen*

>---

{% highlight shell %}
info
man
{% endhighlight %}
*provides information about a command*

>---

{% highlight shell %}
sudo shutdown +1 
{% endhighlight %}
*shuts down the pc in 1 minute*

>---

{% highlight shell %}
sudo apt-get update
{% endhighlight %}
*updates the software list*

>---

{% highlight shell %}
sudo apt-get upgrade
{% endhighlight %}
*updates the software itself*

>---

{% highlight shell %}
sudo apt-get install
{% endhighlight %}
*installs software*

>---

{% highlight shell %}
history
{% endhighlight %}
*shows the previously used commands*

>---

**Variables**  
{% highlight shell %}
NAME=Fran
echo My name is $NAME
{% endhighlight %}

>---

**Permissions**  

| - | d |
|:---:|:---:|
|file|directory|


| rwx | rwx | rwx |
|:---:|:---:|:---:|
|  u  |  g  |  o  |
|users|group|other|

|Permisson|Value|
|:---:|:---:|
| r | 4 |
| w | 2 |
| x | 1 |

>---

{% highlight shell %}
chmod
{% endhighlight %}
*assigns permision to files and directories e.g:*  
*`chmod o+w File.txt`  
`chmod o-w File.txt`  
`chmod 754 File.txt` will give "-rwx r-x r--"*