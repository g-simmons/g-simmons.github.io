---
layout: blog_page
title: Moral Mimicry
description: Can large language models reproduce the moral biases of political groups?
img: /assets/img/pillars.jpg
importance: 1
---

In the past decades, the United States has seen a rise in political polarization. Liberals and conservatives talk past each other, with common ground apparently getting smaller and smaller. What's behind this phenomenon? 

A theory from moral psychology offers one answer to this question: liberals and conservatives have different *moral foundations*. 

<img class="img-fluid z-depth-1" src="{{ '/assets/img/pillars.jpg' | relative_url }}" style="width:50%;margin:auto;display:inherit;">

#### Moral Foundations Theory
Moral Foundations Theory (MFT) attempts to explain this variance. MFT is a theory of morality that argues that people's moral sensibilities draw on five themes, or "foundations". For those with a background in math or machine learning, you might think of the moral foundations as the principal components of moral reasoning. The *Moral Foundations Hypothesis* argues that the relative importance of these foundations varies across social groups, with liberals and conservatives in the US being an example. The "Care" foundation is more important to liberals in the United States than to conservatives, and conservatives value the "Authority" foundation more than liberals. In fact, this variance in moral biases is not just a US phenomenon, but is also observed in other countries. Human social groups tend to vary in the relative importance of certain moral themes, and this variation is reflected in their moral reasoning.

The Moral Foundations Hypothesis offers an explanation for why people of differing social groups might talk past each other when it comes to moral issues. It also offers optimism - acknowledging and studying this difference could help to bridge ideological gaps and encourage productive dialogue. 


#### Do language models reproduce our moral biases? 
Since so much of human thought is expressed in text, it stands to reason that models trained on large amounts of text might learn something about human morality. This leads to a natural question: 

*Can large language models reproduce our moral biases?* 

The *Moral Mimicry* project looks at this question specifically in the context of the Moral Foundations Hypothesis, testing whether models like GPT-3 can simulate the moral biases of US conservatives and liberals [^1]. 

*If we prompt a language model to simulate a political liberal performing some moral reasoning task, does it use liberal moral foundations?* 

<!-- #### Yes, to some extent

<img class="img-fluid z-depth-1" src="{{ '/assets/img/moral_mimicry_rq2.png' | relative_url }}">
<div class="caption"> 
<strong>Figure.</strong>
</div>


#### ... and moreso in bigger models


<img class="img-fluid z-depth-1" src="{{ '/assets/img/moral_mimicry_rq6.png' | relative_url }}">
<div class="caption"> 
<strong>Figure.</strong>
</div> -->

#### Read More
For findings and more details about this work, please refer to the paper. A working draft is available here.
An earlier version of the work is also available on [ArXiv](https://arxiv.org/abs/2209.12106). An updated draft will be available on ArXiv in the coming weeks, after decisions for the [ACL Student Research Workshop]().

This work connects to a number of other papers investigating the capablility of Large Language Models to simulate humans. If this work is interesting to you, I would highly recommend reading the following papers:

* [Out of One, Many: Using Language Models to Simulate Human Samples](https://www.cambridge.org/core/journals/political-analysis/article/out-of-one-many-using-language-models-to-simulate-human-samples/035D7C8A55B237942FB6DBAD7CAA4E49) by Lisa P. Argyle, et. al.
* [Whose Opinions do Language Models Reflect?](https://arxiv.org/abs/2303.17548) by Shibani Santurkar, et. al.


#### Footnotes

[^1]: This choice was based on data availability - there are several human studies investigating the differences between these groups. In theory the methods could be applied to any other social groups, and I suspect that this will be a growing area of research in the coming years.