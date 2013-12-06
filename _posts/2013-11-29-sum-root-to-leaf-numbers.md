---
layout: post
title: "Sum Root to Leaf Numbers"
description: ""
category: ""
tags: [leetcode,java]
---
{% include JB/setup %}

This is a one-shot pass problem. The idea is to first retrieve all the paths from
root to leaf(note the definition of leaf), then sum them up for the final
results. So the problem is really about the first part. Well, a path can be
defined as a String and exploration of the path is basically concatenation of
Strings. Now an important question I asked when I tried to proceed was: when
to save the path? My answer was at the end of a path(i.e. when I saw a leaf
node). Great, now the design decisions have been made and the steps are as
follows:

1. DFS the binary tree.
2. Every time I visit a node, I add the value to the end of the
path(String).
3. I remember the path when I reach a leaf node.

Alright, in order to support the above steps, I made several implementation
decisions:

1. I want my recursive helper function to take the path as a parameter,
rather than the return value, since return value is used when bottom-up, but
the parameter can be expanded right on the visit of the node.
2. I also want an ArrayList as another parameter to make sure that leaf
nodes can access the same list at any time.

Enough words and here is the code:
{% gist 7715416 %}
