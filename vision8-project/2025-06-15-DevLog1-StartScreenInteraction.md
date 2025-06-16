---
layout: post
title: "Vision8 Devlog #1 – Start Screen and Testing Interaction"
date: 2025-06-15
author: Nana Lee
---
This weekend, I built the first working interaction in Vision8: a start screen and a basic vision test flow.

The test is simple — you press "Start Test" and see an arrow on the screen.  


### What I built today

- A **Start Screen** with a single button to launch the test.
- A **Test Screen** that:
  - Shows an arrow in one of four directions.
  - Asks the user whether they saw the arrow.
  - Changes the arrow size depending on the response:
    - *Seen?* → smaller (harder)
    - *Not seen?* → bigger (easier)

This structure mimics how eye doctors test vision, but without needing an actual doctor present.

### Why this matters

Many apps assume users can read text.  
But for someone who’s already struggling with blurry vision, asking them to *read* is asking them to fail.
In the future, the buttons will be replaced by signs such as X and Os.


## 🌀 Naming and Logo Design

So I decided to name this software **Vision8** a long time ago.  
Since this is going to be presented on the App Store, I needed a logo.  
I tried to blend the ideas of **vision**, **eight (8)** (which sounds like *aid*), and medical accessibility.  
I scattered these three ideas, and decided to stick with this one:

![Vision8 Logo](/image/visioninfinity.png)
