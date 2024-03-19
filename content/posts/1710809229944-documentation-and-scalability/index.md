---
title: "documentation & scalability"
date: 2024-03-18
draft: false
description: "a description"
summary: "I talk about writing docs and my current software engineering perspective about it, food for thoughts I would say."
showHero: true
heroStyle: "big"
showSummary: true
showTaxonomies: true
slug: "documentation-and-scalability"
tags: ["code", "thoughts"]
---
<h2 class="mt-0">through the space</h2>
{{< spotify type="track" id="1ujxjsoNvh4XgS2fUNwkZ2" width="auto" height="100" >}}


# The scenario

You're a software engineer in a fast-paced development team. You are astonished
by the complex dynamic nature of agile methods - the quick iterations, the close
collaboration, the emphasis on getting things done. On top of all that, there's
one more thing that keeps your mind awake: documentation.

You know it's important, but every formal documentation process you've
encountered feels like wading through molasses. Too much bureaucracy, and not
enough focus on what really helps what you're doing to succeed.

# The ~*hypothetical*~ problem

A traditional (or more conservative) documentation process approaches often
treat it as a separate activity at the end of a development phase. While this
may not always be the case, it is a common problem in many teams that I've
worked for to document things in an effective way. This creates several
symptoms, like:

- **Outdated Information Spread** :: By the time you write detailed
  documentation, the code might have changed, making your documents inaccurate
  before they're finished.
- **Knowledge Silos** :: Separate documentation becomes outdated, leading to
  knowledge gaps and hindering collaboration.
- **Demoralized Team** :: Complex templates and approvals create a documentation
  burden, impacting morale and productivity.

# My take on it

### First impression

> Assuming that this scenario is the reflection of the reality, I would try to
do is to reflect on top of the described problems, which has a pessimistic-view
of the situation, and try to understand what might be causing all of this.<br>--
Is it related to the process? To the team agreements? To the work environment?

### Rationale

Given the perception that outdated information might be spread over several
places, with a team that handles too many initiatives, this is naturally going
to create silos based on the knowledge of a specific deliverable that the newly
created small group of people are working together. This can also lead to a team
break into smaller group of people to have a better management overall.

With that in mind, a clear problem that I would focus on is **scalability**.
This model, in any stage of it, indicates a red flag when it comes to growing,
for instance **(i)** receiving more initiatives, **(ii)** getting more
head-count, **(iii)** striving to break bigger and more complex problems.

All of that growing side-effects generates a burden in documentation, because
different people are going to need to understand something specific from your
domain really quickly, either because **(i)** you used to work together and now
are in different packs, or because **(ii)** you're expanding your reach to other
domains/BUs.

### Food for thought

1. Treat knowledge as a living part of your job - from coding to conceiving new
   initiatives. Introducing this as a natural part of your flow is going to
   foster smoother collaboration, knowledge transfer, and reduces
   context-switching overhead.
2. Prioritize value-driven documentation, so **don't document everything
   equally**. Focus on areas that will yield the highest return, e.g.:
   - **Complex logic modules** :: clearly document non-obvious design patterns
     and critical workflows
   - **External APIs** :: provide concise instructions and **examples** for
     smooth integration with external system (and this also applies to your own
     **README.md**, xoxo)
   - **Frequently used parts** :: ensure up-to-date and complete documentation
     for the areas that more people look into. This is a direct indicator that a
     well-written documentation is needed
3. Integrate your documentation in your workflow, making a natural extension of
   a process, like:
   - **Enhanced code versioning** :: treat code versioning (git) like a
     communication system, and make it serious. Embrace and try to encourage
     other engineers to be more critical in PRs, write better commits, better PR
     descriptions, consider carefully the words and the way that they're going
     to expose this information so it's useful and easy-to-understand at the
     same time.
   - **Automation** :: you can use some tools that automatically generate API
     documentation based on code annotations or something like it. This also
     opens an opportunity to **use the above suggestion** - that way you can
     integrate documentation and GitHub commits/PRs, for example.

### Conclusion

It all depends. This is a continuous cycle that should never stop evolving, thus
implicating that this work is infinite (or undefined).

<div style="width:100%;height:0;padding-bottom:65%;position:relative;"><iframe src="https://giphy.com/embed/C25OqSUQliU7K" width="100%" height="100%" style="position:absolute" frameBorder="0" class="giphy-embed" allowFullScreen></iframe></div>
