---
layout: post
title:  "RC goals, pairing on C, meals"
date:   2018-04-09 23:50:00 -0400
permalink: goals-notes-pairing-on-c
tags: [recurse center, c, data structures and algorithms]
---

When one is in an environment as self-driven and as unstructured as RC, goal-setting and progress-tracking, are really important. Thus, I've decided to do twice-a-day checkins - one at the start of the day to say 'this is what I plan to do today', and one at the end of the day to say 'this is what I did today, this is what I plan to do tomorrow'.

## Goals - 09 Apr 2018
### Technical
1. Code more C (achieved!)
2. Write a blogpost (achieved!)
3. Start doing a DS&A problems on the whiteboard (achieved!)

### Non-Technical
1. go for Halo Circus' concert at 8.45pm (cancelled due to the singer being unwell)
2. lunch w/ fellow M'sian RCer (who is an alum). (achieved!)

Details on what I achieved (or did not achieve) beneath the cut. Plus some bonus unexpected things!

* * *
<!--more-->

## Technical
### C
some notes from today's Kernighan & Ritchie C study:
* text stream - sequence of characters divided into lines.
* `getchar()` reads the next input character from a text stream and returns that as its value. `c = getchar()` means that the variable c contains the next character from the text stream
* putchar(c). prints the character in `c` each time it's called
* `EOF` is an integer defined in `<stdio.h>`. specific numeric value does not matter as long as it's not the same as any char value.

Got stuck figuring out how to test exercise 1.8, and Zuliped a call for pairing help. Ethan responded. Turns out, he worked through the K&R book... 12 weeks ago, and is very happy to refresh his knowledge. He's also working on learning data structures and algorithms. C is so full of small subtle things that you could accidentally introduce subtle bugs that you don't mean to.

For example, `while(*str++) { // stuff }` means that the code will test for `*str` first, increment `*str` and _then_ only do 'stuff'. I'll write a more detailed explanation about this (and how we realised that logic and tested for it with `printfs()`) sometime. I now have two versions of that exercise - the correct one that I'll commit and push to github, and the buggy one that I now know 'why this is buggy.'

### Leetcode (data structures and algorithms)
* Did the [valid parenthesis](https://leetcode.com/problems/valid-parentheses/description/) problem in Ruby. It passed, and I'm in the top 95% of Ruby solutions. However, I'm still not sure whether I should do these sorts of problems in Python or in Ruby - it frustrates me that some of Ruby's standard library is not very intuitive.
* A bunch of us discussed this and another problem. It's so _nice_ to be able to talk about data structures and algorithms (which I only know from what I have managed to self-laern) with multiple people. We ask questions to, explain to, and learn from each other. I'm so happy.

* * *
## Non-Technical
### Non-Technical Talks! (because we're more than programmers)
* I _love_ how RCers are interested in so many different fields outside programming. Among the talks included going to conferences (both technical and non-technical), learning languages effectively (I was super happy that I have read the book Alan presented on!), spaced repetition, escape rooms, and pro wrestling.

### Halo Circus
* Cancelled, sadly, because Allison is not well. Am sad because I've followed her career since her American Idol 8 days.

### Malaysian Lunch
* Learnt the hard way that missing one stop on an express train can mean overshooting your destination by 30 streets.
* It was nice to hear another Malaysian RCer's story, and to learn and take inspiration from it. Thank you.

* * *
## Bonus
* Talked to Alicia, one of the facilitators.
* Steven brought me PAX East swag, and it was all free.
* Coffee chat with Arun that ended up being a dinner chat. Two other RCers ended up at the same Thai place and we all walked back together laughing about tabs vs spaces and syntax highlighting, among other things.
* All the small (but lovely) conversations I had with various RCers throughout the day.

Finally - thank you, Marianne and Ashley, for your encouragement and for sitting near me as we all type our blog posts up. Being with you helps me feel less... intimidated by the thought of blogging, and reminds me that yes, I do have something to say. Even if it only helps a past version of myself, or a future version of myself (who wonders, 'hey, what did I do at RC again?'), it will be enough.

Till tomorrow.
