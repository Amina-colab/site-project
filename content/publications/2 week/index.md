---
title: "My Second Week in the World of IT"
date: 2026-04-04
draft: false
authors:
  - admin
tags:
  - personal
  - study
  - RUDN
categories:
  - Blog
summary: "How my second week of studying Computer Science at RUDN went"

featured: true
---

## Week Summary

This week I:

+ Finally got to properly learn classes in C++. Before, they seemed like something magical, but now I see them as a convenient way to bundle data and functions together. I figured out the difference between struct and class (everything is private by default — I remembered that after a couple of errors in my code).

+ Another discovery — static member variables. Turns out they are shared across all objects of a class, rather than being copied for each one. I wrote a small object counter, and it worked exactly as I expected — it gave me that satisfying "aha, it works!" feeling.

+ A special challenge — pointers and references. I kept confusing * and & for a long time, but this week things started to click: a pointer is a variable that stores an address, and a reference is an alias (and you can't reassign it). I wrote small value-swapping functions — first with pointers, then with references. The result is the same, but references are easier to read.

## Impressions

Honestly? It was both difficult and very interesting. When I first wrote a Student class with fields and a printInfo() method, then created several objects — I felt like a real developer. Static variables surprised me at first: "How can one variable be shared across all objects?" — but when I added a static counter and saw it increase with each new object, understanding dawned.

Pointers and references caused the most errors. Several times I caught myself trying to dereference nullptr (thankfully the program just crashed instead of corrupting data). But once I figured out passing by reference in functions, it became much clearer how cin >> x works and why x changes.

What I especially appreciate is that during lab sessions at RUDN, the professors explain not only the "how" but also the "why." Now I understand why references are needed in input/output operators and why it's better to use a reference in a copy constructor.

## Plans for Next Week

- Understand constructors and destructors — so far only at the "they are called automatically" level. I want to write my own class with a non-trivial destructor.

- Practice passing pointers to functions (especially with dynamic memory, new and delete).

- Solve several problems with arrays of pointers and possibly start studying dynamic arrays of objects.

- Solidify static methods (so far I've only mastered static variables).

And most importantly — don't be afraid of compilation errors, but read them as hints.

See you next week!