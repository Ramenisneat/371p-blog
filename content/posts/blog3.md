---
title: "CS 371p Fall 2026: Rahul Myana : Blog 3"
date: 2026-02-01T21:17:32-06:00
draft: false
toc: false
images:
tags: 
  - untagged
---
<img src="../../headshot.jpg" width="200"/>


## Blog Entry no°3

**What's up 👋**

I hope your week has gone well. Can't believe we had a winter storm less than a week ago with all this sunlight shining straight into my eyeballs constantly. Honestly, though I am very much enjoying the cooler weather for once.

About this week in this class, the project surprised me. I feel like with a lot of other classes at UT, projects usually comprised of just completing some test cases and your good. However, there were a lot of moving parts with this project with not just the HackerRank test cases, but the unit tests, UAT, gitlab CI pipeline etc. I feel like I am the sort of person that just complete my work in one shot untill it works. So, having to continously check myself to commit and close issues and etc. took me a second.

The assigned paper about Continous Integration was an interesting read. I agree with all of the points the author made about the effectiveness for CI, but the workflow feels a little too idealistic for me. Like, I understand when all the devs are working properly, making meaningful changes to the code and being communicative, CI with changes everyday works well. But I feel like the real world is never like that. I feel like many features take much longer than single commits to get right, most of the time it can take multiple days and commits, but with devs constantly breaking away from devleopment to integrate their sloppy code with other sloppy code can lead to issues. Yes, in a perfect world this is a non issue, but that's the thing, it's not a perfect world. I feel like some devs like the idea of eliminating every ounce of unproductivity from their work, but I think chasing that rabbit hole leads to more problems than solutions. I think having the expectation for fast commits and passed test cases can lead to more hiccups in some cases. I guess what I am trying to say is that there is always going to be some "slop" and that we should embrace this "slop". Instead of pushing out commits hourly with whatever small change we have made, a more substantial change that can be done in a workday or a couple of workdays, with the afforded time we can verify is proper and then push onto our main. I think I like a more middleground approach to CI/CD than what I see in this paper. 

Sorry if that was a bit rambly.

Oh and for my pick-of-the-week this week, is `webhook.site`. I work with a bunch of microcontrollers in my free time and like doing IOT projects, which require you to build APIs and such to get working. With micrcontrollers, sometimes that's the only way to send viable way to diagnose if it's functioning properly since you have such a limited Serial interface to work with. For example if you are doing some sort of image manipulation on a controller, the simplest way to see the results of that is to spin a webserver and have the controller post the data to that API. But working with UT's network can be a pain in regards with local communication, so if I quickly need to verify functionality on a project before creating a central backend to handle requests, I like using this site to handle incoming requests and see if data is being transmitted properly. ig, there is a concern with whether information sent to the site is stored or not, but I genuinely just do dumb stuff with it, so I don't care. 

