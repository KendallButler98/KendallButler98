# Kendall J. Butler

## Contact
I look forward to hearing from you!

- Email: [![Email](https://img.shields.io/badge/Email-red?logo=gmail&logoColor=white)](mailto:kendall.jon.butler@gmail.com)
- LinkedIn: [![LinkedIn](https://img.shields.io/badge/LinkedIn-blue?logo=linkedin&logoColor=white)](https://linkedin.com/in/kendall-butler-b4ba63157/)
- GitHub: [https://github.com/KendallButler98](https://github.com/KendallButler98)

## About

I am a PhD in Physics transitioning into data science, excited to apply my skills to deliver data-driven solutions and actionable insights. With my doctorate, I offer persistence, adaptability, and tested problem-solving ability 

**(Note: Portfolio projects, descriptions of graduate research, and publications are in the "Portfolio" and "Research" sections below.)**

## Portfolio Projects (continuously updating)

### Project 1

### Project 2 - Machine Learning: Sub-Projects Demonstrating Regression, Clustering, Unsupervised Learning and Classification (in-progress)

#### 2.1: Regression analysis of Yelp Review Data

#### 2.2: 

#### 2.3:

#### 2.4: 



## Research

### 1 - Neuronal traveling waves form preferred pathways using synaptic plasticity - Dissertation Thesis

This is the dissertation thesis I wrote and defended in order to earn my PhD from Drexel University. It includes all meaningful projects I completed during my time with the Computational Biophysics group. To complete my research, I used Python heavily, leveraging the BRIAN neural simulator to study traveling waves through networks of neurons. With our model networks, I demonstrated pathway formation when neuronal traveling waves are paired with plasticity in the form of Spike-Timing Dependent Plasticity. I also investigated dynamical changes as a result of changes in specific network parameters as well as through changes in delay times using delay-STDP, which we introduce as an adjustment of the regular STDP rule. 

In the appendix of this thesis, I detail additional results related to those two major projects, recreate work done in mentorship of a senior undergraduate student, and describe additional side projects completed during my years at Drexel University. One such project is a machine learning framework I developed using our traveling wave model, classified inputs (from the fashion-MNIST dataset), and an output network trained for classification using Surrogate Gradient Learning (SGL) and Back-Propagation Through-Time (BPTT) from the outputs of our network. 

**Link to open-access dissertation:** [https://researchdiscovery.drexel.edu/esploro/outputs/doctoral/Pathway-formation-and-dynamical-transitions-by/991022057536604721](https://researchdiscovery.drexel.edu/esploro/outputs/doctoral/Pathway-formation-and-dynamical-transitions-by/991022057536604721)

#### Breakdown of Thesis parts/projects

1. **Chapter 3 - The formation of pathways** (demonstrates pathway formation by traveling waves with the addition of plasticity in the form of STDP) - this is the same as project 1 above.
2. **Chapter 4 - Delay Plasticity (breakdown below)**
   a. A phase space is delineated using various metrics connected to synaptic delays and the rate of neuron membrane recovery
   b. An adjustment of STDP to changes in synaptic delays (delay-STDP), tested for multiple types
   c. Demonstration of increased pathway formation with the combination of STDP and bidirectional delay-STDP
3. **Appendix A** - Supplementary Information for Chapter 3
4. **Appendix B** - Recreation of a project done alongside a student I mentored in the 2023-2024 academic year
5. **Appendix C** - Supplementary Information for Chapter 4
6. **Appendix D** - Additional projects, including additional neuron types, synapse models, surrogate gradient learning (BPTT for spiking signals) using PyTorch, and the effects of network damage on wave propagation
7. **Appendix E** - Visualization of the effects that adjusting various network parameters has on wave propagation

### 2 - Neuronal traveling waves form preferred pathways using synaptic plasticity - Published in the Journal of Computational Neuroscience

**Link to open-access paper:** [https://link.springer.com/article/10.1007/s10827-024-00890-2](https://link.springer.com/article/10.1007/s10827-024-00890-2)

**Repository:** [https://github.com/kjb-research/JCN-Traveling-Wave-Pathways](https://github.com/kjb-research/JCN-Traveling-Wave-Pathways)

This paper simulated traveling waves through a thin (3-layer) sheet of neurons using various mechanisms of input stimulation. The neurons in these simulations (like real neurons) communicated via synapses. Put simply, each neuron has many input synapses from other neurons. When enough stimulation is received from those synapses, the neuron fires and it sends its own signal. When that signal reaches its synapses, stimulation is input into those neurons in turn. We include synaptic plasticity (the ability of synapses to change with activity) in the form of Spike-Timing Dependent Plasticity (STDP), where if the neuron sending a signal spikes before the neuron receiving it, that synapse is strengthened! If the opposite occurs (a negative correlation) that synapse is weakened instead. With the addition of STDP to a network with traveling waves, directional pathways were formed over time in all cases, which we visualized using vector fields of average weight changes for each region.

### 3 - Poster for the 2024 Biophysical Society Conference - "Formation of Synaptic Pathways with Neuronal Traveling Waves"

**PDF of Poster:** [https://github.com/KendallButler98/research_files/blob/main/Poster_2024.pdf](https://github.com/KendallButler98/research_files/blob/main/Poster_2024.pdf)

### 4 - Honors Thesis at the University of Maine - "Investigating the Stability of Observed Low Semi-major Axis Exoplanetary Systems With Hypothetical Outer Planets Using The Program Mercury6"

This is the honors thesis I completed through research my Senior year at the University of Maine, for which I earned highest honors. This project included simulation of three observed planetary systems using the program Mercury6. Each of these simulations included an additional outer planet with varying parameters and simple analysis using a Python script. See link below for the full text:

**Open-access honors thesis:** [https://digitalcommons.library.umaine.edu/honors/586/](https://digitalcommons.library.umaine.edu/honors/586/)



