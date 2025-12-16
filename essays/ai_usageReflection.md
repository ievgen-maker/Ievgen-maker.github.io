---
layout: essay
type: essay
title: "Cooking With AI or Getting Cooked By AI"
date: 2025-12-15
published: true
labels:
  - Software Engineering
  - Education
  - AI
  - Reflection
---

<img width="200px" class="rounded float-start pe-4" src="../img/aiGoodBad.png">

*AI isn’t automatically good or bad—it just amplifies whatever habits you already have.*

## I. Introduction

AI can either be the best tool or the worst tool ever designed, depending on how you use it. In education, having instant access to a deep explanation that can be tuned to *your* level is honestly invaluable. At the same time, it can create real challenges with learning if you start relying on it without actually understanding what it’s doing. In my personal experience, I’ve seen this happen to me and to other people who use AI tools like ChatGPT: the time saved and the “high-quality output” at first is enough to pull you in, and if you’re not careful, that turns into overreliance and laziness instead of struggle, growth, and real comprehension.

In Software Engineering (and specifically in ICS 314), this matters a lot because the course is built around practice, repetition, and applying concepts under pressure (WODs especially). AI can accelerate learning *way* more than ever before if you use it to learn and engage—rather than just doing Ctrl+C / Ctrl+V. For this course, the main AI tools I’ve used (or experimented with) are **ChatGPT**, and occasionally **GitHub Copilot** (for small suggestions/autocomplete), plus **Bard/Gemini** a few times to compare explanations when ChatGPT felt off or overconfident.


## II. Personal Experience with AI (ICS 314)

### 1 Experience WODs (e.g., E18)

For experience WODs, it’s basically the same WOD pressure but with a slightly different flavor: you still need speed, but you also need accuracy because the task usually has hidden “gotchas.” AI was most useful here when I treated it like a *debugging mirror* instead of a *solution generator*.

**Example prompts I used:**
- “Create a practice WOD similar to **E18**. Focus on the same skills, but change the data and requirements so I can’t memorize the answer.”
- “Here is my code. I’m getting `undefined` when I run it—point out the bug but don’t rewrite the whole solution.”
- “List 5 edge cases this code might fail on based on the instructions.”

**How useful it was / benefits:**
- Helped me generate extra reps so I wasn’t practicing only one exact version of the WOD.
- Helped with small bugs that would otherwise eat time under pressure.
- Helped me think about edge cases faster, which is usually what separates “almost done” from “done.”

**Costs:**
- If I used AI too early, it reduced my ability to build the solution from scratch on my own.
- Sometimes it suggested solutions that worked in general, but didn’t match the course’s intended approach.


### 2 In-class Practice WODs

In-class practice WODs are where AI can either help you build skill or quietly destroy it, depending on whether you’re using it as a tutor or as a shortcut. I tried to use AI for *micro-help*—one concept, one bug, one line—so the practice still stayed real.

**Example prompts I used:**
- “Explain this underscore function in one paragraph and give me a tiny example.”
- “Give me a hint for how to start, but don’t write the full solution.”
- “What does this error message usually mean in JavaScript?”

**Benefits:**
- Faster recovery when I got stuck early.
- Better understanding when I asked for explanations, not answers.
- More practice volume overall because I spent less time stalled.

**Costs:**
- Easy to accidentally “borrow” logic without truly learning it.
- Sometimes the explanation was technically correct but not intuitive, which slowed me down anyway.


### 3 In-class WODs

In-class WODs are the most high-stress version of the same skillset: time constraints, performance pressure, and limited room for mistakes. After enough practice, AI became less of a teacher and more of a *panic button* for weird edge cases or syntax blanks.

**Example prompts I used (rarely during the actual WOD context):**
- “I blanked on the syntax for X—show me the minimal example.”
- “This edge case fails. Why? Here is the input/output.”

**Benefits:**
- Quick syntax reminders when my brain was more stressed than stupid.
- Reduced the chance of losing the whole WOD to one small mistake.

**Costs:**
- Using it during a timed assessment can turn into dependency if you’re not careful.
- The risk isn’t just academic—it’s personal confidence. If AI becomes the safety net, you stop trusting your own thinking.


### 4 Essays

AI is good for a quick scan, grammar cleanup, and helping organize thoughts. It can also generate a draft, but that’s where the danger is: generating a draft can trap you in a false sense of “I wrote this,” when really the voice and authenticity are missing.

**Example prompts I used:**
- “Check this paragraph for grammar and flow, but keep my diction and tone.”
- “Give me 3 stronger thesis options based on what I already wrote—don’t add new claims I didn’t make.”
- “Point out where my argument jumps too fast and suggest transitions.”

**Benefits:**
- Saves time on revision and clarity.
- Makes structure problems obvious (weak transitions, unclear thesis, repetitive points).

**Costs:**
- If you let it write too much, your essay starts sounding like AI.
- It can suggest claims that sound good but aren’t actually grounded in what you wrote.


### 5 Final project

In larger settings like team work, AI performs relative to the context: the people involved, the codebase size, and the specificity of the problem. It’s really good at giving a coding draft, but those drafts often miss edge cases and project conventions.

**Example prompts I used:**
- “Here’s our current function and the bug we’re seeing. Suggest a minimal fix that doesn’t change the function signature.”
- “Given this React component, how can I refactor it to reduce duplication without changing behavior?”
- “List likely edge cases for this feature based on the requirements.”

**Benefits:**
- Quick “directory understanding” when I pasted small, focused snippets + context.
- Helpful for debugging and brainstorming test cases.
- Best when used to *fix my code* rather than generate new code from scratch.

**Costs:**
- Sometimes it went out of scope and suggested changes that broke other working parts.
- If I asked it to rewrite an entire file, it tended to overcorrect and “rebuild” things that didn’t need rebuilding.


### 6 Learning a concept / tutorial

This one is dependent on prompting. A weak prompt leads to either irrelevant teaching or a complicated explanation that doesn’t match your level. A strong prompt makes AI feel like a personal tutor.

**Example prompts I used:**
- “Teach me this concept like I’m in ICS 314. Use a simple example, then a slightly harder one.”
- “Explain this in 5 sentences first, then expand if I ask.”
- “I’m confused about X vs Y—compare them and give one example.”

**Benefits:**
- Fast clarity when the explanation is tuned correctly.
- Good bridge from “I’m lost” to “I can actually try this now.”

**Costs:**
- Bad prompts waste time and can mislead.
- Sometimes the explanation is correct but still not usable under pressure.


### 7 Answering a question in class or in Discord

I don’t have a ton of experience using AI directly for this, but I can see how it helps with quick clarification. The main risk is that it can produce answers that are “too much” for the moment.

**Example prompts I used (rarely):**
- “Give a short, beginner-friendly explanation I could post in Discord (no jargon).”
- “Explain why this bug happens in plain English, then show a tiny fix.”

**Benefits:**
- Helps communicate clearly.
- Faster support when someone is stuck.

**Costs:**
- Can overwhelm people with overengineered responses.
- Still requires judgment about course level and what’s appropriate to share.


### 8 Asking or answering a smart-question

Same logic as above. AI is useful here because it can turn a vague question into something answerable, which is a real skill in software engineering.

**Example prompts I used:**
- “Turn my question into a ‘smart question’ with the right technical details included.”
- “What info am I missing that I should include to get help debugging this?”

**Benefits:**
- Reinforces good habits: context, expected vs actual output, minimal reproduction.
- Helps you learn how to ask better questions over time.

**Costs:**
- If you always rely on AI to form the question, you don’t develop the skill naturally.


### 9 Coding example (e.g., “give an example of using Underscore .pluck”)

I honestly didn’t use AI much for this. I stayed personally interested in figuring out examples myself, because examples are where you can accidentally inherit a solution and stop thinking.

**What I did instead (when tempted):**
- I’d look up the docs or class examples first, then only ask AI if I was still confused.

**Why:**
- For me, building the example is part of the learning.
- If the example is “gifted” to you too easily, your brain doesn’t build the connection.


### 10 Explaining code

AI is useful for explaining code *when you already have the code*. It helps surface assumptions and logic paths you might not notice.

**Example prompts I used:**
- “Explain what this function does and what assumptions it makes.”
- “Summarize this code in 5 bullet points, then tell me one thing that could go wrong.”

**Benefits:**
- Helps me verify I understand what I wrote.
- Makes it easier to communicate with teammates.

**Costs:**
- AI can sound confident even when it misunderstands intent.
- If you trust the explanation blindly, you can end up misunderstanding your own code.


### 11 Writing code

AI is strongest when writing code in *small pieces*, not entire files. The more you ask it to generate, the more likely it goes out of scope.

**Example prompts I used:**
- “Write a helper function that does X, and match this style (no extra features).”
- “Given this function signature, implement the missing logic but don’t change anything else.”

**Benefits:**
- Quick drafts for small functions.
- Useful when I already know what I want and just need a clean starting point.

**Costs:**
- It sometimes misses edge cases and requirements.
- Too easy to accept code without truly owning the logic.


### 12 Documenting code

This is one of the cleaner uses because documentation is about clarity, not invention.

**Example prompts I used:**
- “Write JSDoc comments for this function based on what it currently does (don’t change logic).”
- “Rewrite this comment to be clearer and shorter.”

**Benefits:**
- Makes code easier to maintain and hand off.
- Encourages good habits (clear contracts, clear assumptions).

**Costs:**
- Documentation can become “fluffy” unless you keep it strict.
- If the AI misunderstood the code, it can document the wrong behavior.

---

### 13 Quality assurance (e.g., “What’s wrong with this code <code here>” or “Fix the ESLint errors in <code here>”)

This is one of the most practical uses. QA questions are well-scoped and grounded in concrete errors.

**Example prompts I used:**
- “Here are the ESLint errors—fix them with minimal changes and explain each fix.”
- “This test fails only on this case. Why? Here’s the input/output.”
- “Point out the bug and explain it, but don’t rewrite the whole function.”

**Benefits:**
- Huge time saver.
- Helps you learn patterns through repetition (lint issues, common JS mistakes).

**Costs:**
- Easy to accept fixes without learning why they matter.
- Sometimes it “fixes” by silencing warnings rather than improving the code.

---

### 14 Other uses in ICS 314 not listed

**Other ways I used AI:**
- **Planning + checklists:** “Given this requirement, list the steps I should implement in order.”
- **Edge-case brainstorming:** “What are 10 edge cases for this input validation?”
- **Rubber-duck debugging:** “Ask me questions to help me debug this instead of giving the answer.”

**Benefit:**
- Helps structure work and keep momentum.

**Cost:**
- If you treat it like an oracle instead of a tool, you stop verifying things yourself.


## III. Impact on Learning and Understanding

AI has influenced my learning in a way that is both positive and risky. On the positive side, it boosted my speed and confidence when I used it correctly: clarifying concepts, debugging small issues, and generating extra reps for WOD-style practice. It made the “getting unstuck” moments shorter, which kept me practicing instead of spiraling.

But on the other side, it definitely creates a temptation to skip the hard part—the part where your brain has to sit in confusion and actually build the mental model. If I used AI too early, my comprehension got weaker because I never forced myself to struggle through the logic. So in my opinion, AI enhanced my problem-solving most when I used it *after* I attempted the problem and had something concrete to debug or improve.


## IV. Practical Applications Outside ICS 314

Outside ICS 314, AI tools feel even more “real” because real-world coding is full of documentation, unfamiliar libraries, and constant debugging. AI can be effective for:
- speeding up onboarding into a codebase,
- generating checklists and test ideas,
- and catching obvious mistakes early.

In collaborative settings (like group projects or hackathon-style work), the effectiveness depends on discipline: if the team uses AI to accelerate understanding, it’s a boost; if the team uses AI to replace understanding, it becomes technical debt waiting to happen.


## V. Challenges and Opportunities

**Challenges/limitations I encountered:**
- AI can be confidently wrong, and beginners often can’t tell.
- It can overengineer solutions, which hurts learning and sometimes breaks project constraints.
- It can “solve” in a way that bypasses the course’s intended skill-building.

**Opportunities for better integration:**
- Using AI explicitly as a teaching assistant: guided prompts, concept checks, and “explain your reasoning” workflows.
- Teaching students how to prompt responsibly (small scope, minimal changes, verify output).
- Encouraging AI use for debugging and reflection rather than full-solution generation.


## VI. Comparative Analysis: Traditional vs AI-Enhanced Approaches

Traditional teaching methods (lectures, docs, practice, office hours) build fundamentals and discipline, but they can be slower when you’re stuck at 1am on a small bug. AI-enhanced learning improves engagement because feedback is instant, and it can increase retention *if* you use it as an interactive tutor.

The main difference is this: traditional methods force you to slow down and think; AI lets you move fast. Speed is good, but only if you’re still learning. So the best approach is a hybrid: fundamentals from traditional methods, plus AI as a targeted assistant for clarification, debugging, and extra practice.


## VII. Future Considerations

In the future, I think AI will become a normal part of software engineering education, but the focus should shift from “can you avoid AI” to “can you use AI without losing your skills.” Advancements will make AI more integrated into IDEs and workflows, but that also increases the need for strong judgment: verification, testing, and understanding.

The biggest improvement area is teaching students *how to use AI responsibly*: how to scope prompts, how to validate outputs, how to learn from explanations, and how to avoid dependency.


## VIII. Conclusion

Overall, my reflection is that AI in ICS 314 can be either a huge advantage or a huge trap. It saves time, improves iteration speed, and can accelerate learning—especially for debugging, concept clarification, and extra WOD practice. But it can also create overreliance, weaken comprehension, and reduce authentic problem-solving if it becomes a shortcut.

My main recommendation is to integrate AI in a way that encourages learning rather than replacement: promote small, targeted prompts; require verification; and treat AI like a powerful tool that you control—not something that controls your effort. At the end of the day, the impact of AI isn’t determined by the tool itself—it’s determined by how we choose to interact with it.
