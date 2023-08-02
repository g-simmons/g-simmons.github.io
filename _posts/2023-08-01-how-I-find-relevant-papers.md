---
layout: post
title: "How I Find Relevant Papers"
date: 2023-07-25 11:12:00-0400
description: "It's not hard, but it takes time."
---

"ML moves fast, it's so hard to keep up". If I had an NVIDIA H100 SXM 80GB for every time I heard this...

I'll describe my method, your mileage may vary. If you end up developing an alternative approach, I'd be curious to hear about it! 

"Keeping up with ML" can mean differen things. My approach is divided into two parts:
- Part 1 is about keeping up with *general trends* in the field of NLP and ML more broadly.
- Part 2 is about finding relevant work and keeping up with progress on specific topics.

## Part 1: Broad Trends

For broad trends in the field, I listen to a lot of podcasts and scroll Twitter. Any time anyone says something interesting about ML, follow them on Twitter. Cool paper - follow the authors. Cool blog post - follow the author. Cool podcast - follow the guest. Podcast guest mentions someone else who sounds cool - follow them.

I especially recommend to follow Twitter accounts that filter new paper releases. Both AK's ([Aran Komatsuzaki](https://twitter.com/arankomatsuzaki) and [A. Khaliq](https://twitter.com/_akhaliq)) are great examples of this. [John Nay](https://twitter.com/johnjnay) is another account who just started recently and happens to post about things close to my research interests.

Podcasts I listen to:

  - [AXRP Podcast](axrp.net)
  - [The Inside View](theinsideview.ai)
  - [The Lunar Society](https://www.dwarkeshpatel.com/podcast)
  - Machine Ethics Podcast
  - Machine Learning Street Talk
  - Some episodes of Lex Fridman


## Part 2: Specific topics

Broad trends will often only be tangentially relevant to the specific thing you're working on. Here's how I find relevant papers for specific topics I'm interested in:

### Initial Searching

#### A common fallacy - "novel" == "no related work"
At this point, I suggest that you take the attitude of "there is nothing new under the sun" - there *has* to be relevant work.

A mistake I made was thinking...

"Ok I need to do novel research. That means there's probably not gonna be related work". 

...then confirmation bias kicks in, and after 5 minutes of google searching, I would think... 

"guess I was right, there's no relevant literature, I'm on my own". 

Then 3 months into the project, I find out someone did it already 🙃. Better to know in advance.

#### The four hindrances to finding related work

For me, the roots of this fallacious thinking were:
- hubris
- naivete
- fear of having to abandon my idea
- not understanding constitutes "novelty" or "relatedness"

#### The initial search
Start with the keywords you are aware of. Search these keywords, and find some papers that are relevant to what you're looking for in *at least one aspect*. 

This can be the same method, different domain. Or same domain, different problem setup. Or same algorithm, different problem setup. And so on...


### Search Engine
I use [Semantic Scholar](https://www.semanticscholar.org/me/research) for most of my literature searches. 

### Let the recommender do the work
Add the relevant papers you find to a folder in Semantic Scholar. Each folder gives you **email recommendations of papers related to those in the folder.** Make sure you're subscribed for email recommendations. Semantic Scholar calls these "Research Feeds". I typically start with one research feed for the project. 

Read the research feeds, and when relevant papers turn up, add them to the folder. The Semantic Scholar recommender system is actually quite good -- with a focused collection of a dozen papers in a folder it's worth the time to read the recommendations.

### Expand the keyword list, do more searches
As you add some relevant papers, **expand your keyword list** - different authors will refer to the same thing with different names. 

**Do new variants of your searches with different combinations of keywords.** Filter the search results, add the relevant ones to the folder, repeat. 

A complete keyword list should have at least a dozen entries.

Here's an example of a keyword list from a project I was working on:

```
## Keywords:
Look at AI personification/ LLM personality keywords
MFT
Moral Foundations Theory
Morality
Morals
Ethics
Ethical
Ethical Judgements
Ethical decision-making
Moral foundations
Conservative
Liberal
Political ideology
Political identity
Foundation Models
Bot
rhetoric
bot-generated content
Computational argumentation
```

### Getting even more focused:

As the project expands or you take on multiple projects, subthemes will start to emerge, and often these will be common across projects. When I encounter this I **make a separate folder for each subtheme**. This gives the recommender a much tighter cluster of papers to use as examples, resulting in **higher-quality recommendations**.

For example, if you're doing *synthetic text data generation*, and working in the *low-resource NLP subdomain*, you might make a folder for each. Then you can get recommendations for similar methods in different domains, *and* recommendations for different methods in the same domain, without confusing the recommender.

## Part 3: The value of reading a lot:
Personal experiences vary, but I feel like **something clicked for me only after reading 100-200 papers**. 

Before that point, I didn't have a confident sense of what to search for, how much related literature to expect for a given idea, etc. etc. After reading some 200 papers, I felt much more confident about this, and was able to open a paper and quickly understand the contributions and whether it's relevant to my project or not. 

This isn't a flex, I'm sure there are folks out there who might have the same experience after only 10-20 papers. When I listen to early-PhD friends, I often think that many of their problems would solve themselves if they just read a couple hundred papers.

Also, to be clear, this was **not a deep reading** - most of these were converted to audio that I listened to once while driving or doing chores.
 
At 1.5x speed a typical paper can be 30-40 minutes long, so this is something like 100 hours of listening time. I did this piecewise maybe 1-4 papers at a time, over a span of months. More than 4 papers back-to-back was too fatiguing.

The goal here isn't to collect knowledge - that's what deep reading is for. The goal is to collect a lot of pointers to what's "out there", to get a general sense for what's going on in the literature and expand your domain vocabulary/keyword list, so you at least know what you don't know.

Once you feel like your list of relevant work is closer to complete, you know what you don't know, then you can allocate your deep reading budget more effectively, focusing on the highly-relevant papers.

