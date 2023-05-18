---
layout: blog_page
title: Moral Mimicry
description: Can large language models reproduce the moral biases of political groups?
img: /assets/img/pillars.jpg
importance: 1
toc: true
tools:  
- HuggingFace
- DeepSpeed
---

In the past decades, the United States has seen a rise in political polarization. Liberals and conservatives talk past each other, with common ground apparently getting smaller and smaller. What's behind this phenomenon? 

A theory from moral psychology offers one answer to this question: liberals and conservatives have different *moral foundations*. 

<img class="img-fluid z-depth-1" src="{{ '/assets/img/pillars.jpg' | relative_url }}" style="width:50%;margin:auto;display:inherit;">

## Moral Foundations Theory
Moral Foundations Theory (MFT) attempts to explain this variance. MFT is a theory of morality that argues that people's moral sensibilities draw on five themes, or "foundations". For those with a background in math or machine learning, you might think of the moral foundations as the principal components of moral reasoning. The *Moral Foundations Hypothesis* argues that the relative importance of these foundations varies across social groups, with liberals and conservatives in the US being an example. The "Care" foundation is more important to liberals in the United States than to conservatives, and conservatives value the "Authority" foundation more than liberals. In fact, this variance in moral biases is not just a US phenomenon, but is also observed in other countries. Human social groups tend to vary in the relative importance of certain moral themes, and this variation is reflected in their moral reasoning.

The Moral Foundations Hypothesis offers an explanation for why people of differing social groups might talk past each other when it comes to moral issues. It also offers optimism - acknowledging and studying this difference could help to bridge ideological gaps and encourage productive dialogue. 

## How do language models use moral language? 
To evaluate whether LLMs use moral language appropriately, I introduced two criteria:

**Criterion A** proposes that LLMs satisfy some level of human-like foundation word use if they use foundation words that are situationally appropriate, meaning they should be more likely to express a particular foundation when prompted with a scenario where that foundation is salient.

**Criterion B** demands that LLMs not deviate from human foundation use beyond a certain level of variation that is expected among humans.

Our results showed that LLMs do satisfy Criterion A, as they increased the use of foundation-associated words appropriate to the ground truth foundation label across all five foundations. 

However, we found that the difference between the language model and human foundation use was generally greater than the difference between individual humans, indicating that LLMs do not fully meet Criterion B.


## Do language models reproduce our moral biases? 
Since so much of human thought is expressed in text, it stands to reason that models trained on large amounts of text might learn something about human morality. This leads to a natural question: 

*Can large language models reproduce our moral biases?* 

The *Moral Mimicry* project looks at this question specifically in the context of the Moral Foundations Hypothesis, testing whether models like GPT-3 can simulate the moral biases of US conservatives and liberals [^1]. 

*If we prompt a language model to simulate a political liberal performing some moral reasoning task, does it use liberal moral foundations?* 

<img class="img-fluid z-depth-1" src="{{ '/assets/img/moral_mimicry_rq2.png' | relative_url }}">
<div class="caption"> 
</div>

Results indicate that models from the GPT-3, GPT-3.5 and OPT model families are more likely to use the binding foundations when prompted with conservative political identity, and are more likely to use the individualizing foundations when prompted with liberal political identity. Emphasis on individual foundations in each category differs by model family. OPT-30B shows larger effect sizes for Fairness/Cheating than Care/Harm and larger effect sizes for Sanctity/Degradation vs.~Authority/Subversion, while GPT-3.5 demonstrates the opposite. I suspect that this may be due to differences in training data and/or training practices between the model families. This opens an interesting question of how to influence the moral mimicry capabilities that emerge during training, via dataset curation or other methods.  

## How does LLM foundation use change with model size? 

<img class="img-fluid z-depth-1" src="{{ '/assets/img/moral_mimicry_rq6.png' | relative_url }}">
<div class="caption"> 
</div> 

The results from show some relationship between moral mimicry and model size. Effect sizes tend to increase with parameter count in the OPT family, and less so in the GPT-3 family. 

Both 175B-parameter GPT-3.5 models show relatively strong moral mimicry capabilities, moreso than the 175B GPT-3 model text-davinci-001. This suggests that parameter count is not the only factor leading to moral mimicry. The GPT-3.5 models were trained with additional supervised fine-tuning not applied to the GPT-3 family, and used text and code pre-training rather than text alone. 


## Read the Paper
[Latest Draft]({{ '/assets/pdf/moral_mimicry_Apr_14_2023.pdf' | relative_url }}) 

An earlier version of the work is also available on [ArXiv](https://arxiv.org/abs/2209.12106). 

## Related Work
This work connects to a number of other papers investigating the capablility of Large Language Models to simulate humans. If this work is interesting to you, I would highly recommend reading the following papers:

* [Out of One, Many: Using Language Models to Simulate Human Samples](https://www.cambridge.org/core/journals/political-analysis/article/out-of-one-many-using-language-models-to-simulate-human-samples/035D7C8A55B237942FB6DBAD7CAA4E49) by Lisa P. Argyle, et. al.
* [Whose Opinions do Language Models Reflect?](https://arxiv.org/abs/2303.17548) by Shibani Santurkar, et. al.


#### Footnotes

[^1]: This choice was based on data availability - there are several human studies investigating the differences between these groups. In theory the methods could be applied to any other social groups, and I suspect that this will be a growing area of research in the coming years.