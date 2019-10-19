---
layout: post
title:  "Windows CLI Review"
permalink: https://rosaf2.github.io/jekyll/CLI/
---
## *Command Line*

>---

{% highlight powershell %}
cd
{% endhighlight %}
*change directory*  

>---

{% highlight powershell %}
cd ..  
{% endhighlight %}
*go back*  

>---

{% highlight powershell %}
cd ../..
{% endhighlight %}  
*go back twice*

>---

{% highlight powershell %}
cd \
{% endhighlight %}  
*go to the root directory*

>---

{% highlight powershell %}
cd /d  
{% endhighlight %}  
*move to whichever drive or folder from anywhere  
e.g: `cd /d C:/`*

>---

{% highlight powershell %}
cls  
{% endhighlight %}  
*clears the screen*

>---

{% highlight powershell %}
color 0F  
{% endhighlight %}  
*changes the CLI colors (hexadecimal)*

>---

{% highlight powershell %}
/?  
{% endhighlight %}  
*help switch*

>---

{% highlight powershell %}
dir ::address  
{% endhighlight %}  
*displays the contents from the address*

>---

{% highlight powershell %}
dir /a  
{% endhighlight %}  
*displays all files and directories including hidden ones*

>---

{% highlight powershell %}
dir /ah  
{% endhighlight %}  
*displays all hidden files*

>---

{% highlight powershell %}
dir /s  
{% endhighlight %}  
*displays files or contents inside subfolders*

>---

{% highlight powershell %}
dir /ad  
{% endhighlight %}  
*displays all the directories only*

>---

{% highlight powershell %}
dir /on  
{% endhighlight %}  
*displays in alphabetical order*

>---

{% highlight powershell %}
dir /b  
{% endhighlight %}  
*displays using only the names*

>---

{% highlight powershell %}
dir /w  
{% endhighlight %}  
*wide format*

>---

{% highlight powershell %}
dir /p  
{% endhighlight %}  
*one page at a time*

>---

{% highlight powershell %}
dir *.png  
{% endhighlight %}  
*wildcard*

>---

{% highlight powershell %}
dir C:\???????.txt  
{% endhighlight %}  
*displays all text files with 7-character names*

>---

{% highlight powershell %}
tree  
{% endhighlight %}  
*displays content branching style*

>---

{% highlight powershell %}
md  
mkdir  
{% endhighlight %}  
*creates a directory*

>---

{% highlight powershell %}
rd  
rmdir  
{% endhighlight %}  
*removes an empty directory*

>---

{% highlight powershell %}
rd /s  
{% endhighlight %}  
*deletes a directory and all its subfolders*

>---

{% highlight powershell %}
type  
{% endhighlight %}  
*displays contents of the file*

>---

{% highlight powershell %}
type nul > File.txt  
{% endhighlight %}  
*creates a file*

>---

{% highlight powershell %}
echo  
{% endhighlight %}  
*displays text to the screen*

>---

{% highlight powershell %}
echo Text > File.txt  
{% endhighlight %}  
*creates a file and writes "Text" in it*

>---

{% highlight powershell %}
attrib  
{% endhighlight %}  
*shows attributes of everyfile in the current directory*

>---

{% highlight powershell %}
attrib +h  
{% endhighlight %}  
*makes a file hidden*

>---

{% highlight powershell %}
ipconfig  
{% endhighlight %}  
*displays network settings*

>---

{% highlight powershell %}
path  
{% endhighlight %}  
*displays the path*

>---

{% highlight powershell %}
prompt  
{% endhighlight %}  
*sets the default cmd prompt*

>---

{% highlight powershell %}
set  
{% endhighlight %}  
*sets variables e.g.  
`set path=%path%;C:\..`  
`set name=something` ( `echo %name%` )    
`set prompt=$t Hello World $g` ("$t" displays the time and "$g" the ">" sign)*

>---

{% highlight powershell %}
cmd  
{% endhighlight %}  
*Starts a new instace of the command line*

>---

{% highlight powershell %}
cmd /t:0F  
{% endhighlight %}  
*changes CLI colors (hexadecimal)*

>---

{% highlight powershell %}
start  
{% endhighlight %}  
*runs applications e.g.  
`start cmd /k "prompt $v & color 0F"`  
("/k" to the immediate commands, "$v" displays the windows version)*

## *Batch Script*

>---

{% highlight powershell %}
REM  
::  
{% endhighlight %} 
*Comments*

>---

{% highlight powershell %}
@echo off
@echo on
{% endhighlight %} 

>---

{% highlight powershell %}
echo %~nx0
{% endhighlight %}   
*displays the name of the file on the console*

>---

{% highlight powershell %}
title  
{% endhighlight %} 
*sets the title of the batch script*

>---

{% highlight powershell %}
echo. 
{% endhighlight %}  
*blank line*

>---

{% highlight powershell %}
pause  
{% endhighlight %} 
*pauses the script*

>---

{% highlight powershell %}
pause > nul 
{% endhighlight %}  
*pauses the batch script and does not display any text*

>---

**loop**
{% highlight powershell %}
:a  
echo hi!  
pause  
goto :a
{% endhighlight %} 

>---

{% highlight powershell %}
net user Bob /add 
{% endhighlight %}  
*adds new user*

>---

{% highlight powershell %}
net user Bob /delete 
{% endhighlight %}  
*delets user*

>---

{% highlight powershell %}
net localgroup "Cool Users" /add  
{% endhighlight %} 
*adds new group*

>---

{% highlight powershell %}
net localgroup "Cool Users" /delete  
{% endhighlight %} 
*deletes local group*

>---

{% highlight powershell %}
net localgroup "Cool Users" Bob /add  
{% endhighlight %} 
*adds user to local group*

>---

{% highlight powershell %}
net localgroup "Cool Users" Bob /delete  
{% endhighlight %} 
*deletes user from local group*

>---

{% highlight powershell %}
chkdsk > C:\\..\\File.txt  
{% endhighlight %} 
*checks the disk for errors and puts the ruslts into a text file*

>---

{% highlight powershell %}
schtasks /create /tn /tr /sc /d /st /rt  
{% endhighlight %} 
*creates new scheduled task with the following parameters:* 

*"/tn" (name for the task)  
"/tr" (program to run)  
"/sc" (frequence)  
"/d" (day)  
"/st" (time)  
"/rt" (privilage)*