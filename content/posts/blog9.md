---
title: "CS 371p Fall 2026: Rahul Myana : Blog 9"
date: 2026-03-15T16:56:07-05:00
draft: false
toc: false
images:
tags: 
  - untagged
---
<img src="../../headshot.jpg" width="200"/>

## Blog Entry no°9

**What's up 👋**

I was lazy and I didn't show up to classes this week, so I don't have many thoughts on the contents that were discussed during the lectures. Looking at the notes, allocator_traits seems like a cool way to access allocator functions to add allocator functionality to your container. Still need to look into it.

The project this week meant a lot to me. It may sound weird. But I have a reason. Back in CS429 (~3.5 years ago, damn), when we had a very similar malloc project. It was taught to us that a free list needed to be used and that a linked list was commonly used. But the project description was like "This may not be the only solution, you could try other creative solutions" or something along that lines. So, me as a budding CS freshman, was like "wow, I have an idea of using tags to mark blocks as free or used". Very similar to sentinels hmmm. And it worked, kinda? It was working flawlessly and iirc the tests showed performance metrics which I bragged to my friend about. But it still didn't work fully? "odd" I thought, I literally don't see any reason why. It seemed like blocks tended to have breaks in the memory addresses, but I didn't do that. It turns out, that the implementation of sbrk that the project gave to me, PURPOSELY SOMETIMES BREAKS UP THE ADDRESSES. NORMAL SBRK DOES NOT DO THIS. BUT THIS IMPLEMENTATION DOES. MAKING MY SOLUTION NULL AND VOID. MAYBE I COULD KEEP TRACK OF OFFSETS OR SOMETHING BUT MY RAGE KNEW NO BOUNDS. I COULD NOT THINK CLEARLY AND WITH THE SUBMISSION BEING THAT NIGHT, i just gave in a previous linked list solution. I never experienced greater shame. I'm sorry if I sound crazy, but I genuinely think back to this almost weekly. So this project, with the usage of sentinels, healed me (somewhat).

Also AI is useless, like genuinely for debugging anything with more than 2 levels of logic. I felt like the allocate and deallocate methods very easy to write up (given my past encounter with sentinels...), but when it came to debugging a very strange bug that I encountered, it could not do it. It hallucinated, gave me garbage fixes and more junk. It's because LLMs being a textual model, cannot really represent that state of an allocator properly. So when it can't find a solution in this weird latent space incorrect world view it has constructed, it just imploded. Continuing to try to use AI was just gonna waste even more time, so I just ignored it and went back to the good ole days of printf debugging. felt like a farmer returning from the bourgeois vibe coding hell. 

My pick-of-the-week for this week is [uxn](https://100r.co/site/uxn.html) is this weird/fun toy virtual machine implementation that has this old retro rom game sharing kind of attitude to it. The language used to create this roms are is a very simple stack-based concatative language, which is fun to make sense of. 

<img src="https://100r.co/media/content/projects/uxnexplode.jpg" width="400"/>

