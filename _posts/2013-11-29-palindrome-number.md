---
layout: post
title: "Palindrome Number"
description: ""
category: ""
tags: [leetcode,java]
---
{% include JB/setup %}

I did not pass the problem at the first run, due to the time exceeding error.
The improved approach is simple: peel the head and tail at each round and
compare if they agree. Note the */100* part.

{% gist 7714940 %}
