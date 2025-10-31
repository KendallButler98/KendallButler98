# Kendall J. Butler

**(Descriptions of graduate research, and publications are in the "Research" section, with minor additional computational analyses in the "Data Science Projects" sections below.)**

## Contact
I look forward to hearing from you!

- Email: [![Email](https://img.shields.io/badge/Email-red?logo=gmail&logoColor=white)](mailto:kendall.jon.butler@gmail.com)
- LinkedIn: [![LinkedIn](https://img.shields.io/badge/LinkedIn-blue?logo=linkedin&logoColor=white)](https://linkedin.com/in/kendall-butler-b4ba63157/)

## About

I am a computational biophysicist with a Ph.D. from Drexel University, focused on modeling complex neuronal systems and analyzing emergent dynamics in large-scale simulations.

**Education:**
- **PhD Physics**, Drexel University (2025)
- **MS Physics**, Drexel University (2022)
- **BS Physics**, University of Maine (2020, Highest Honors)

In 2020, I began the physics PhD program at Drexel University. The first research group I joined at Drexel was the PROSPECT collaboration, for which I used C++ to analyze Bismuth-Polonium background radiation for their neutrino detector. In 2021, I began work with the Computational Biophysics group, simulating traveling waves in spiking neural networks in MATLAB. After qualifying for PhD candidacy, I translated this code into Python in order to have a more adaptable and flexible framework to continue my research with. My dissertation research focused on applying learning rules, dynamical analysis and even machine learning techniques to traveling waves in a simulated model capable of reproducing neuronal traveling waves, all with the goal of elucidating possible functions of this phenomenon in the brain.

**Research Accomplishments:**
- Designed and analyzed large neuronal networks (30,000 neurons) to investigate the purpose of traveling waves in the brain
- Revealed, quantified and visualized pathway formation as a result of the co-incidence of traveling waves and Spike-Timing Dependent Plasticity (STDP)
- Elucidated a dynamical phase-space measuring wave continuity and curl in connection to synaptic delay times and membrane potential recovery
- Modified the classical excitatory STDP rule to adjust synaptic delays, observing transitions in wave dynamics as delays are modulated
- Developed visualization techniques and novel metrics for analysis of our simulation output data
- Presented a poster at the 2024 Biophysical Society Conference
- Published in the Journal of Computational Neuroscience

**Computational Development:**
- Translated legacy MATLAB code into a Python-based framework
- Applied data analysis, modeling, and simulation techniques in Python
- Developed a PyTorch-based machine learning framework for the classification of inputs using our network model

**Mentorship & Teaching:**
- Taught Python programming and simulation to first-year physics majors
- Supervised a team of "Physics Fellows"
- Mentored a senior undergraduate on a capstone project using linear regression to measure wave speed

Overall, my experience as a computational neuroscientist and physicist demonstrates my capabilities as a researcher, mentor, and teacher, and I am eager to apply and further develop these skills in a postdoctoral or research-oriented role.

## Research

### 1 - Pathway formation and Dynamical Transitions by Neuronal Traveling Waves with Plasticity - Dissertation Thesis (June 2025)

This is the dissertation thesis I wrote and defended in order to earn my PhD from Drexel University. It includes all meaningful projects I completed during my time with the Computational Biophysics group. To complete my research, I used Python heavily, leveraging the BRIAN neural simulator to study traveling waves through networks of neurons. With our model networks, I demonstrated pathway formation when neuronal traveling waves are co-incident with plasticity in the form of Spike-Timing Dependent Plasticity. I also investigated dynamical changes as a result of changes in specific network parameters as well as through changes in delay times using delay-STDP, which I introduce as an adjustment of the regular STDP rule. 

In the appendix of this thesis, I detail additional results related to those two major projects, recreate work done in mentorship of a senior undergraduate student, and describe additional side projects completed during my years at Drexel University. One such project is a machine learning framework I developed using our traveling wave model, classified inputs (from the fashion-MNIST dataset), and an output network trained for classification using Surrogate Gradient Learning (SGL) and Back-Propagation Through-Time (BPTT) from the outputs of our network. 

**Link to open-access dissertation:** [Dissertation](https://researchdiscovery.drexel.edu/esploro/outputs/doctoral/Pathway-formation-and-dynamical-transitions-by/991022057536604721)

#### Breakdown of Thesis parts/projects

1. **Chapter 3 - The formation of pathways** (demonstrates pathway formation by traveling waves with the addition of plasticity in the form of STDP) - this is the same as the published paper (project 2) below.
2. **Chapter 4 - Delay Plasticity**
   a. A phase space is delineated using various metrics connected to synaptic delays and the rate of neuron membrane recovery
   b. An adjustment of STDP to changes in synaptic delays (delay-STDP), tested for multiple types
   c. Demonstration of increased pathway formation with the combination of STDP and bidirectional delay-STDP
3. **Appendix A** - Supplementary Information for Chapter 3
4. **Appendix B** - Recreation of a project done alongside a student I mentored in the 2023-2024 academic year
5. **Appendix C** - Supplementary Information for Chapter 4
6. **Appendix D** - Additional projects, including additional neuron types, synapse models, surrogate gradient learning (BPTT for spiking signals) using PyTorch, and the effects of network damage on wave propagation
7. **Appendix E** - Visualization of the effects that adjusting various network parameters has on wave propagation

### 2 - Neuronal traveling waves form preferred pathways using synaptic plasticity - Published in the Journal of Computational Neuroscience (December 2024)

**Link to open-access paper:** [Butler, K., Cruz, L., Journal of Computational Neuroscience, 2024](https://link.springer.com/article/10.1007/s10827-024-00890-2)

**Repository:** [J. of Comp. Neurosci. Reproducibility Code](https://github.com/kjb-research/JCN-Traveling-Wave-Pathways)

This paper simulated traveling waves through a thin (3-layer) sheet of neurons using various mechanisms of input stimulation. The neurons in these simulations (like real neurons) communicated via synapses. Put simply, each neuron has many input synapses from other neurons. When enough stimulation is received from those synapses, the neuron fires and it sends its own signal. When that signal reaches its synapses, stimulation is input into those neurons in turn. We include synaptic plasticity (the ability of synapses to change with activity) in the form of Spike-Timing Dependent Plasticity (STDP), where if the neuron sending a signal spikes before the neuron receiving it, that synapse is strengthened! If the opposite occurs (a negative correlation) that synapse is weakened instead. With the addition of STDP to a network with traveling waves, directional pathways were formed over time in all cases, which we visualized using vector fields of average weight changes for each region.

### 3 - Dynamical transitions in traveling waves by synaptic delay plasticity - Manuscript in preparation, to be submitted early 2026

This project, as outlined in chapter 4 of my dissertation, investigates dynamical transitions in our traveling wave networks. First, I reveal a phase space, quantifying wave continuity and propagation curl in relation to both membrane potential recovery and the scale of distance-dependent delay times. We found that wave longevity transitioned from transient to continuous wave propagation as both delay times and membrane recovery rates were increased, while the curl of propagation was significantly effected only by synaptic delays. We extended these ideas in connection to plasticity by adjusting STDP into delay-STDP in three forms (increasing-only, decreasing-only, bidirectional delay changes). With this model we observed real-time dynamical transitions that could help interpret the possible effects of real delay plasticity, which we do not yet have a full understanding of.

### 4 - Poster for the 2024 Biophysical Society Conference - "Formation of Synaptic Pathways with Neuronal Traveling Waves" (February 2024)

**PDF of Poster:** [Biophysical Society Poster](https://github.com/KendallButler98/research_files/blob/main/Poster_2024.pdf)

### 5 - Honors Thesis at the University of Maine - "Investigating the Stability of Observed Low Semi-major Axis Exoplanetary Systems With Hypothetical Outer Planets Using The Program Mercury6" (May 2020)

This is the honors thesis I completed through research my Senior year at the University of Maine, for which I earned highest honors. This project included simulation of three observed planetary systems using the program Mercury6. Each of these simulations included an additional outer planet with varying parameters and simple analysis using a Python script. See link below for the full text:

**Open-access honors thesis:** [Undergraduate Honors Thesis](https://digitalcommons.library.umaine.edu/honors/586/)

## Data Science Projects

### Project 1: E-commerce Customer Analysis - Understanding Behavior and Identifying High-value Segments

**Repository:** [Segmentation & Clustering Project](https://github.com/KendallButler98/Ecommerce_Analysis/tree/main)

This project includes an analysis of the "Online Retail II UCI" dataset sourced from Kaggle: [https://www.kaggle.com/datasets/mashlyn/online-retail-ii-uci](https://www.kaggle.com/datasets/mashlyn/online-retail-ii-uci), which includes data on individual transactions from an Ecommerce company over two years of business. My analysis demonstrates fundamental concepts and methods in data science, including:
- data cleaning
- exploratory analysis
- customer segmentation using RFM analysis
- Unsupervised machine learning (Kmeans clustering)

### Project 2: Advising Restaurants on How to Improve Customer Reviews Using Multiple Linear Regression on Yelp Review Data

**Repository:** [Multiple Linear Regression Project](https://github.com/KendallButler98/yelp_regression/tree/main)

This project includes an analysis of a subset of the [Yelp Open Dataset](https://business.yelp.com/data/resources/open-dataset/) provided by codecademy for academic purposes. My analysis demonstrates the following skills:
- data cleaning
- feature selection
- multiple linear regression
- model evaluation



