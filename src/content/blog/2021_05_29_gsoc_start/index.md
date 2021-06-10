---
title: "A Few Preliminary Thoughts"
tags: ["GSoC", "Molecular Dynamics", "Message"]
description: "My first post for GSoC."
author: "Orion Cohen"
date: "2020-05-29"
---

My stated goal this summer is to write a package to make studying ion solvation easier. As I put it in [my GSoC blurb](https://summerofcode.withgoogle.com/projects/#6227159028334592), I am aiming to implement a "robust and cohesive set of methods for solvation analysis." Peripherally, I hope to learn about open-source software, develop as a programmer, save the world, etc. This is an incredible opportunity. It is synergistic with my research, it aligns with my career goals and my ideological positions, and it puts "Google" on my C.V. It's exciting, but also a bit intimidating. By beginning this project I am leaving the comfort of my local repos and venturing into the messy, paradoxical world of practical, collaborative programming.

For the first time in my (brief) programming career, I am designing software primarily for use by others, rather than myself. Instead of writing a program tailored to my particular needs, I must write it for a general audience. The hacky code I write isn't just an inconveniece for my future self, but also  my generous GSoC mentors, not to mention any future users. It's not sufficient to write functions that I can remember how to use, the code should also be simple, communicable, and flexible enough to be learned by others. It's a greater degree of responsibility than I am accustomed to! 

Despite the complexity of these requirements, my aim is simple: I would like to make my MDAnalysis project **good** software. In my mind, this invokes not only software that is useful, but also software that is **clean** and makes **smart abstractions**. However, as I've contemplated this aim, I've noted a tension between my mostly aesthetic notion of cleanliness and the practical business of writing code. Yes, abstraction is central to programming, but is it worth making users learn an abstraction just to execute a simple routine? What will make my program worth using? How do I balance flexibility and ease? I am afraid that my idealistic notions of **good** programming won't survive my encounter with reality. That when the figurative cards are on the table, my code will be riddled with the same inconsistencies and flaws that plague so many scientific codes.

Either way, for the next couple weeks, I'll be writing code, writing tests, and formalizing my program structure. In my next post, I will discuss the abstraction I intend to build around solvation.

