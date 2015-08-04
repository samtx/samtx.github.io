---
layout: post
title: Math Displayed Using MathJax
date: 2015-07-31
---
### Problem
How to find the roots of \\(ax^2 + bx + c = 0 \\)
 
### Answer
The roots are
\\[
x = \frac{-b\pm\sqrt{b^2-4ac}}{2a}
\\]

###Some more math...

\\(y = y_0 + \frac{1}{2}gt^2\\)  
linear acceleration\!

Now let's try some integrals and series summations

\\[
\displaystyle\sum_{i=1}^{10} t_i
\\]
\\[
\int_0^\infty \mathrm{e}^{-x}\,\mathrm{d}x
\\]

Success! This math typesetting is being generated with a call to the [mathjax.org](https://www.mathjax.org/)
site in the `head.html` from the `_includes` folder in the Jekyll file tree.
I'm using the `https` CDN call in the `<script>` tag, like so:

{% highlight r %}
<!--- For MathJax rendering --->
    <script type="text/javascript" 
        src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML">
    </script>
{% endhighlight %}

Within the markdown file, the math is written like this:

~~~
### Problem
How to find the roots of \\(ax^2 + bx + c = 0 \\)
 
### Answer
The roots are
\\[
x = \frac{-b\pm\sqrt{b^2-4ac}}{2a}
\\]

###Some more math...

\\(y = y_0 + \frac{1}{2}gt^2\\)  
linear acceleration\!

Now let's try some integrals and series summations

\\[
\displaystyle\sum_{i=1}^{10} t_i
\\]
\\[
\int_0^\infty \mathrm{e}^{-x}\,\mathrm{d}x
\\]
~~~

Learning how to quickly and effectively write in \\(\LaTeX\\) will be essential in 
graduate school. Writing in \\(\LaTeX\\) feels similar to programming, and the syntax
can be unforgiving. The practice I get by writing down some of my math, physics, and engineering
notes in this blog will hopefully keep me fresh, if it doesn't drive me insane first.

*I just want to make a Jacobian matrix... How hard is that?!*

Full credit goes to the blogs that I referenced to learning how to write this post:
[Gaston Sanchez](http://gastonsanchez.com/blog/opinion/2014/02/16/Mathjax-with-jekyll.html)\\
[kayzhang](http://www.minixli.com/2014/10/20/using-mathjax-with-jekyll/)\\
[Haixing Hu](http://haixing-hu.github.io/programming/2013/09/20/how-to-use-mathjax-in-jekyll-generated-github-pages/)

And I also found this site by [Xu Cheng](https://xuc.me/blog/KaTeX-and-Jekyll/), specifying 
how to use KaTeX instead of MathJax to typeset math on Jekyll. It seems very promising, but I'll leave it as a to-do for now. Today, let's 
keep it simple.