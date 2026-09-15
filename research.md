---
layout: my-page
title: Research
---

Over the course of my Bachelor's, Master's and Ph.D. I have had the opportunity to work on several short and long-term research projects on various topics in Physics through internships, research assistantships or thesis projects (please refer to my [LinkedIn](https://www.linkedin.com/in/anikhalder/) page for details). I have worked mainly on analytical and computational projects in the fields of laser optics, planetary and space science, geosciences, x-ray reflectometry, and of course, astrophysics. Please refer to my [Google Scholar](https://scholar.google.com/citations?user=HZm11dQAAAAJ&hl=en) profile for a full list of publications that I am involved in.

Here, I present some of my current research projects in weak lensing cosmology and galaxy evolution and their associated publications:

### pop-cosmos and galaxy populations

<img src="images/popcosmos_KiDS1000_colours_sSFR.png" alt="pop-cosmos KiDS-1000 image" style="float:left; padding-bottom:12px" />

[pop-cosmos](https://github.com/Cosmo-Pop/pop-cosmos) is a generative model for the evolving galaxy population, calibrated on deep multi-wavelength photometry from COSMOS2020. It provides a physically motivated prior over the galaxy population up to redshift *z* ≈ 6 in stellar population synthesis parameter space. Using this prior with an emulator for stellar population synthesis and GPU-accelerated sampling, we have inferred joint posteriors on the redshifts and physical properties (such as stellar mass and star-formation rate) of 4 million galaxies in the Kilo-Degree Survey (KiDS-1000). The image above shows their inferred colours against inferred redshift, shaded by specific star-formation rate (courtesy: *Halder et al. 2026*). This is the first principled Bayesian inference of galaxy properties for a wide-area weak lensing survey. We validated the redshifts against around 185,000 KiDS galaxies with DESI spectroscopic redshifts. The same galaxy population model also forward-models the KiDS-1000 redshift distributions directly, without spectroscopic reweighting. With these catalogues we can select galaxy samples by their physical properties rather than by colour proxies, which opens the way to weak lensing and multi-tracer analyses with better control of systematic effects such as intrinsic alignments.

**Halder**, Peiris, Thorp, Leistedt, Mortlock, Jagwani, Tudorache, Deger, Van den Bussche, Leja, Wright (2026)\
*pop-cosmos: Redshifts and physical properties of KiDS-1000 galaxies*\
[arXiv:2602.03930](https://arxiv.org/abs/2602.03930) &nbsp; [MNRAS](https://doi.org/10.1093/mnras/stag1590)

Leistedt, Peiris, **Halder**, Thorp, Mortlock, Loureiro, Alsing, Jagwani, Tudorache, Deger, Leja, Van den Bussche, Wright, Li, Kuijken, Hildebrandt (2026)\
*pop-cosmos: Forward modeling KiDS-1000 redshift distributions using realistic galaxy populations*\
[arXiv:2602.03935](https://arxiv.org/abs/2602.03935)

Thorp, Peiris, Jagwani, Deger, Alsing, Leistedt, Mortlock, **Halder**, Leja (2025)\
*pop-cosmos: Insights from generative modeling of a deep, infrared-selected galaxy population*\
[arXiv:2506.12122](https://arxiv.org/abs/2506.12122) &nbsp; [ApJ](https://doi.org/10.3847/1538-4357/ae0936)

&nbsp;

### The integrated 3-point correlation functions

<img src="images/6xi3PCFs_illustration_v4.png" alt="Integrated 3PCFs image" style="float:left; padding-bottom:12px" />

In this series of works we have developed a set of practical higher-order statistics called the *integrated 3-point correlation functions* which can be easily measured from galaxy imaging data alongside conventional 2-point statistical methods and has the potential to put tighter constraints on cosmological, galaxy bias as well as baryonic feedback parameters (see image above; courtesy: *Halder et al. 2023*). This statistic measures the *position-dependent* 2-point correlation functions of a field (e.g. 3 x 2-point galaxy-lensing correlations) inside a local 2D patch and correlates them with the 1-point average shear or galaxy density within the same patch. This correlation admits a very well-defined physical interpretation as the modulation of the small-scale 2PCFs by long-wavelength features of the field and in turn is sensitive to the higher-order squeezed bispectrum configurations (3-point function) of the field. Using semi-analytical methods based on perturbation theory for accurately modelling this statistic along with the inclusion of galaxy bias, intrinsic alignments, baryonic feedback effects as well as other nuisance parameters, we have extensively validated our models against N-body simulations and with state-of-the art machine learning neural networks developed fast inference pipelines for their application to galaxy survey data (which we are currently undertaking). We are also extending this to a simulation based inference framework.

Gebauer, **Halder**, Seitz, Anbajagane (2026)\
*𝚂𝙱𝚒𝟹𝙿𝙲𝙵: Simulation-based inference with the integrated 3PCF*\
[arXiv:2510.13805](https://arxiv.org/abs/2510.13805) &nbsp; [JCAP](https://doi.org/10.1088/1475-7516/2026/06/036)

**Halder**, Gong, Barreira, Friedrich, Seitz, Gruen (2023)\
*Beyond 3x2-point cosmology: the integrated shear and galaxy 3-point correlation functions*\
[arXiv:2305.17132](https://arxiv.org/abs/2305.17132) &nbsp; [JCAP](https://iopscience.iop.org/article/10.1088/1475-7516/2023/10/028)

Gong, **Halder**, Barreira, Seitz, Friedrich (2023)\
*Cosmology from the integrated shear 3-point correlation function: simulated likelihood analyses with machine-learning emulators*\
[arXiv:2304.01187](https://arxiv.org/abs/2304.01187) &nbsp; [JCAP](https://iopscience.iop.org/article/10.1088/1475-7516/2023/07/040)

**Halder**, Barreira (2022)\
*Response approach to the integrated shear 3-point correlation function: the impact of baryonic effects on small scales*\
[arXiv:2201.05607](https://arxiv.org/abs/2201.05607) &nbsp; [MNRAS](https://academic.oup.com/mnras/article-abstract/515/3/4639/6648837?redirectedFrom=fulltext&login=false)

**Halder**, Friedrich, Seitz, Varga (2021)\
*The integrated 3-point correlation function of cosmic shear*\
[arXiv:2102.10177](https://arxiv.org/abs/2102.10177) &nbsp; [MNRAS](https://academic.oup.com/mnras/article-abstract/506/2/2780/6309317?redirectedFrom=fulltext)

&nbsp;

### The PDF of cosmic density fluctuations

<img align="left" width="330" height="300" src="images/jointPDF.png" alt="Joint PDF image" style="float:left; padding-right:12px" />

Along with my collaborators I have worked on modelling the 1-point PDF of weak lensing convergence as well as the joint PDF of 3D matter and galaxy density fluctuations (see image on the left; courtesy: *Friedrich et al. 2022*). Conventional 2-point analysis tools would compress this joint PDF into just 3 quantities: the variance of matter density fluctuations, the variance of galaxy density fluctuations, and their cross-covariance. In this work, we developed a model for the full shape of the joint galaxy-matter PDF and extensively validated it using N-body simulations and mock Halo Occupation Distribution (HOD) galaxy catalogs. Studying the full shape of the 1-point PDF is another way to go beyond 2-point analyses and enables further insights into the nature of the cosmic web of structures, especially on cosmological as well as galaxy bias and stochasticity parameters. We are currently extending our modelling to perform a joint-PDF analysis using CMB lensing data from SPT and DESY3 lens galaxies. 

Friedrich, Castiblanco, **Halder**, Uhlemann (2026)\
*Bye binormal: analysing the joint PDF of galaxy density and weak lensing convergence*\
[arXiv:2507.16957](https://arxiv.org/abs/2507.16957) &nbsp; [MNRAS](https://academic.oup.com/mnras/article/545/4/staf2181/8408449)

Barthelemy, **Halder**, Gong, Uhlemann (2024)\
*Making the leap I: Modelling the reconstructed lensing convergence PDF from cosmic shear with survey masks and systematics*\
[arXiv:2307.09468](https://arxiv.org/abs/2307.09468) &nbsp; [JCAP](https://iopscience.iop.org/article/10.1088/1475-7516/2024/03/060)

Friedrich, **Halder**, Boyle, Uhlemann, Britt, Codis, Gruen, Hahn (2022)\
*The PDF perspective on the tracer-matter connection: Lagrangian bias and non-Poissonian shot noise*\
[arXiv:2107.02300](https://arxiv.org/abs/2107.02300) &nbsp; [MNRAS](https://academic.oup.com/mnras/article/510/4/5069/6505138?login=true)

&nbsp;

### Intrinsic alignments and baryonic feedback

<img align="left" width="400" src="images/halo_feedback_probe_sensitivity.png" alt="Halo feedback sensitivity image" style="float:left; padding-right:12px" />

Weak lensing and other probes of the large-scale structure are shaped by astrophysical effects that must be modelled to infer the correct cosmology. Two of the most important are the intrinsic alignments (IA) of galaxy shapes and the redistribution of matter by baryonic feedback from galaxy formation. Within the LSST Dark Energy Science Collaboration, we have infused a range of IA models directly into weak lensing simulations and studied how they change non-Gaussian cosmic shear statistics, including the integrated 3-point functions. Using the FLAMINGO simulations, we have studied feedback from the perspective of halo assembly histories: which halo populations the thermal and kinetic Sunyaev-Zel'dovich effects, X-ray number counts and weak lensing are sensitive to (see image on the left; courtesy: *Lucie-Smith et al. 2025*), and when in their history feedback changes their mass. Feedback redistributes baryons most efficiently when halos reach a mass of about 10<sup>12.8</sup> solar masses.

<div style="clear:both"></div>

Harnois-Déraps, Šarčević, Medina Varela, et al. incl. **Halder** (LSST DESC, 2026)\
*Non-linear infusion of intrinsic alignment and source clustering: impact on non-Gaussian cosmic shear statistics*\
[arXiv:2509.25166](https://arxiv.org/abs/2509.25166) &nbsp; [MNRAS](https://doi.org/10.1093/mnras/stag1213)

Lucie-Smith, Peiris, Pontzen, **Halder**, Schaye, Schaller, Helly, McGibbon, Elbers (2025)\
*Cosmological feedback from a halo assembly perspective*\
[arXiv:2505.18258](https://arxiv.org/abs/2505.18258) &nbsp; [PRD](https://doi.org/10.1103/vh8n-9cr2)

&nbsp;

### Quantifying cosmological information

<img src="images/c3nn_architecture.png" alt="C3NN image" style="float:left; padding-bottom:12px" />

Going beyond 2-point statistics raises a practical question: how much information does each statistic carry, and how reliably can we extract it? With the Cosmological Correlator Convolutional Neural Network (C3NN), we fused a convolutional neural network with the framework of cosmological N-point correlation functions, so that the outputs of the network can be written explicitly in terms of analytically tractable correlation functions (see image above; courtesy: *Gong et al. 2024*). This opens the machine-learning "black box": we can rank how much each order of correlation function contributes to a task, such as distinguishing weak lensing convergence maps with different dark energy equations of state. I am also using random matrix theory to understand how noise in estimated covariance matrices affects cosmological inference.

Gong, **Halder**, Bohrdt, Seitz, Gebauer (2024)\
*C3NN: Cosmological Correlator Convolutional Neural Network, an interpretable machine-learning framework for cosmological analyses*\
[arXiv:2402.09526](https://arxiv.org/abs/2402.09526) &nbsp; [ApJ](https://doi.org/10.3847/1538-4357/ad582e)

&nbsp;
