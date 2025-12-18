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
summary: "Web application designed and implemented under the ICS314 large group project with the use of GitHub, Git, VSCode, ESLint, Prisma, and Vercel."
---

## Overview

Rainbow Recipes is an initiative to make cooking at the University of Hawaiʻi a viable and not a terrifying experience. It is a service designed for the University of Hawaiʻi students who require quick and cheap meals but do not have the unlimited time, money, or patience to go hunting for ingredients around the campus. The application bridges the gap between “I want to cook something decent” and “I have no idea what to make or where to get the ingredients” by allowing users to browse and save recipes, read vendor information, and use a vendor map to connect a recipe to real-life ingredient sourcing. So, if you want to have the bigger picture, the live site is at [https://rainbow-recipes.vercel.app](https://rainbow-recipes.vercel.app), and the GitHub organization page is at [https://rainbow-recipes.github.io](https://rainbow-recipes.github.io).

<img width="900px" class="rounded mx-auto d-block my-4" src="../img/landingPage.png">

## Contributions

Most of the work I did was the “make it feel like a real application” layer, and also the parts of the internal structure that helped the app to stay stable as we added new features. Navigation was made consistent across the site by me designing and implementing the footer because, in group projects, the small stuff is what makes the difference between “finished” and “kind of pasted together.” Besides that, I was involved in the creation and upkeep of the backend database schema with Prisma. This task entailed that we keep the data model clean while adding new functionalities and also that we do not quietly create a lot of problems for the future every time we introduce a new relationship or table.

The vendor map is the feature of which I am the most proud because it is the place where the app ceases to be “just recipes” and starts feeling like it is real student life. A recipe is good, but it is a lot more efficient when the app can answer the question, “okay, where can I actually buy this around campus?”

<img width="900px" class="rounded mx-auto d-block my-4" src="../img/mapVendor.png">

The profile page is also something I put together so that users might get a little corner of the app for themselves where their account and saved things are really. That job made me consider the issue of how sign-in is linked with user-specific data and how to maintain the experience so that it is not abrupt or buggy.

<img width="900px" class="rounded mx-auto d-block my-4" src="../img/recipeList.png">

In order to improve the project’s reliability, I introduced Playwright tests. The reason is that group projects have this cursed habit of breaking something that was working yesterday, and automated tests are among the few means to discover such breakings at their early stage. Also, to make account behavior more predictable and the app less like it has session amnesia, I set up sign-in and sign-out. And, at the end of the day, I was the guy behind the team’s risk management and coordination. Mostly it refers to being the one who ensured that we were realistic about the timing, cutting down on the duplicated work, and lessening the disorder when exams and holidays made everyone’s schedules unpredictable.

## What I Learned

The most important thing that I learned is that teamwork becomes a lot more doable when the project is designed in such a way that supports teamwork. If everything is intertwined, then even good teammates end up interfering with each other, and the process of development turns into a merge-conflict simulator. However, when the project is broken down into separate units with well-defined duties, individuals can work simultaneously without constantly bumping into each other, and at that point, the whole thing starts to look like one system rather than a collection of half-finished ideas.

Moreover, I was taught that planning ahead is not throwing away time even though it may seem so. The moments when we took the time to slow down and reach an agreement on structure—that included the look of the data, the responsibilities of the feature, and what could be safely assumed about the page—were also the times we rescued ourselves from hours of confusion later on. It’s basically the difference between constructing with a map and entering a forest, hoping to find the exit eventually.

Regarding tools, I ceased to consider Git and GitHub as “merely submission” and started recognizing them as the core of actual collaboration. Prisma introduced me to the concept of how significantly easier life can be if your database is well-maintained rather than gradually turning into a junk drawer. Playwright showed me that testing should not be regarded as a mere extra that deserves to be done, but rather it is the way to prevent a project from sudden and random crashes when multiple people are making changes simultaneously. Also, doing the deployment via Vercel made it very clear that “works on my laptop” is not really that much unless it is done reliably in a real environment as well.

## Links

You can access the deployed application at [https://rainbow-recipes.vercel.app](https://rainbow-recipes.vercel.app). The GitHub organization page is accessible at [https://rainbow-recipes.github.io](https://rainbow-recipes.github.io). The source code is open for everyone directly at [https://github.com/rainbow-recipes/rainbow-recipes](https://github.com/rainbow-recipes/rainbow-recipes).
