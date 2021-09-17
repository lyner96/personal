---
layout: default
title: 'Self-supervised Learning'
date: 2021-09-15
tags: [technical]
comments: true
---
> Last update on 17 Sep 2021 

Wherever possible, you should aim to start your neural network training with a pre-trained model, and fine tune it. You really don’t want to be starting with random weights, because that’s means that you’re starting with a model that doesn’t know how to do anything at all! With pretraining, you can use 1000x less data than starting from scratch. So, what do you do if there are no pre-trained models in your domain? You should use a general-purpose pre-trained model, even if it is not in the domain of the problem that you’re working in. We would like something which works better but doesn’t will need a huge amount of data. The secret is “self-supervised learning”. [1]

Self-supervised learning (SSL) is one of the most promising ways to  approximate a form of common sense in AI systems. SSL obtains supervisory signals from the data itself, often leveraging the underlying structure in the data. The general technique of SSL is to predict any unobserved or hidden part (or property) of the input from any observed or unhidden part of the input. [2]

In self-supervised learning the task that we use for pretraining is known as the “pretext task”. The tasks that we then use for fine tuning are known as the “downstream tasks”. Once you have pretrained your model with a pretext task, you can move on to fine tuning. At this point, you should treat this as a transfer learning problem, and therefore you should be careful not to hurt your pretrained weights. Often, it turns out that you don’t need a particularly complex pretext task to get great results on your downstream task. Therefore, you could easily end up wasting time over engineering your pretext task. Note also that you can do multiple rounds of self-supervised pretraining and regular pretraining. For instance, you could use one of the above approaches for initial pretraining, and then do segmentation for additional pretraining, and then finally train your downstream task. [1]

Taken from:
1. [fast ai ~ SSL and CV](https://www.fast.ai/2020/01/13/self_supervised/)
2. [FAIR ~ Self-supervised learning: The dark matter of intelligence](https://ai.facebook.com/blog/self-supervised-learning-the-dark-matter-of-intelligence/)

---

Read more:

[Bootstrap Your Own Latent (BYOL)](../../subcontent/byol)