# Overview:-

## Natural Language Inference(NLI)

The goal of natural language inference (NLI), a widely-studied natural
language processing task, is to determine if one given statement
(a premise) semantically entails another given statement (a hypothesis).

## Zero Shot Learning(ZSL)

Zero-shot learning (ZSL) is a problem setup in machine learning, where
at test time, a learner observes samples from classes that were not
observed during training, and needs to predict the category they belong
to. This problem is widely studied in computer vision, natural language
processing and machine perception. Unlike standard generalization in
machine learning, where classifiers are expected to correctly classify
new samples to classes they have already observed during training, in
ZSL, no samples from the classes have been given during training the
classifier.

# Task to perform:-

In this particular notebook my task is to find the `label` or you could
say (a premise) semantically entails the `doc` or (a hypothesis), for practice
we feed different numbers of `labels` to the `classifier`, and in return it
gave the probabilities for each of the `label` specified... The second task
is to find the sentiment of the particular sentence in `doc`... It is also
done in both ways when the labels are mutually exclusive(default) and when its
not... At last time and `CPU` usage is also calculated for the `classifier`.

# Structure/ process:-

This uses a wrapper called `ktrain`. The `ZeroShotClassifier` from `text`
(a module available in ktrain) is used to perform the main task.

* First we initialize a `sample doc` that can be feed into the classifier.

* Second we initialize a `labels` that may or may be not entails the sentence/text in `sample doc`.

* At last the necessary parameter must be passed in `ZeroShotClassifier`.

> NOTE:- If the labels are to be treated as mutually-exclusive, we can set `multilabel=False`
