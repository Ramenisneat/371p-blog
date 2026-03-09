---
title: "CS 371p Fall 2026: Rahul Myana : Blog 8"
date: 2026-03-08T20:31:15-05:00
draft: false
toc: false
images:
tags: 
  - untagged
---

## Blog Entry no°8

**What's up 👋**

This week's problem was interesting because it made me realize that the standard library won't always be the solution. For the problem, my solution required a way to store a pair in a set. I reasearched online and I realized that there isn't any standard way to hash a pair, so I had to define that hash function myself. The solution worked, but when I put it through the test cases, I got an out-of-time error. I realized that although my solution worked with the std library and was elegant, the overhead that it costed was too much for large test cases. I simplified my solution by shifting the pair into one 64 bit `long long` and that sped things up tremendously. It made me realize that sometimes solutions don't involve you importing some library and it means you should get your hands dirty.

The paper from this week was a little confusing at first, because I kept asking myself why can't we implement 2 different interfaces, it feels a little too obtuse to implement an adapter class to solve the problem. It feels obviously clear to me to have a singular class inherit from multiple abstract classes and it keeps ISP secure. Then the paper briefly clarified that multiple inheritance is also a solution. Maybe it's because the paper is somewhat old, the concepts were a little alien to me. 

C struct vs classes was a little convoluted. I don't like how the semantics of a struct/class can change so easily especially for member initialization. I understand that there is a convention, but I feel like with the nature of structs and classes, it's very easy for that to be forgotten. I feel like cpp's insistance to be backwards compatible with C can be a crutch

My pick-of-the-week for this week is just a party trick I learnt about C and cpp.<br>
Yk how array indexing is just pointer arithmetic<br>
So in pointer arithmetic terms: `arr[idx] is just *(arr + idx)`<br>
But addition is commutative so you `can write it as *(idx + arr)` <br>
Which means you can index by doing `idx[arr]` which compiles <br>
So like `2[arr]` works and compiles, although is obviously impractical. neat.


