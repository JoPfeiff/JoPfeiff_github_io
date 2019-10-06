---
layout: post
title: What do Deep Networks like to Read?
---

Our paper [What do Deep Networks like to Read?](https://arxiv.org/abs/1909.04547) is available on arXiv!

Here, we uncover artifacts that are encoded in our models, by finetuning a pretrained autoencoder using gradients from a classifier with frozen weights. 

(1) We pre-train a Seq2Seq autoencoder to initially adequately reproduce the input text. (2) We pre-train different classification models for diverse tasks. (3) We fine-tune the weights of the autoencoder with the gradients of the classifier with fixed weights. 

This rephrases the original sentences and gives us a view into what deep networks like to read. We find differences in how CNNs, LSTMs and Deep Averaging Networks restructure the sentences. 

By flipping the labels from the gold class, we force the autoencoder to rephrase the sentence in away that the classifier predicts the „new“ label. This helps us identify if the model has possibly encoded artifacts of the data set.

*Abstract:*
Recent research towards understanding neural networks probes models in a top-down manner, but is only able to identify model tendencies that are known a priori. We propose Susceptibility Identification through Fine-Tuning (SIFT), a novel abstractive method that uncovers a model's preferences without imposing any prior. By fine-tuning an autoencoder with the gradients from a fixed classifier, we are able to extract propensities that characterize different kinds of classifiers in a bottom-up manner. We further leverage the SIFT architecture to rephrase sentences in order to predict the opposing class of the ground truth label, uncovering potential artifacts encoded in the fixed classification model. We evaluate our method on three diverse tasks with four different models. We contrast the propensities of the models as well as reproduce artifacts reported in the literature.

