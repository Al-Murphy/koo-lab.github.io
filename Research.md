---
title: Research
permalink: /Research/
---
### Interpretable Deep Learning for Regulatory Genomics 

<p align="justify"> 
	Deep learning is being applied rapidly in many areas of genomics, demonstrating promising performance across a wide variety of regulatory prediction tasks <a href="https://www.sciencedirect.com/science/article/pii/S2452310020300032">[1]</a>. Despite the promise of deep learning systems, it remains unclear whether improved predictions will translate into new biological discoveries because of their low interpretability, which has earned them a reputation as a black box. Understanding the reasons underlying a deep learning model’s prediction may reveal new biological insights not captured by previous methods. Our research develops methods to interpret deep learning models through <b>design principles</b>, <b>interrogation methods</b>, and <b>robust training</b>.
</p>

<p align="justify"> 
	<b>Design principles</b> can guide parameters to learn human-interpretable, biologically-meaningful representations with an inductive bias (Fig. 1). Towards this, we have previously shown that the downsampling intermediate representations in deep convolutional neural networks (CNNs), a popular modeling choice for genomics, directly affect the extent that biological features, such as sequence motifs, are learned in each layer <a href="https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1007560">[2]</a>. We have also demonstrated that highly divergent activation functions also encourage CNNs to learn more interpretable representations <a href="https://www.nature.com/articles/s42256-020-00291-x">[3]</a>. We are currently exploring how hybrid networks that build upon convolutional layers with attention mechanisms can be utilized to uncover complex motif interactions <a href="https://openreview.net/forum?id=ITOQhccyRsk">[4]</a>, the so-called cis-regulatory code.
</p>


 <img class='img-responsive center-block' src="/images/research/representations.png" width="80%" height="80%"/>
<p align="justify"> 
	<sub><b>Figure 1.</b> Distributed representations recognize features, in this case a grandma and a cat, by integrating partial feature representations from many different neurons. On the other hand, local representations only employ a single neuron, a so-called grandma neuron, to recognize whole feature representations. In genomics, this corresponds to learning whole sequence motifs (local representations) or partial sequence motifs (distributed representations), which are difficult to interpret. 
	</sub>
</p>

<p align="justify"> 
	We are also interested in developing <b> interrogation methods </b> to access representations learned by deep (black box) models. We developed an interrogation method that uncovers global feature importance with synthetic sequences. This framework was instrumental to show that ResidualBind – our state-of-the-art deep learning model that is trained to predict sequence specificities of RNA-binding proteins – learns features not considered by previous methods <a href="https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1008925">[5]</a>. We are expanding this methodology to uncover higher-order interactions of cis-regulatory elements, i.e. regulatory codes, from high-throughput sequencing datasets <a href="https://www.biorxiv.org/content/10.1101/2023.07.03.547592v1">[6]</a>. We have recently extended this method to computer vision, with the broader aim of understanding cancer prognosis from histology data.
</p>

<p align="justify"> 
<b>Robust training methods</b> – adversarial training, Gaussian smoothing, and regularization – have been developed to improve the robustness of deep learning to adversarial examples, which are specially crafted perturbations added to data such that they are imperceptible to humans but can easily trick a state-of-the-art classifier (Fig. 2). There is growing evidence that adversarial training also leads to more robust features. We have observed deep learning models that learn robust features through design principles and robust training methods are generally more interpretable with attribution methods <a href="https://genomebiology.biomedcentral.com/articles/10.1186/s13059-023-02941-w">[7]</a>, <a href="https://www.biorxiv.org/content/10.1101/657437v1.abstract">[8]</a>, <a href="https://openreview.net/forum?id=LGgo0wPM2MF">[9]</a>. We are interested in establishing robust training standards for genomics and, more broadly, understanding the properties that make deep learning more robust and trustworthy.
</p>

  <img class='img-responsive center-block' src="/images/research/piggie.png" width="70%" height="70%"/>
<p align="justify"> 
	<sub><b>Figure 2.</b> On the left, an image of a pig is correctly classified by a state-of-the-art neural network. After a small perturbation is added to every pixel of the image, the new image (on the right) is visually very similar to the original image, but now the neural network predicts it is an airliner.
	</sub>
</p>
<br>

### Language Models for Biological Sequences

<p align="justify"> 
	Multiple sequence alignments of proteins inform statistical models of evolutionary constraints linked to function (Fig. 3A), which include site-independent conservations and pairwise coevolutions. These models can then be repurposed to: score mutations in protein sequences, predict protein contacts (Fig. 3B), search for homologs, and design proteins. There has been growing interest in replacing traditional models – Position Specific Scoring Matrices (PSSMs), Markov Random Fields (MRFs), and Multivariate Gaussians (MGs) (see Fig. 3C) <a href="https://arxiv.org/abs/1906.02598">[8]</a> – with alignment-free <b>deep generative models</b> <a href="https://www.biorxiv.org/content/10.1101/2021.10.23.465204v1">[9]</a>  – variational autoencoders (VAEs) <a href="https://www.biorxiv.org/content/10.1101/2020.11.29.402875v1">[10]</a>  - and language models based on transformers, but tailored with biological priors <a href="https://www.biorxiv.org/content/10.1101/2020.12.21.423882v2">[11]</a>. We are interested in interpreting these promising class of models to understand how they build representations and how to harness them to push the boundaries of basic science and cancer biology.  
</p>

  <img class='img-responsive center-block' src="/images/research/protein.png" width="70%" height="70%"/>
	<sub><b>Figure 3.</b> (<b>A</b>) Multiple sequence alignment of homologous protein sequences. Positions with the same amino acid are conserved (green column). Positions that are in structural contact can exhibit covariation (coupled columns covarying blue and yellow). (<b>B</b>) Example contact map shows protein positions from N to C terminus. Grey dots represent known contacts from x-ray crystallography, while blue dots represent covariation predictions by an MRF. (<b>C</b>) Graphical representation of statistical models for sequence analysis. (Images courtesy of Sergey Ovchinnikov)
	</sub>
<br>
<br>
<br>
<br>
<br>
<br>



















