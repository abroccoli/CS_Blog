---
layout: post
title: "Queues and Stacks and Sets"
date: 2015-03-30 16:58:35 -0400
comments: true
categories:
---

<p>Hello! Today marks my first baby-step back into the world of Computer Science since graduating from Syracuse last spring. I took a look at Queues, Stacks, Sets, Associative Arrays, and Arrays in an attempt to get a better grasp on the minutiae of data and be able to apply my knowledge to writing quicker and more elegant code.</p>

<h2>Arrays and Associative Arrays</h2>

<h4>Arrays</h4>

<p>In order to get a grasp on the rest of the data types I planned on exploring I first found it necessary to re-evaluate my understanding of Arrays. Sure, I have iterated over a countless number of arrays over the course of my time sitting in front of a computer but did I really understand exactly what constituted an array?</p>
<p>On it's most fundamental level, an Array is just a chunk of memory. A basic array implies that this chunk is a static size and does not change over the course of the codes execution. A dynamic array is an array that can change in length, this is the type of array that I am accustom to using in Ruby and JavaScript. I found myself wondering why someone want to use a static array when dynamic arrays are available? The answer it turns out is because of how dynamic arrays adjust themselves in size. When a dynamic array needs to grow the array doubles itself in size, creating room for twice as many elements as were previously in the array. Using a lot of dynamic arrays can take up quite a bit of memory, thus when it the exact number of values in an array is know it is best practice to use a static array.</p><p>So why even use arrays? Well as anyone who has written code has undoubtedly come across scenarios where multiple similar data values required processing. If there were n values that needed to be run through the same function, without an array we would be required to define each value separately and then write out the code to apply that function n times. With an array it's as simple as defining the array and then passing that array into the function once and allowing it to iterate over each element and apply the same logic to each element of the array.</p>

<h4>Associative Arrays</h4>

<p>An Associative Array is also called a Hash Table and is closely related to the hash object that I have used so many times in Ruby. An Associate Array applies a key to each value of the array, and when a hashing function is applied to that key it is immediately linked to the corresponding value of the array. This allows for incredibly quick lookup, insertion, and deletion of elements into an associative array.</p>

<h2>Sets</h2>

<p>Using a set is a great way to increase processing speed and eliminate issues that arise with nested loops. A set can be thought of as a Hash with no values, a set of keys that can be directly accessed. While adding values to a set is not ideal and can cause issues, getting values from a set is very fast. In the past I have used nested loops to iterate through arrays and then iterate again over each element of that array. This causes an exponential processing time and can create big issues the longer the arrays get. By turning one array into a set prior to iterating through them you can eliminate the risks of exponential computations and instead end up with a standard linear process.</p>

<h2>Stacks and Queues</h2>

<h4>Stacks</h4>

<p>Stacks are groups of data that are Last in First Out (LIFO). This means that the last item appended onto a stack is the first item that must be accessed in order to keep moving through the stack. Stacks can be thought of like a stack of cards, in order to get to the bottom card you must take off the ones that you placed on top of it first.</p>

<h4>Queues</h4>
<p>Queues are relatives of stacks that are First in First Out (FIFO) data types. Queues can easily be pictured by thinking of lines that we all wait in on a daily basis. The first data placed in a queue is the first data that can be accessed from a queue. This data structure is very useful when code needs to be executed orderly.</p>
