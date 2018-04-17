---
layout: post
title: "solved my first dynamic programming problem! plus C and string compression notes"
date:   2018-04-16 17:50:00 -0400
permalink: dynamic-programming-c-string-compression
tags: [recurse center, dynamic programming, data structures and algorithms, c]
---

Week 3 Day 1 @ Recurse Center! Time flies by.

* * *

## Dynamic Programming
* [Best time to buy and sell stock once](https://leetcode.com/problems/best-time-to-buy-and-sell-stock/). Paired with Sean on this. We got a brute force O(n^2) solution that exceeded the time limit. After more than half an hour discussing, trying out solutions, and getting stuck at certain parts, we resorted to Google.
* We found [this similar problem](https://www.geeksforgeeks.org/maximum-difference-between-two-elements/), looked at the code, understood it, then closed the tab and tried to apply it to our problem from memory. It worked, and I presented it at the group discussion later. Super happy because I've never even written dynamic programming pseudocode, let alone written code to solve a dynamic programming problem.
* Because of this, I continue to tell myself that "I am not good at this because I haven't seen it before and/or I don't understand the concept. this does not mean I will never understand the concept or that I will never be good at it."

* * *

## String Compression
* Less than a week before I left for RC, a colleague started a presentation series. Every 2 weeks, he presents on a computer science concept and gives a problem for everyone to solve (should they wish). Even though I'm on a sabbatical now, I still want to follow along with what he is doing. Thus, I am solving the questions.
* This fortnight's question: Implement a method to perform basic string compression using the counts of repeated characters. For example, the string aabcccccaaa would become a2blc5a3. If the "compressed" string would not become smaller than the original string, your method should return the original string. You can assume the string has only uppercase and lowercase letters (a - z)
* Seemed quite simple, but I realised that I need to take into account the two edge case of the last character. What happens when the last character is different from the second-last character, and what happens when the last character is the same as the second-last character?
* Code [here](https://gist.github.com/contrepoint/02fcbf2f967eb6206025223c84d74db8). I am sure it can be improved and refactored. Constructive criticism is super welcome!

* * *

## More C notes
*  `*` is a dereferencing operator
* `&` gets the address of the variable after it
*  ```c
    int x = 1, y = 2, z[10];
    int* ip; /* ip is now a pointer to an int an `int star` */
    ip = &x; /* ip points to the address of x */
    y = *ip; /* dereference ip, so get the thing that is at the address that ip points to. x is 1, so now y is 1 */
    *ip = 0; /* x is now 0 because ip points to the address of x */
    ip = &z[0]; /* ip now points to the address that z[0] is at */
    ```
* A string constant is something like `"I am a string"`
* pointers can point to pointers. so something like `char** p` is a variable p that points to a pointer to a char
