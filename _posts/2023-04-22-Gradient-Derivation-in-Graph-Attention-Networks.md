---
layout: post
---
Graph Attention Networks (GATs) have recently emerged as a promising approach for learning on graph-structured data. However, the performance achieved by these networks has been found to be varying across different datasets, and the reasons for this inconsistency remain an unanswered question in research. Gaining insights into the training dynamics of these statistically learning models is an important step towards improving the effectiveness of learning on graph-structured data. In particular, understanding the backward path, or backpropagation, is essential for comprehending the training behavior of a neural network. Backpropagation is a crucial process for the network to learn and enhance its performance by iteratively modifying its weights. Hence, by understanding the backward path, knowledge about how and why certain weights are being adjusted can be acquired. This can help in debugging issues during the training process.

### Gradients in GATv2
A comprehensive derivation of the gradients for the trainable model parameters of GATv2 [1]<d-cite key="GATv2"></d-cite>, a prominently used GAT realization, is published at: 
<a href="https://arxiv.org/abs/2304.10939">https://arxiv.org/abs/2304.10939</a>.

### Implementation of GAT+
The gradient derivations supplement the efforts of [2]<d-cite key="neumeier2023"></d-cite>, where limitations and potential pitfalls of GATv2 are investigated. To overcome the identified limitations the work proposes architectural adaptions to the prominently used GATv2 which have shown to improve training robustness and performance. The official implementation of the introduced architecture (GAT+) is publicly available [here](https://github.com/MB-Team-THI/sparse-graph-attention-optimization). The implementation is based on the PyTorch Geometric library, enabling users to effortlessly integrate the proposed architecture.


<h3 id="references">References</h3><ol id="references-list" class="references">
  <li id="GATv2">
    <span class="title">How Attentive are Graph Attention Networks?</span> 
    <br>Shaked Brody, Uri Alon, Eran Yahav, 2022. International Conference on Learning Representations (ICLR).
 <a href="https://openreview.net/forum?id=F72ximsx7C1" style="text-decoration:inherit;">https://openreview.net/forum?id=F72ximsx7C1</a>
  </li><li id="neumeier2023"><span class="title">Optimization and Interpretability of Graph Attention Networks for Small Sparse Graph Structures in Automotive Applications</span> 
  <br>M. Neumeier, A. Tollkuhn, S. Dorn, M. Botsch, and W. Utschick, 2023. IEEE Intelligent Vehicles Symposium (IV). 

{% comment %}
Might you have an include in your theme? Why not try it here!
{% include my-themes-great-include.html %}
{% endcomment %}

