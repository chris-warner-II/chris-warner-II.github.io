---
title: "1. Coupled oscillator model for image segmentation"
excerpt: "<img src='/images/img_seg_model.png' width='500' height='400'/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <img src='/images/cartoonization.png' width='300' height='200'/> <br/> Inspired by neuroscience and the retina, we pioneered a model that performs image segmentation by grouping together nearby image regions with similar features in phase space, resulting in a cartoonization of the image. The model simulates phase relaxation in a system of coupled Kuramoto oscillators with the strength of interaction defined by the Topographic Modularity between regions in the image. We demonstrate that this method outperforms other graph theoretic network construction methods as well as spectral Eigen-based methods for community detection by evaluating performance on the Berkeley Image Segmentation Dataset (BSDS)."
collection: portfolio
---

<img src='/images/img_seg_model.png' align='center' width='700' height='550'/> 
<br/> 
Synchrony in periodic retinal spike trains could convey contextual information of the visual input, which is extracted by computations in the retinal network. To explore this hypothesis, we propose a computational model for image segmentation consisting of a Kuramoto model of coupled oscillators whose phases model the timing of individual retinal spikes. Phase couplings between oscillators are shaped by the stimulus structure, causing cells to synchronize if the local contrast in their receptive fields is similar. In essence, relaxation in the oscillator network solves a graph clustering problem with the graph representing feature similarity between different points in the image. The resulting spike trains multiplex two types of information, local contrast in individual spike rates, and image segments in sets of neurons that fire nearly synchronously.

<img src='/images/cartoonization.png' align='right' width='300' height='200' padding: 5px 5px 5px 5px;/> Qualitatively, the phase map after relaxation results in a cartoonization of the original image, smoothing away texture within segments while keeping segment boundaries crisp.

<img src='/images/SegAssessPipeline.png' align='left' width='400' height='300' padding: 5px 5px 5px 5px;/> We measured the model's performance and compared it to other methods with the Berkeley Image Segmentation Data Set (BSDS). First, network couplings are computed from image similarity and proximity between two locations. Next, after being initialized by pixel intensity value, phase relaxes through the interactions in the network. Binary boundaries are constructed by thresholding the phase map and Precision, Recall and F-measure metrics are computed by comparing the boundaries to human annotated segment boundaries. 

