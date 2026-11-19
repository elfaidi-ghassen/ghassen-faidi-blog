---
title: Fundamentals Change How You Learn
author: Ghassen Faidi
pubDatetime: 2026-10-18
slug: fundamentals-change-how-you-learn
featured: true
draft: false
tags:
  - computer-science
  - learning
  - fundamentals
description: Why having a solid foundation in computer science changes how you learn, think, and approach new problems.
---

We often hear the generic advice to “focus on the fundamentals.” For some reason, I believed that advice even before I understood why it matters. It just sounds like common sense, and fortunately, it turned out to be good advice. I realized this after taking multiple free OSSU courses and reading a couple of books (OSTEP, Computer Networking: A Top Down Approach, Dan Grossman’s PL course, …). I also realized this more deeply when I started learning web development, and even more during my first internship.

Here’s the key idea: **two different people can study the same material from the same teacher or book and walk away with completely different experiences because of the knowledge they already have.**

![Palm Trees - Jan Ciągliński (1909)](https://substackcdn.com/image/fetch/$s_!tNow!,w_1456,c_limit,f_auto,q_auto,good,fl_progressive:steep/https%3A%2F%2Fsubstack-post-media.s3.amazonaws.com%2Fpublic%2Fimages%2F38416049-5029-4835-b8df-79361ed3b229_1800x1184.jpeg)

*Palm Trees - Jan Ciągliński (1909)*

“Previous knowledge” makes learning new things much more fun because you’re not starting from scratch every time! When we haven’t internalized the key fundamental “chunks of knowledge,” every new problem we face feels completely new, so it feels much more painful. But what’s worse is that we learn less from the experience. Without a well-organized base of knowledge, new information has no meaningful place to attach to, so much of it is quickly forgotten.

There are three things that good fundamentals help you with:

1. They allow you to extract SO MUCH from ANYTHING you learn.
2. They guide you to ask the right questions and learn faster. Learning compounds really fast at some point.
3. Odd things feel odd to you.

For example, after studying OS and networks, I internalized the idea of a server. It actually took me quite a while to fully get it. Here’s a casual explanation:

A server is a process that has an open socket (on a specific port). But to grasp this, I had to understand what a process is. Luckily, I learned about it from an OS book (OSTEP). A process is an “abstraction” of a running program. When you run a program, the OS wants to keep track of what’s going on, so each running program is represented in the OS as a process with an ID and a status. It’s pretty much like an object with some fields. They’re basically stored in a table. Each time you run a program, a process starts running, i.e., it’s added to the table. When you kill a process, it stops and is removed from the table, etc.

(The concept of abstraction itself is part of CS fundamentals, and it took me some time to internalize it and start seeing it everywhere. It’s amazing how a single word can capture so much meaning.)

But then, what’s a socket? It’s an abstraction of the networking stuff. It’s an API (a bunch of functions provided by the OS) that you can call as a developer so your process (running program) can communicate over the network. You don’t need to know much about networks or TCP to use it, just the API’s inputs and outputs. So basically, a server must have some sort of socket that clients can connect to and send bytes to. The server understands those bytes, usually through a string-based “protocol,” and then responds accordingly.

This is just some CS fundamentals, nothing fancy. But now that I’ve spent around a year studying web development, I can see how all of this was there all along (but in different shapes and flavors). Everything is built on top of fundamental concepts, and it’s so much fun.

1. This allowed me to learn way more from the resources I was using. I kept digging: “Wait, where is the process?” “How does this work?” “What happens when I use `docker run`?” I used SSH for the first time and thought, “But wait, how is this happening? There must be an SSH process running on the server or something.” Or, “Hey, where is the database process?” And you just keep digging.
2. It’s related to the previous point, but having good fundamentals helps you ask better questions, which in turn help you fix problems faster and deepen your understanding.
3. Sometimes you encounter something new that makes you question what you’ve learned before. It challenges the mental model you’ve built. You feel surprised, and your understanding broadens. It’s hard to notice these things without having the fundamentals.

And this doesn’t mean we need “perfect” fundamentals. I’m aware of some of the gaps I have, and I plan to work on them, but we just need to internalize the key concepts. If you haven’t mastered the fundamentals yet, I highly recommend the following:

- **Build a simple shell.** It’s really simple; a shell is just a program you run, and a Python script would do (or C if you like more challenge). Understand how the shell runs other programs and what `PATH` is, the system calls, etc. I highly recommend Python so you can focus on the OS concepts. Though I’m sure some would disagree on that point.
- **Build a simple HTTP server.** Jim Kurose has [recorded lectures](https://gaia.cs.umass.edu/kurose_ross/lectures.php) explaining the fundamentals of computer networks. The first two chapters are more than enough for most people. After that, you can easily build a simple HTTP server. If you want to spice it up, add some multithreading. He has the [starter code](https://gaia.cs.umass.edu/kurose_ross/programming.php) available too.

These two projects have had the highest ROI of anything I’ve done while learning. They even made me fall in love with CS.