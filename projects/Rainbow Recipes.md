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
  - Optimization & Mathematical Approach
summary: "Web application developed and deployed as part of the ICS314 large group project using GitHub, Git, VSCode, ESLint, Prisma, and Vercel."
---

## Overview

Rainbow Recipes is a comprehensive platform built for University of Hawaiʻi students who want quick, affordable, and genuinely good meal options without turning cooking into a second job. Student life comes with tight budgets, limited time, and the constant question of “okay, but where do I even get the ingredients near campus?”—so the whole point of Rainbow Recipes is to bridge that gap. The app lets users browse and save recipes, explore vendor information, and use a vendor map to connect meal planning to real ingredient sourcing around UH. The live site is available at [https://rainbow-recipes.vercel.app](https://rainbow-recipes.vercel.app), and the GitHub organization page is [https://rainbow-recipes.github.io](https://rainbow-recipes.github.io) for anyone who wants the broader project context.

<img width="900px" class="rounded mx-auto d-block my-4" src="../img/landingPage.png">

## Contributions

I designed and implemented the site footer to keep navigation consistent and polished across the app, and I worked on backend database schema creation and management to keep our data model clean and reliable as features grew. I also contributed the vendor map feature so users could actually connect “this recipe looks good” to “where can I buy the ingredients near me,” and I built out the profile page so users could manage their identity and saved content in one place.

<img width="900px" class="rounded mx-auto d-block my-4" src="../img/recipeList.png">

The recipes page was one of the areas where the project started to feel like a real product instead of a prototype, because it gave users a clean, scrollable place to browse options quickly and come back to favorites later.

<img width="900px" class="rounded mx-auto d-block my-4" src="../img/mapVendor.png">

The vendor map was the feature that grounded the app in real student life, since it ties the cooking workflow to actual sourcing and makes the “how do I get this stuff?” question easier to answer.

I wrote Playwright tests to catch regressions early, configured sign-in and sign-out functionality so accounts behaved predictably, and supported the team through risk management and coordination when priorities shifted as the holidays and exams started affecting everyone’s schedules.

## What I Learned

The best lesson for me was how teamwork becomes easier when the system is built from independent parts that cooperate without clinging to each other. Once components are separated clearly, multiple people can move fast at the same time without constantly colliding (aka dealing with version issues through Git), and the project starts to feel like one thing instead of a pile of unfinished ideas.

## Links

You can visit the deployed application at [https://rainbow-recipes.vercel.app](https://rainbow-recipes.vercel.app). You can explore the GitHub organization page at [https://rainbow-recipes.github.io](https://rainbow-recipes.github.io). You can view the source code directly in the repository at [https://github.com/rainbow-recipes/rainbow-recipes](https://github.com/rainbow-recipes/rainbow-recipes).
