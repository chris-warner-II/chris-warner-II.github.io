---
title: "Vocal complexity of human speech (Postdoc Project)"
excerpt: "<img src='/images/TIMIT_waveform.png' width='500' height='400'> <img src='/images/TIMIT_spectrogram.png' width='400' height='300'> <br/> The goal of this project is to understand the hierarchical temporal complexity of auditory signals. ['Predictive information'](https://arxiv.org/abs/cond-mat/9902341) (PI) quantifies how much information about the future of a signal is contained in its past. We apply the PI framework to human speech in the TIMIT dataset to explore how acoustical and phonetic features contribute to the complexity of vocal signals. We also compare results from human speech to other animal vocalizations, like bird song. Toward this goal, we also build machine learning models to perform automatic speech recognition (asr) and phoneme classification based on spectrogram features."
collection: portfolio
---

Conversations about the analysis of poetic text in phoneme and syllable embedding space led to this collaboration with Dr. Kris Bouchard's [Neural Systems Data Science Laboratory](https://bouchardlab.lbl.gov). 'Predictive Information' (PI) is an information theoretic measure that quantifies how much the past of a signal predicts about the future of that signal. We use this framework to quantify and compare the vocal complexity of different individuals and across species. We explore PI for bird song and human speech. As it relates to spoken-word poetry, I expect a more complex rhythm and rhyme-scheme would yield higher values of PI since the signal's past contains more information about the signal's future. 

In order to compute PI, we first convert an audio signal into a spectrogram. Then, there are two parameters which directly go into the PI calculation, (d, T). The embedding dimension, d, compresses spectral information into a lower dimension than the number of frequency bins in the spectrogram. This work Leverages the [Compressed Predictive Information](https://arxiv.org/pdf/2203.02051) method and the underlying dimensionality reduction technique, [Dynamical Components Analysis](https://arxiv.org/abs/1905.09944). Exploring the effect d has on PI, we find that signals can be compressed spectrally without losing predictive power. The time parameter, T, controls how far back and forward into the past and future the algorithm looks to compute PI. It shift the focus from spectral complexity (when T=1) to temporal complexity (for T>1). Large T values are necessary to pull out rhythm and rhyme scheme in spoken word poetry. 

The algorithm becomes quite computationally expensive for large T values. We have explored speeding up the computation with efficient sparse matrix multiplication on GPUs using C++ libraries.

This project is still a work in progress, among other side projects at this moment. Some selected slides from project presentation are located [here](https://chris-warner-ii.github.io/files/Warner_VoxComplex.pdf).
