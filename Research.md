---
title: Research
permalink: /Research/
---
The <b>Koo Laboratory</b> studies sequence-function relationships with interpretable deep intelligent systems. We are interested in uncovering  cis-regulatory elements and their interactions for gene expression, RNA-protein interactions, and protein structure. Our goal is to elucidate the functional impact of genomic variants, which can provide insights into mutations associated with complex diseases, including cancer.
<br>

### Interpreting Deep Learning for Regulatory Genomics 

Deep learning is being applied rapidly in many areas of genomics, demonstrating improved performance over previous methods on benchmark datasets. Despite the promise of deep learning systems, it remains unclear whether improved predictions will translate to new biological discoveries because of their low interpretability, which has earned them a reputation as a black box. Understanding the reasons for a deep learning model’s prediction may reveal new biological insights not captured by previous methods. Our research develops methods to interpret deep learning models through design principles and interrogation methods.

<b>Design principles </b>, which include architecture choices and the incorporation of priors, can create an inductive bias that guides parameters to learn human-interpretable, biologically-meaningful representations. For instance, we have previously shown that the downsampling intermediate representations in convolutional neural networks (CNNs) directly affects the extent biological features, such as sequence motifs, are learned in each layer <a href="https://www.biorxiv.org/content/10.1101/362756v3">[1]</a>. More recently, we demonstrate that highly divergent activation functions, such as an exponential, encourages CNNs to learn more interpretable representations <a href="https://www.biorxiv.org/content/10.1101/650804v1.abstract">[2]</a>.
<br>
<br>


 <img class='img-responsive center-block' src="/images/research/representations.png" width="80%" height="80%"/>
<sub>Distributed representations use many neurons to contribute to the recognition of a feature, in this case a grandma and a cat.  Local representations are when a single neuron recognizes the entire feature, not requiring collaboration with any other neurons. In genomics, this corresponds to learning whole sequence motifs (local representations) or partial sequence motifs (distributed representations), which are difficult to interpret. 
</sub>
<br>
<br>

We are also interested in developing <b> interrogation methods </b> to access representations learned by a deep black box model. Recently, we developed an interrogation method that combines causal inference with attribution methods <a href="https://www.biorxiv.org/content/10.1101/418459v1.abstract">[3]</a>. Our causal attribution framework was instrumental to show that ResidualBind – our state-of-the-art deep learning model that is trained to predict sequence specificities of RNA-binding proteins – learns features not considered by previous methods. We are expanding this methodology to uncover higher-order interactions of cis-regulatory elements, i.e. regulatory codes, from high-throughput sequencing datasets and validating our predictions experimentally with collaborators. 
<br>

### Improving Interpretability with Adversarial Training 

For classification tasks, CNNs have been shown to be susceptible to specially crafted perturbations which alter their predictions confidently to the wrong class (see figure below). Much research has been focused on characterizing a networks susceptibility to these adversarial examples. Robust training methods -- adversarial training, Gaussian smoothing, and regularization -- have been developed to make CNNs more robust to adversaries, but they have also been shown to learn more robust features. We have observed that CNNs that learn robust features -- through design principles and robust training methods -- are more interpretable with gradient-based saliency methods <a href="https://www.biorxiv.org/content/10.1101/657437v1.abstract">[4]</a>. We are interested in exploring how robust training methods promote an inductive bias towards a biologically-meaningful parameter space and establishing robust training standards for genomic sequences. 


  <img class='img-responsive center-block' src="/images/research/piggie.png" width="70%" height="70%"/>
<sub>On the left, an image of a pig is correctly classified by a state-of-the-art convolutional neural network. After A small perturbation is added to the image at every pixel to yield an image on the right that is visually very similar to the original image, but now the CNN predicts that it is an airliner.
</sub>
<br>
<br>

### Scoring Mutations in Proteins with Deep Generative Models

Since evolution samples functional protein sequences, statistical models can be trained to learn functional sites -- site-independence conservations (1-body interactions) and evolutionarily coupled positions (2-body interactions) -- from a multiple sequence alignment of homologous sequences. These models can then be utilized to score mutations in protein sequences, predict protein contacts, perform homology search, and design proteins. Recently, there has been growing interest in replacing more traditional models -- which include Position Sensitive Scoring Matrix (PSSM), Markov Random Fields (MRFs) and Multivariate Gaussians (MGs) -- with <b>deep generative models</b> <a href="https://arxiv.org/abs/1906.02598">[5]</a> -- which include variational autoencoders (VAEs), seq2seq models based on recurrent neural networks, generative adversarial networks (GANs), and transformer networks. Our group is interested in interpreting these promising class of models to understand what they are capable of learning. Our goal is to explore the utility of these class of models to inform the deleteriousness of mutations in protein sequences, which can help to prioritize disease-associated genomic variants in coding regions. 
<br>
<br>

  <img class='img-responsive center-block' src="/images/research/protein.png" width="80%" height="80%"/>

<br>
<br>
<br>
<br>
<br>
<br>



















