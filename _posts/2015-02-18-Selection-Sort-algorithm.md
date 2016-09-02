---
layout: post
title: "Selection Sort algorithm"
description: 
headline: 
modified: 2015-02-18
category: webdevelopment
tags: [jekyll]
imagefeature: algorithm.jpg 
mathjax: 
chart: 
comments: true
featured: true
---


In this sorting algorithm  we get the minimum value of an array and swamp it with the 0 position of the array. Then we search for the minimum value without considering the value of the 0th position.
After that we will swamp it with the value in the 1st position. We do this until we get the array sorted.

Run time of this algorithm is O(n2). This does not change with the order of the elements in the array because still has to go through all element to get the minimum value.

![sorting]({{ site.url }}//images/post2/Selection-Sort-Animation.gif)

References
Image source [1] - https://en.wikipedia.org/wiki/Selection_sort