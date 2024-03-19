---
title: "documentation & scalability"
date: 2024-03-19
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

- **Outdated information spread** :: By the time you write detailed
  documentation, the code might have changed, making your documents inaccurate
  before they're finished.
- **Knowledge silos** :: Separate documentation becomes outdated, leading to
  knowledge gaps and hindering collaboration.
- **Demoralized team** :: Complex templates and approvals create a documentation
  burden, impacting morale and productivity.

# My take on it

### First impression

> Assuming that this scenario is the reflection of the reality, what I would try
to do is to reflect on top of the described problem and symptoms, which has a
pessimistic-view of the situation, and try to understand what might be causing
all of this.<br>-- Is it related to the process? To the team agreements? To the
work environment?

### Rationale

Given the challenges of outdated information spread across multiple locations
and a team handling too many initiatives, knowledge silos naturally form. These
silos develop around the specific deliverables of newly-created smaller working
groups.

This is often seen when engineers with specialized knowledge work on
multidisciplinary teams. As a result, the larger team may break into smaller
groups for improved management and better career development, from both the
engineers and the manager itself.

With that in mind, a clear problem that I would focus on is **scalability**.
This model, in any stage of it, raises concerns about growth. For instance,
challenges arise with **(i)** handling more initiatives, **(ii)** increasing headcount,
and **(iii)** tackling larger, more complex problems.

These growth-related side effects create a documentation burden. Different
people need to quickly understand specific aspects of your domain, either
because **(i)** you previously worked together and are now in separate groups,
or **(ii)** your reach is expanding to other domains or business units.

### Food for thought

1. **Embrace knowledge as a core aspect of your work** :: integrate knowledge
   sharing into everything from coding to project planning. This promotes
   seamless collaboration, efficient knowledge transfer, and minimizes
   disruptive context switching.

2. **Prioritize value-driven documentation** :: don't document everything
   equally. Focus on areas that will yield the highest return, e.g.:
   - **Complex logic modules** :: clearly document non-obvious design patterns
     and critical workflows
   - **External APIs** :: provide concise instructions and **examples** for
     smooth integration with external system (this also applies to your own
     **README.md**, xoxo)
   - **Frequently used parts** :: ensure up-to-date and complete documentation
     for the areas that more people look into. This is a direct indicator that a
     well-written documentation is needed
3. **Weave documentation into your workflow** :: make it a natural extension of
   a process, like:
   - **Leveraging enhanced code versioning** :: treat code versioning (git) as a
     communication tool. Encourage thoughtful commits, descriptive PR comments,
     and a focus on clarity and understanding throughout the review process.
   - **Automating where possible** :: Explore tools that generate API
     documentation from code annotations. This fosters synergy between
     documentation and GitHub commits/PRs.

### Conclusion

The key lies in continuous evolution. Documentation is a dynamic process that
must constantly adapt. Recognize that this work is ongoing and essential to
growth. By the end of the day, *it all depends* 🙃

<div style="width:100%;height:0;padding-bottom:65%;position:relative;"><iframe src="https://giphy.com/embed/C25OqSUQliU7K" width="100%" height="100%" style="position:absolute" frameBorder="0" class="giphy-embed" allowFullScreen></iframe></div>
