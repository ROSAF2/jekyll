---
layout: post
title: Programming 1
permalink: /P1/
---
{% highlight csharp %}
float number = 5.78F; 
{% endhighlight %}

Format:  
> Scientific Notation:  
**E** (Number of decimal places) **G** (number of digits in total)  

>**C** (currency sign and decimal places)  
**F** (Just number of decimals)  
**N** (adds commas)  
**P** (percentage sign and decimal places "only multiplies it by 100") 

 
{% highlight csharp %}
double number1 = 45.6; 
Int number2; 

number2 = (int) number1; 
{% endhighlight %}

 
{% highlight csharp %}
int comparador = string.Compare(carnet, "si", true); 
{% endhighlight %}

 
{% highlight csharp %}
Random rand = new Random(); 

rand.Next(100) ---> from 0 to 99 

rand.Next(30,40)--->  from 30 to 39  
{% endhighlight %}

{% highlight csharp %}
tempInc = rand.NextDouble();
//randomly picks a real number from 0 to 1  
{% endhighlight %}

{% highlight csharp %}
var e = '€'; 
Console.OutputEncoding = Encoding.UTF8; 
{% endhighlight %}

{% highlight csharp %}
Using System.Threading 

Thread.Sleep(100); 
Console.Clear(); 
{% endhighlight %}

 {% highlight csharp %}
string line="something"; 
string line2=string.Copy(line); 
{% endhighlight %}

 
{% highlight csharp %}
int number = int.MinValue;
{% endhighlight %}
