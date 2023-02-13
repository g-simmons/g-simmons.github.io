---
abstract: The dominant sequence transduction models are based on complex recurrent
  or convolutional neural networks that include an encoder and a decoder. The best
  performing models also connect the encoder and decoder through an attention mechanism.
  We propose a new simple network architecture, the Transformer, based solely on attention
  mechanisms, dispensing with recurrence and convolutions entirely. Experiments on
  two machine translation tasks show these models to be superior in quality while
  being more parallelizable and requiring significantly less time to train. Our model
  achieves 28.4 BLEU on the WMT 2014 Englishto-German translation task, improving
  over the existing best results, including ensembles, by over 2 BLEU. On the WMT
  2014 English-to-French translation task, our model establishes a new single-model
  state-of-the-art BLEU score of 41.8 after training for 3.5 days on eight GPUs, a
  small fraction of the training costs of the best models from the literature. We
  show that the Transformer generalizes well to other tasks by applying it successfully
  to English constituency parsing both with large and limited training data.
authors:
- Ashish Vaswani
- Google Brain
- Noam Shazeer
- Google Brain
- Niki Parmar
- Jakob Uszkoreit
- Llion Jones
- Aidan Gomez
- "\u0141ukasz Kaiser"
- Google Brain
- Illia Polosukhin
equations:
- /assets/papercast/attention-is-all-you-need/equations_0.png
- /assets/papercast/attention-is-all-you-need/equations_1.png
- /assets/papercast/attention-is-all-you-need/equations_2.png
- /assets/papercast/attention-is-all-you-need/equations_3.png
- /assets/papercast/attention-is-all-you-need/equations_4.png
- /assets/papercast/attention-is-all-you-need/equations_5.png
- /assets/papercast/attention-is-all-you-need/equations_6.png
- /assets/papercast/attention-is-all-you-need/equations_7.png
- /assets/papercast/attention-is-all-you-need/equations_8.png
- /assets/papercast/attention-is-all-you-need/equations_9.png
- /assets/papercast/attention-is-all-you-need/equations_10.png
figures:
- /assets/papercast/attention-is-all-you-need/figures_0.png
- /assets/papercast/attention-is-all-you-need/figures_3.png
- /assets/papercast/attention-is-all-you-need/figures_4.png
- /assets/papercast/attention-is-all-you-need/figures_5.png
- /assets/papercast/attention-is-all-you-need/figures_6.png
layout: papercast
mp3: /assets/papercast/attention-is-all-you-need/attention-is-all-you-need.mp3
slug: attention-is-all-you-need
title: Attention is all you need
vtt: /assets/papercast/attention-is-all-you-need/attention-is-all-you-need.vtt
---
