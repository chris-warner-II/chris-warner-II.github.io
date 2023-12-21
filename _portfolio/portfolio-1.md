---
title: "1. Coupled oscillator model for image segmentation"
excerpt: "<img src='/images/img_seg_model.png' width='550' height='400'/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <img src='/images/cartoonization.png' width='350' height='200'/> <br/> Inspired by neuroscience and the retina, we pioneered a model that performs image segmentation by grouping together nearby image regions with similar features in phase space, resulting in a cartoonization of the image. The model simulates phase relaxation in a system of coupled Kuramoto oscillators with the strength of interaction defined by the Topographic Modularity between regions in the image. We demonstrate that this method outperforms other graph theoretic network construction methods as well as spectral Eigen-based methods for community detection by evaluating performance on the Berkeley Image Segmentation Dataset (BSDS)."
collection: portfolio
---

Synchrony in periodic retinal spike trains may convey contextual information about the visual input, which is extracted by computations in the retinal network. To explore this hypothesis, we propose a computational model for image segmentation consisting of a Kuramoto model of coupled oscillators whose phases model the timing of individual retinal spikes. Phase couplings between oscillators are shaped by the stimulus structure, causing cells to synchronize when the local contrast in their receptive fields is similar. In essence, relaxation in the oscillator network solves a graph clustering problem with the graph representing feature similarity between different points in the image. The resulting spike trains multiplex the two types of information, local contrast in individual spike rates, and image segments in sets of neurons that fire nearly synchronously. <br/> 
<img src='/images/img_seg_model.png' align='center' width='750' height='500'/>
<p style="text-align: center; font-size:11pt"><strong>fig. 1</strong> Figure caption here. </p>

Qualitatively, the phase map after relaxation provides a qualitative "cartoonization" of the original image, smoothing away texture within segments while keeping boundaries at the edges of objects crisp. This provides a rudimentary image segmentation that could feasibly occur within the hardware of and using what signals are available to the retina.  

<img src='/images/cartoonization.png' align='center' width='550' height='250'/> 
<p style="text-align: center; font-size:11pt"><strong>fig. 2</strong> Figure caption here. </p>

Here, topographic modularity vs Laplacian, Association and Modularity and Kuramoto vs spectral Eigen methods.



To assess the model's performance and compare it to other methods, we leverage the Berkeley Image Segmentation Data Set (BSDS), and develop a performance evaluation pipeline computing Precision, Recall and F-measure metrics between human annotations and boundaries discovered by the algorithm. 

<img src='/images/SegAssessPipeline.png' align='center' width='500' height='400'/> 
<p style="text-align: center; font-size:11pt"><strong>fig. 3</strong> Figure caption here. </p>

The F-measure metric demonstrates the improvement in boundary detection provided by the 2D Topographic Modularity method with Kuramoto relaxation over other methods.

<img src='/images/Fmax_img_seg.jpg' align='center' width='750' height='500'/>
<p style="text-align: center; font-size:11pt"><strong>fig. 4</strong> Figure caption here. </p>
