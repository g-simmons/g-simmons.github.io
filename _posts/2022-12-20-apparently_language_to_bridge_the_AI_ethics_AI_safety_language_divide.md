---
layout: post
title: "The Apparent Perspective: Language to Bridge the Anthropomorphism Divide"
date: 2022-12-20 11:12:00-0400
description: Why AI safety and AI ethics folks keep talking past each other, and what we can do about it.
---

### A story as old as Twitter:

Anyone who is on AI Twitter has probably seen the pattern I'm about to describe. 

**It starts in the "AI safety" camp:**
- Study the text artifacts that language models produce under certain conditions
- Find an interesting pattern 
- Language models are obviously just doing  $$ P(w_i \vert w_{i-1} \ldots w_1) $$, but *a lay person might interpret the pattern as human-like behavior* 
- Out of concern for how people might be impacted by this pattern, publish the results.
- Assuming that readers can figure out the anthropomorphic status of AI systems on their own, take liberties with anthropomorphic language.

**Then it continues in the "AI ethics" camp:**
- AI research lab releases a new paper
- Paper contains language that suggests LMs are doing some human-like behavior 
- Language models are obviously just doing $$ P(w_i \vert w_{i-1} \ldots w_1) $$, the paper is clearly anthropomorphizing
- This might *mislead people into thinking LMs are doing more than they actually are.* 
- Out of concern for how people might *be misled by this AI hype*: 
	- point out the liberal anthropomorphization and/or 
	- reframe the paper with language that is *conservative* w/r/t anthropomorphization

### Why am I writing about this? 

The fact that this has become so predictable suggests that this cycle has exhausted its utility. People are spending their time and energy engaging in both sides of this pattern, and from my perspective it seems like returns are diminishing. AI safety folks keep publishing papers with liberal anthropomorphization, AI ethicists keep pointing out the anthropomorphization, and the cycle continues. I think both sides are probably motivated by an earnest concern for humanity, and the discourse could be much more productive if this point of friction were resolved.

### What do I see as the crux of the issue?

**Appearances matter:** Humans have a strong tendency to ascribe agency and other human characteristics even to systems where most agree that no such characteristics exist, like robot vacuum cleaners or Amazon Alexa. In a future where humans more frequently interact with LLMs and the text artifacts they produce, or interact with LLM+'s and their outputs, appearances will matter. 

Both sides are acting out of concerns for how activities in the field of AI impact society. 
- The AI ethics camp is concerned that the capabilities of language models are overhyped and overly anthropomorphized. 
- The AI safety camp is concerned that LMs will have as-yet unpredictable societal impacts. 

### Why is resolving this issue important?

Two valid research agendas that are currently pursued with friction could be pursued cooperatively:

**Agenda 1:** Understand the anthropomorphic status of LLMs, LLM+'s, and artificial intelligences in general. Give the public a clear perspective on what AI systems can and cannot do. Help people avoid anthropomorphization (for current AI systems that are largely agreed to not be human-like), or apply the appropriate degree of anthropomorphization (in the case that some future AI systems are found to be human-like to some degree). 

**Agenda 2:** Understand LLMs, LLM+'s, and artificial intelligences in general from the *apparent perspective (see below)*. People will likely interact with AI systems without a complete education about their anthropomorphic status. What should be done on the systems side in anticipation of this? 

### What do I propose as a solution? 
The apparent perspective.

<iframe width="600" height="400" src="https://www.youtube.com/embed/rz5TGN7eUcM" title="Apparently This Kid is Awesome, Steals the Show During Interview" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Video: Noah Ritter exemplifying the apparent perspective.

**What's the "apparent perspective"?**: This is the perspective that a lay person would take on text artifacts produced by LMs if the source of the text was not known. The apparent perspective asks the following: Without knowledge of who or what wrote this text, how could it be interpreted? 

**Solutions for the anthropomorphically liberal:**
Use language that acknowledges the unclear anthropomorphic status of LLMs, while at the same time fosters productive discourse from the apparent perspective. Make it clear when you are taking the apparent perspective. I think this approach offers real benefit, as language that is imprecise or too liberal w/r/t anthropomorphic status of LMs will cause some readers to dismiss the entire paper.

**Solutions for the anthropomorphically conservative:**
Have a little bit of patience w/r/t overly-anthropomorphized results from the liberal camp. Consider what results would mean from the apparent perspective. Could you see a lay person anthropomorphizing the LM behavior (especially if they didn't know it was an LM)? Does this have meaningful implications?

### Language for the apparent perspective:

Here are some examples of how I might reframe language that is anthropomorphically liberal to be more transparent:

- "Arguments" -> "Apparently-argumentative text artifacts"
- "Desires" -> "Apparent desires"
- ...

The key is that this language shift moves potential criticism from "is the language model actually doing that?" (usually not the point) to "could a human interpret the text artifact that way?" (a trailhead for an interesting research agenda!).

For those making criticisms along the lines of "is the language model actually doing that?", the language shifts above can also be used while reading. If it looks like the authors are assuming language models are conscious, what if they were making a different assumption? What if they were assuming a lay person might *interpret* the outputs of LLMs as if they were written by a conscious entity?

### Why the apparent perspective is worth taking seriously

- Lay people may interact with text artifacts where it is unclear whether the text is written by a human or AI system. There have been some suggestions to mandate that AI products disclose when text artifacts (or video, etc) are produced by an AI, but it's conceivable that some AI products would skirt such hypothetical regulations.

- At a certain level of fluency, it might become difficult not to see LLM-produced text artifacts through an anthropomorphic lens, even if the source is known. The LaMDA incident is an early instance of this - if LM fluency increases, this might become more widespread. Imprecise language from AI researchers definitely doesn't help, but it's not the only issue at hand. Even with an education in the anthropomorphic status of AI systems, people might still gravitate towards the apparent perspective because it's *easier*. This bears similarity to certain optical illusions - even when the mechanism for the illusion is known, it's difficult to "unsee" it.

### TLDR
I am offering a solution for a pattern of discourse that doesn't look productive from my perspective. In this pattern, research results are presented in a way that anthropomorphizes a non-human AI system. Critics fixate on the anthropomorphization, which distracts from the actual point of the paper. The apparent perspective is a view on AI systems that considers whether a lay person might ascribe human qualities to AI systems or their outputs. Authors studying AI systems can make it explicit when they are taking the apparent perspective by simple rephrasing. Readers can apply the apparent perspective at reading time to see beyond distracting anthropomorphization.

### Clarifying terminology:

**What's anthropomorphization?:** Ascribing human-like characteristics to something non-human, where presumably the characteristics do not exist.

**What do I mean by anthropomorphic status?**: I am using this phrase to refer to the status of AI systems with respect to agency, consciousness, sentience, intentionality, desire, etc. The consensus view is that most of these qualities are present in humans and not present in today's AI systems. Whether these qualities might exist in a future AI system (a "pure" language model, or an LLM+ a la David Chalmers) is an open philosophical question. 

**What do I mean by anthropomorphically liberal or anthropomorphically conservative language?** Anthropomorphically conservative language is careful not to ascribe human qualities to non-human entities (AI systems in this context). In contrast, anthropomorphically liberal language describes AI system behavior with human-like descriptors "when the shoe fits" (when a lay person might use those descriptors). 

### Disclaimers:

I'm only qualified to comment on this phenomenon as a consumer of AI Twitter discourse, and as someone who is interested in AI and human interaction. It's likely that the discourse pattern I identify here appears more "campish" and polarized on Twitter than it is in actuality. I think those on the AI ethics side have a valid point in asking for more precise language w/r/t anthropomorphization. I think the AI safety side also has a valid point in asking readers to consider results from the apparent perspective. The apparent perspective is not valid in all cases - in the case that AI system outputs could not be mistaken for human-produced artifacts, treating them as such would be silly. In less clear-cut cases, I think it is an open question worthy of pursuit whether LM-produced and human-produced artifacts are distinguishable. 