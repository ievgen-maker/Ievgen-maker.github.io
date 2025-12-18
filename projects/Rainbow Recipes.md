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

Rainbow Recipes is basically an effort to make cooking as a UH student achievable rather than a nightmare. It’s a service built for University of Hawaiʻi students who need fast and cheap food, but don’t have unlimited time, money, or patience to hunt down ingredients around campus. The app fills the gap between “I want to cook something decent” and “I have no idea what to make or where to get the ingredients” by letting users browse and save recipes, read vendor information, and use a vendor map to connect a recipe to real-life ingredient sourcing. The live site is at [https://rainbow-recipes.vercel.app](https://rainbow-recipes.vercel.app), and the GitHub organization page is at [https://rainbow-recipes.github.io](https://rainbow-recipes.github.io) if you want the bigger picture.

<img width="900px" class="rounded mx-auto d-block my-4" src="../img/landingPage.png">

## Contributions

A lot of what I worked on was the “make it feel like a real application” layer, plus parts of the internal structure that kept things from collapsing as features got added. I designed and implemented the footer so navigation stayed consistent across the site, because in group projects the small stuff is what makes the difference between “finished” and “kind of pasted together.” I also worked on creating and maintaining the backend database schema with Prisma, which meant keeping the data model clean as we added functionality and making sure we weren’t quietly creating future problems every time we introduced a new relationship or table.

The feature I’m most proud of is the vendor map, because that’s where the app stops being “just recipes” and starts feeling connected to real student life. A recipe is nice, but it becomes way more useful when the app can answer the question, “okay, where can I actually buy this around campus?”

<img width="900px" class="rounded mx-auto d-block my-4" src="../img/mapVendor.png">

I also built the profile page so users could have their own space in the app, where their account and saved items actually live. That work pushed me to think through how sign-in connects to user-specific data, and how to keep the experience consistent so it doesn’t feel random or buggy.

<img width="900px" class="rounded mx-auto d-block my-4" src="../img/recipeList.png">

On the reliability side, I wrote Playwright tests because group projects have this cursed habit of breaking something that worked yesterday, and automated tests are one of the few ways to catch that early. I also configured sign-in and sign-out so accounts behaved predictably and the app didn’t feel like it had session amnesia. Finally, I supported team risk management and coordination, which mostly meant keeping us realistic about timing, reducing duplicated work, and lowering the chaos when exams and holidays made everyone’s schedules unpredictable.

## What I Learned

The biggest thing I learned is that teamwork is way easier when the project is built to support teamwork. When everything is tangled together, even good teammates end up stepping on each other, and development turns into a merge-conflict simulator. But when the project is divided into independent parts with clear responsibilities, people can work in parallel without constantly colliding, and the whole thing starts to feel like one system instead of a pile of half-finished ideas.

I also learned that planning early isn’t wasted time, even though it feels like it in the moment. The times we slowed down to agree on structure—what the data should look like, what a feature is responsible for, and what a page can safely assume—were the times we saved ourselves hours of confusion later. It’s basically the difference between building with a map and walking into a forest hoping you eventually find the exit.

Tool-wise, I stopped thinking of Git and GitHub as “just submission” and started seeing them as the backbone of real collaboration. Prisma made me appreciate how much easier life is when your database stays clean instead of slowly turning into a junk drawer. Playwright taught me that testing isn’t extra credit—it’s how you keep a project from randomly collapsing when multiple people are pushing changes. And deploying through Vercel made it obvious that “works on my laptop” doesn’t mean much unless it runs reliably in a real environment too.

## Links

The deployed application is available at [https://rainbow-recipes.vercel.app](https://rainbow-recipes.vercel.app). The GitHub organization page is available at [https://rainbow-recipes.github.io](https://rainbow-recipes.github.io). The source code is available directly at [https://github.com/rainbow-recipes/rainbow-recipes](https://github.com/rainbow-recipes/rainbow-recipes).

