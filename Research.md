---
title: Research
permalink: /Research/
---
### Interpreting Deep Learning for Regulatory Genomics 

<p align="justify"> 
	Deep learning is being applied rapidly in many areas of genomics, demonstrating improved performance over previous methods on benchmark datasets. Despite the promise of deep learning systems, it remains unclear whether improved predictions will translate to new biological discoveries because of their low interpretability, which has earned them a reputation as a black box. Understanding the reasons for a deep learning model’s prediction may reveal new biological insights not captured by previous methods. Our research develops methods to interpret deep learning models through <b>design principles</b>,  <b>interrogation methods</b>, and <b>robust training</b>.
</p>

<p align="justify"> 
	<b>Design principles</b> can help create an inductive bias that guides parameters to learn human-interpretable, biologically-meaningful representations (see Figure below). For instance, we have previously shown that the downsampling intermediate representations in convolutional neural networks (CNNs) directly affects the extent that biological features, such as sequence motifs, are learned in each layer <a href="https://www.biorxiv.org/content/10.1101/362756v3">[1]</a>. More recently, we demonstrated that highly divergent activation functions, such as an exponential, encourages CNNs to learn more interpretable representations <a href="https://www.biorxiv.org/content/10.1101/650804v1.abstract">[2]</a>.
</p>


 <img class='img-responsive center-block' src="/images/research/representations.png" width="80%" height="80%"/>
<p align="justify"> 
	<sub>Distributed representations recognize features, in this case a grandma and a cat, by integrating partial feature representations from many different neurons. On the other hand, local representations only require a single neuron, so-called grandma neurons, to recognize whole feature representations. In genomics, this corresponds to learning whole sequence motifs (local representations) or partial sequence motifs (distributed representations), which are difficult to interpret. 
	</sub>
</p>

<p align="justify"> 
	We are also interested in developing <b> interrogation methods </b> to access representations learned by a deep black box model. Recently, we developed an interrogation method that combines causal inference with attribution methods. Our causal attribution framework was instrumental to show that ResidualBind – our state-of-the-art deep learning model that is trained to predict sequence specificities of RNA-binding proteins – learns features not considered by previous methods <a href="https://www.biorxiv.org/content/10.1101/418459v1.abstract">[3]</a>. We are expanding this methodology to uncover higher-order interactions of cis-regulatory elements, i.e. regulatory codes, from high-throughput sequencing datasets and validating our predictions experimentally with collaborators. 
</p>

<p align="justify"> 
<b>Robust training methods</b> – adversarial training, Gaussian smoothing, and regularization – have been developed to make CNNs more robust to adversarial examples, which are specially crafted perturbations added to data such that they are imperceptible to humans but can easily trick a state-of-the-art classifier (see figure below). There is growing evidence that adversarial training, in particular, also promotes learning more robust features. We have observed that CNNs that learn robust features – through design principles and robust training methods – are generally more interpretable <a href="https://www.biorxiv.org/content/10.1101/657437v1.abstract">[4]</a>. We are interested in establishing robust training standards for genomics and more broadly understanding the properties that make networks more robust.
</p>

  <img class='img-responsive center-block' src="/images/research/piggie.png" width="70%" height="70%"/>
<p align="justify"> 
	<sub>On the left, an image of a pig is correctly classified by a state-of-the-art convolutional neural network. After a small perturbation is added to every pixel of the image, the new image (on the right) is visually very similar to the original image, but now the CNN predicts that it is an airliner.
	</sub>
</p>

### Scoring Mutations in Proteins with Deep Generative Models

<p align="justify"> 
	Sequence evolution can inform probabilistic models of a protein's functional contstraints. 
	From a multiple sequence alignment of homologous sequences (Fig. A), satistical models have been developed to capture site-independence conservations and evolutionarily-coupled positions. These models can then be repurposed to score mutations in protein sequences, predict protein contacts (Fig. B), perform homology search, and design proteins. There has been growing interest in replacing traditional models – which include Position Sensitive Scoring Matrix (PSSM), Markov Random Fields (MRFs) and Multivariate Gaussians (MGs) – with <b>deep generative models</b> <a href="https://arxiv.org/abs/1906.02598">[5]</a> – which include variational autoencoders (VAEs), seq2seq models based on recurrent neural networks, generative adversarial networks (GANs), and transformer networks (Fig. C). We are interested in interpreting this promising class of models to understand what they are capable of learning. Our goal is to identify the deleteriousness of mutations in protein sequences, which can help to prioritize disease-associated genomic variants in coding regions. 
</p>

  <img class='img-responsive center-block' src="/images/research/protein.png" width="70%" height="70%"/>
	<sub>(<b>A</b>) Multiple sequence alignment for homologous protein sequences. Positions with the same amino acid are conserved (green column). Positions that are in structural contact can exhibit covariation (coupled columns covarying blue and yellow). (<b>B</b>) Contact map that shows positions of protein from N to C terminus. Grey dots represent known contacts from x-ray crystallography, while the blue dots represent covariation predictions made by a MRF. (<b>C</b>) Graphical representation of statistical models for sequence analysis. 
	</sub>
<br>
<br>
<br>
<br>
<br>
<br>



















