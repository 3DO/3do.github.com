---
layout: post
title: "How to Make Latex Math Work in Jekyll"
description: ""
category: ""
tags: [latex, mathjax]
---
{% include JB/setup %}

[MathJax](http://www.mathjax.org) is a tool for embedding latex math formulas into
your own website.

###Installation
Open _include/themes/yourtheme/default.html where “yourtheme” is whichever theme
you’re currently using. Put the following code in.

	<head>
	...
		<script type="text/javascript"
			src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML">
		</script>
	...
	</head>


###Usage & Results
Now you are free to use `\\[...\\]`, `\\(...\\)` and `$$...$$` for your
favorite equations.

Here is an example MathJax inline rendering \\( 1/x^{2} \\), and here is a
block rendering: 
\\[ \frac{1}{n^{2}} \\] 
and,
\\[ x = 1 y = 2\\]
\\[u=v\\]
and,
$$a^2 + b^2 = c^2$$
