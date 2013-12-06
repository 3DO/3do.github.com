---
layout: post
title: "Sort Colors"
description: ""
category: ""
tags: [leetcode, java]
---
{% include JB/setup %}

The two-pass algorithm is trival and skipped here. The idea of one-pass
algorithm is simple: we keep track of three pointers, one for the position
after the head zeros, one for the position before the tail twos and the last
pointer for the current position. Everytime if we see a zero, we swap the zero
ahead, and similarly when we see a two, we swap down to the end. However the
implementation is tricky and one needs to be really careful.

{% gist 7713656 %}
