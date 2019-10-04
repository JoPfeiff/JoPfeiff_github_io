---
layout: post
title: Update - Best Paper Award at Repl4NLP
---

Our paper [Specializing Distributional Vectors of All Words for Lexical Entailment](https://www.aclweb.org/anthology/W19-4310.pdf) won the best paper award!

*Abstract:*
Semantic specialization methods fine-tune distributional word vectors using lexical knowledge from external resources (e.g., WordNet) to accentuate a particular relation between words. However, such post-processing methods suffer from limited coverage as they affect only vectors of words seen in the external resources. We present the first postprocessing method that specializes vectors of all vocabulary words – including those unseen in the resources – for the asymmetric relation of lexical entailment (LE) (i.e., hyponymyhypernymy relation). Leveraging a partially LE-specialized distributional space, our POSTLE (i.e., post-specialization for LE) model learns an explicit global specialization function, allowing for specialization of vectors of unseen words, as well as word vectors from other languages via cross-lingual transfer. We capture the function as a deep feedforward neural network: its objective re-scales vector norms to reflect the concept hierarchy while simultaneously attracting hyponymyhypernymy pairs to better reflect semantic similarity. An extended model variant augments the basic architecture with an adversarial discriminator. We demonstrate the usefulness and versatility of POSTLE models with different input distributional spaces in different scenarios (monolingual LE and zero-shot cross-lingual LE transfer) and tasks (binary and graded LE). We report consistent gains over state-of-the-art LE-specialization methods, and successfully LE-specialize word vectors for languages without any external lexical knowledge.

