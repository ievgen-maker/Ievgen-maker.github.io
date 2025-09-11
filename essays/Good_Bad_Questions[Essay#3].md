---
layout: essay
type: essay
title: "It’s Not You, It’s Your Question — I Think We Should See Other Forums"
date: 2025-09-10
published: true
labels:
  - Communication
  - Forums
  - Computer Science
  - Writing Skills
---

<img width="200px" class="rounded float-start pe-4" src="../img/Good_Bad_Questions.png">

*Good questions earn good answers. Communication is key.*

## Good Questions Get Good Answers

Communication is key.  

We all heard it, we all hear it, and will continue hearing it from the people that surround us on a daily basis—it’s inarguable as much as it is inescapable. Communication spans both personal and professional lives, and in both spaces, strong communication is what shapes our understanding of everything and everyone around us. From casual personal conversations to formal work presentations to moments when we need help, communication carries us through. Much of life is shaped by asking for directions and seeking help from others. Each encounter provides not only solutions but also insights that enhance our ability to navigate future challenges.  

But what exactly makes a good question to ask when you need support?  

## Natural Selection of Questions: Only the Strong Survive

We can look at *How To Ask Questions The Smart Way* by Eric Steven Raymond (ESR) as part of his essay advocating effective communication for Software Engineers, Computer Scientists, and others in technology. However, his arguments apply far beyond tech—they extend to any field and even our personal lives. Bad questions, Raymond explains, are the ones that show little effort: “My {program, configuration, SQL statement} doesn’t work” or “Why is this broken?” With no context or detail, these kinds of questions force others to play “Twenty Questions.” As Raymond notes: “I have better things to do.” Interestingly, a question can be detailed but still fail if it’s posted in the wrong forum. A misplaced question is wasted effort.  In contrast, good questions demonstrate preparation and respect. They show that the asker has tried to solve the problem, include specifics about the environment, and describe the symptoms clearly: “The code from project foo doesn’t compile under Nulix version 6.2. I’ve read the FAQ, but it doesn’t have anything in it about Nulix-related problems. Here’s a transcript of my compilation attempt; is it something I did?” Rather than demanding an answer, this kind of question, as Raymond puts it, *“gives people something to chew on”* and makes it easy for others to engage. Good questions don’t just ask for help—they contribute to the community.  

## Red Pill: Answers. Blue Pill: Awkward Silence.

Take the perfect “smart” question example:  
**[Why is processing a sorted array faster than processing an unsorted array?](https://stackoverflow.com/questions/11227809/why-is-processing-a-sorted-array-faster-than-processing-an-unsorted-array)**  

The first impression is ideal: precise in its title, clearly framing the curiosity. The author provides context: C++ environment and Java, short code snippets with comments, and a reproducible test.  

In fact, here’s the exact C++ code that demonstrated the ~6x speedup:

```cpp
#include <algorithm>
#include <ctime>
#include <iostream>

int main()
{
    // Generate data
    const unsigned arraySize = 32768;
    int data[arraySize];

    for (unsigned c = 0; c < arraySize; ++c)
        data[c] = std::rand() % 256;

    // !!! With this, the next loop runs faster.
    std::sort(data, data + arraySize);

    // Test
    clock_t start = clock();
    long long sum = 0;
    for (unsigned i = 0; i < 100000; ++i)
    {
        for (unsigned c = 0; c < arraySize; ++c)
        {   // Primary loop.
            if (data[c] >= 128)
                sum += data[c];
        }
    }

    double elapsedTime = static_cast<double>(clock()-start) / CLOCKS_PER_SEC;

    std::cout << elapsedTime << '\n';
    std::cout << "sum = " << sum << '\n';
}
```
Because the question setup was solid, the answers explained not just *what* but *why*: modern CPUs “guess” which way an `if` will go (branch prediction). Sorted data makes that guess easy—so the loop flies—while random data causes mispredictions and slows things down. Responders backed this with measurements, rewrites that avoided the `if`, and compiler optimization notes. The top response to this question literally explained theory from scratch and backed it up with run-time data to show the original issue the question author faced and why. 

This is the **red pill**: one precise, reproducible question produced precise, reusable lessons for everyone.  

By contrast, consider the vague post titled  
**[Why is my LLM generating repetitive outputs? How can I improve diversity?]([https://stackoverflow.com/questions/ask](https://stackoverflow.com/questions/79761715/why-is-my-llm-generating-repetitive-outputs-how-can-i-improve-diversity))**  

At first glance, it looks like a good question — the title sounds clear — but the body immediately stumbles. The author pastes a description of their `generate()` parameters (`do_sample=True`, `temperature=1.0`, `top_k=50`), but stops there. They never share the actual code they used, a reproducible example, or any of the model’s outputs. Instead, the post is just a wall of text saying “my output repeats phrases like a loop.”  

Readers are left guessing:  
- Which model was used?  
- What’s the input prompt?  
- How long are the generations?  
- Is this a dataset or model issue?  

Because there is no minimal reproducible example, no before/after outputs, and no baseline for comparison, responders can’t do much beyond generic advice (“try changing `repetition_penalty`” or “lower your temperature”).  

This is the **blue pill**: a seemingly well-titled question that collapses into vague problem descriptions and lacks actionable context. The thread risks stalling out or attracting downvotes — which is exactly what happened, with a negative score and no accepted solution.


<img width="400px" class="rounded float-start pe-4" src="../img/badQuestion.png">



>## TL;DR: Ask Better, Suffer Less

Good, strong questions earn attention and unlock high-signal answers.  

The “sorted array” post modeled ESR’s rules—so the community delivered layered explanations that taught beyond the original task. By contrast, the “Update public key” post lacked structure, and so it died.  

**Takeaway:** Treat forums like a lab.  
- State the goal.  
- Show the experiment.  
- Report the data.  
- Ask a focused *why*.  

That’s how you get real answers.  
