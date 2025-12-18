---
layout: project
type: project
image: img/rainbowRecipeLogo.png
title: "Rainbow Recipes"
date: 2025-12-17
published: true
labels:
  - Application Development
  - Database & Backend
  - Optimization and Mathematic Approach
overview: "Web application designed and implemented under the ICS314 large group project with the use of GitHub, Git, VSCode, ESLint, Prisma, and Vercel."
---

## Overview

Rainbow Recipes is basically an attempt to make cooking a less dreadful and more doable experience at the University of Hawaiʻi. It's a service aimed at university students who are in need of fast and affordable meals but at the same time, they don't have an endless amount of time, money, or patience to go running around the campus for ingredients. This tool helps to fill the big gap between the ideas of “I want to cook something decent” and “I have no idea what to make or where to get the ingredients”. Basically, it lets the users interact with recipes by searching and saving them, vendor info reading, and vendor locating through a map from which a recipe links to the real-life ingredient sourcing.

<img width="900px" class="rounded mx-auto d-block my-4" src="../img/landingPage.png">

## Contributions

In fact, most of my contributions targeted the layer which “made it look like a real application” and also those bits of the internal framework which were responsible for the app’s stability while our feature branch was working. To ensure that navigation remains user-friendly throughout the site, I came up with the footer and implemented it, because, in group projects, the small things are what really make a difference between 'done' and 'kind of thrown together'. Besides that, I took part in the backend database schema's creation and upkeep with Prisma. That involved not only making the data model neat while new functions were added but also making sure that incidental problems are not being created every time we introduce a new relationship or table.

Where the app moves beyond “just recipes” to actually engaging user life, is the point of the vendor map, and that’s the feature I’m most proud of. A recipe is nice, but it really becomes a lot more practical when the app is capable of answering the question, “so, where can I actually get these around campus?”

<img width="900px" class="rounded mx-auto d-block my-4" src="../img/mapVendor.png">

Also, the profile page construction was my responsibility, as well as the preparation for users to have a little corner of the app which is actually theirs where their account and saved things live. The work around here made me think a lot about how sign-in connects to user-specific data and how to keep the experience consistent so it doesn't feel abrupt or buggy.

<img width="900px" class="rounded mx-auto d-block my-4" src="../img/recipeList.png">

To make the system more reliable, I introduced Playwright tests because group projects have this cursed habit of breaking something that was working yesterday, and automated tests are one of the few ways to catch that early. Moreover, I arranged sign-ins and sign-outs in such a way as to render account behavior more predictable and prevent the app from being perceived as having session amnesia. Alongside the coding, I took care of most of the team's risk management and coordination, which was largely about keeping us realistic in terms of timing, cutting down on duplicated work and reducing the disorder that arose when exams and holidays made everyone's schedules unpredictable.

## What I Learned

The major point I got from the whole thing is that the problem of teamwork becomes way easier to solve when the project is structured in a manner that it facilitates teamwork. If everything depends on each other, even excellent teammates might end up obstructing each other, and the development process turns into a merge-conflict simulator. However, when the project is divided into different components with clearly defined roles, folks can work at the same time without frequent clashes, and it doesn't seem to be a compilation of half-finished ideas but rather one system. Besides that, I learned that being prepared is not wasting time even though it may seem so at the moment since the act of slowing down to agree on the structure saved us a lot of time that would have been spent in confusion later.

As far as the tools are concerned, I no longer perceive Git and GitHub as 'just submission' but rather as the backbone of real collaboration, and I understand how much my life can be simplified if I keep my database in good shape rather than gradually turning it into a messy drawer. Playwright made it very clear that testing is not an extra thing that you do when you have some free time, rather it's the way you avoid the random crashes that occur when several people are pushing their changes at the same time. On the other hand, deploying using Vercel made it very clear that "works on my laptop" doesn't really mean much unless it works reliably in a real environment too.


## Links

You can access the deployed application at [https://rainbow-recipes.vercel.app](https://rainbow-recipes.vercel.app). The GitHub organization page is accessible at [https://rainbow-recipes.github.io](https://rainbow-recipes.github.io). The source code is open for everyone directly at [https://github.com/rainbow-recipes/rainbow-recipes](https://github.com/rainbow-recipes/rainbow-recipes).
