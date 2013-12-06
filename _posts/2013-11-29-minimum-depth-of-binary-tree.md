---
layout: post
title: "Minimum Depth of Binary Tree"
description: ""
category: ""
tags: [leetcode,java]
---
{% include JB/setup %}

This problem is an interesting comparison to *Maximum Depth of Binary Tree*,
which is essentially getting the height of a tree. When getting the maximum of
left and right subtrees[show me the code], if one subtree does not exist we
treat the height to be 0. However, this is not true in the *Minimum Depth*
problem. When the subtree does not exist, we should move that out of
consideration, in other words, use `Integer.MAX_VALUE` as its height. This
little trick solves the problem.

{% gist 7715169 %}
