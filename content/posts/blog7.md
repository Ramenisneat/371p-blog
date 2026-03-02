---
title: "CS 371p Fall 2026: Rahul Myana : Blog 7"
date: 2026-03-01T19:23:44-06:00
draft: false
toc: false
images:
tags: 
  - untagged
---

<img src="../../headshot.jpg" width="200"/>

## Blog Entry no°7

**What's up 👋**

This weeks paper was interesting to read about. The main definition of LSP is `If S is of subtype T, then objects of type T should be replaceable with objects of type S without breaking the program`. This feels obvious to me, like "duh, that's definition of a ISA relationship", but the counter examples really highlighted the complexity within that definition. Inheritance is more about behavior complexity rather than code reuse than I previosuly thought. From reading the paper I gathered that a subclass must not:
- Strenghten preconditions
- Weaken postconditions
- Change the meaning of class methods

I think you could further simplify this by asking "if swapping this subclass everywhere where the parent class is will break the program"

Regarding this weeks problem, I started to notice a trend in my solutions. Most programming questions can be solved with a Hash map/set. I used a map to simplify the problem in this one and I have also completed next week's problem with just using a set. I took the Information Retrieval class with Professor Mooney last semester and he would always say: "What's my favorite data structure? Hashmaps!". I am starting to feel his enthusiasm for them as well. 

I think something from this week's lectures that was interesting was the introduction of the `friend` keyword. How it can establish a direct connection from one class to another, to access it's private variables. It's the first time I have seen this type of behavior and it's very strange to just allow an entire other class access ALL of the prviate variables of your class. I feel like this is a hamfisted way to allow this functionality by breaking encapsulation. I wonder if there are any CVEs that describe an attack vector using the friend keyword.  

My pick-of-the-week for this week is maybe using a vps. A vps is a virtual private server. It acts like a dedicated server with dedicated resources but internally its all virtualization. I picked this because I hate how cumbersome it is to communicate between devices on the UT network if you are not able to define a static IP. I've created a simple DHCP router with an ESP32 to act like a local network but someone took it from me 💀. So, I think just having a vps act like proxy might be the move.