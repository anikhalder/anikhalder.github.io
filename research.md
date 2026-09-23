---
layout: my-page
title: Research
---

My research connects the physics of galaxy populations with cosmology. Wide-area imaging surveys such as DES, KiDS, Euclid and the Vera C. Rubin Observatory's LSST map the positions, shapes and colours of millions to billions of galaxies. The same data record how galaxies form and evolve and how the large-scale structure of the Universe grows. I develop statistics that extract more of this information than standard 2-point analyses, infer the physical properties of galaxies at survey scale, and model the astrophysical effects that must be understood to interpret the data. A full list of publications is on [Google Scholar](https://scholar.google.com/citations?user=HZm11dQAAAAJ&hl=en) and [ORCID](https://orcid.org/0000-0002-0352-9351).

### pop-cosmos and galaxy populations

<img src="images/popcosmos_KiDS1000_colours_sSFR.png" alt="Inferred colours against redshift for 4 million KiDS-1000 galaxies, shaded by specific star-formation rate" style="float:left; padding-bottom:12px" />

[pop-cosmos](https://github.com/Cosmo-Pop/pop-cosmos) is a generative model for the evolving galaxy population, calibrated on deep multi-wavelength photometry from COSMOS2020. It provides a physically motivated prior over the galaxy population up to redshift *z* ≈ 6 in stellar population synthesis parameter space. Using this prior with an emulator for stellar population synthesis and GPU-accelerated sampling, we have inferred joint posteriors on the redshifts and physical properties (such as stellar mass and star-formation rate) of 4 million galaxies in the Kilo-Degree Survey (KiDS-1000). The image above shows their inferred colours against inferred redshift, shaded by specific star-formation rate (figure courtesy: *Halder et al. 2026*). This is the first principled Bayesian inference of galaxy properties for a wide-area weak lensing survey. We validated the redshifts against around 185,000 KiDS galaxies with DESI spectroscopic redshifts. The same galaxy population model also forward-models the KiDS-1000 redshift distributions directly, without spectroscopic reweighting. With these catalogues we can select galaxy samples by their physical properties rather than by colour proxies, which opens the way to weak lensing and multi-tracer analyses with better control of systematic effects such as intrinsic alignments.

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

<img src="images/6xi3PCFs_illustration_v4.png" alt="Illustration of the six integrated 3-point correlation functions of cosmic shear and galaxy density, and the parameter constraints they give" style="float:left; padding-bottom:12px" />

The integrated 3-point correlation functions (i3PCFs) are higher-order statistics that are easy to measure from galaxy imaging data alongside the standard 2-point correlation functions (see image above; figure courtesy: *Halder et al. 2023*). They measure the *position-dependent* 2-point correlation functions of cosmic shear and galaxy density inside local patches of the sky and correlate them with the mean shear or galaxy density in the same patches. This has a clear physical interpretation, the modulation of small-scale correlations by large-scale fluctuations, and gives access to the squeezed bispectrum of the fields. We developed perturbation-theory models for the i3PCFs that include galaxy bias, intrinsic alignments, baryonic feedback and observational systematics, validated them against N-body simulations, and built fast inference pipelines using neural-network emulators and simulation-based inference. On simulated DES Year 3-like data, adding the i3PCF to the shear 2-point functions improves the figure of merit for Ω<sub>m</sub>, σ<sub>8</sub> and w<sub>0</sub> by about 64%. We are now applying the i3PCF to DES Year 3 data.

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

<img align="left" width="330" src="images/jointPDF.png" alt="Joint probability distribution of matter and galaxy density fluctuations from simulations compared with the model" style="float:left; padding-right:12px" />

At any given scale, 3×2-point statistics compress the joint distribution of matter and galaxy density fluctuations into three numbers: their two variances and their covariance. The full shape of this probability distribution function (PDF) contains considerably more information. With my collaborators I have modelled the full shape of the joint matter and galaxy density PDF, including galaxy bias and stochasticity, and validated it against N-body simulations and mock galaxy catalogues (see image on the left; figure courtesy: *Friedrich et al. 2022*). We have extended this to the joint PDF of projected galaxy density and weak lensing convergence, released as the public toolkit CosMomentum, and to the PDF of the lensing convergence reconstructed from cosmic shear under the Dark Energy Survey Year 3 mask and systematics, preparing these statistics for application to survey data.

<div style="clear:both"></div>

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

<img align="left" width="400" src="images/halo_feedback_probe_sensitivity.png" alt="Halo masses and redshifts that tSZ, kSZ, X-ray and weak lensing probes are sensitive to" style="float:left; padding-right:12px" />

Weak lensing and other probes of the large-scale structure are shaped by astrophysical effects that must be modelled to infer the correct cosmology. Two of the most important are the intrinsic alignments (IA) of galaxy shapes and the redistribution of matter by baryonic feedback from galaxy formation. Within the LSST Dark Energy Science Collaboration, we have infused a range of IA models directly into weak lensing simulations and studied how they change non-Gaussian cosmic shear statistics, including the integrated 3-point functions. Using the FLAMINGO simulations, we have studied feedback from the perspective of halo assembly histories: which halo populations the thermal and kinetic Sunyaev-Zel'dovich effects, X-ray number counts and weak lensing are sensitive to (see image on the left; figure courtesy: *Lucie-Smith et al. 2025*), and when in their history feedback changes their mass. Feedback redistributes baryons most efficiently when halos reach a mass of about 10<sup>12.8</sup> solar masses.

<div style="clear:both"></div>

Harnois-Déraps, Šarčević, Medina Varela, et al. incl. **Halder** (LSST DESC, 2026)\
*Non-linear infusion of intrinsic alignment and source clustering: impact on non-Gaussian cosmic shear statistics*\
[arXiv:2509.25166](https://arxiv.org/abs/2509.25166) &nbsp; [MNRAS](https://doi.org/10.1093/mnras/stag1213)

Lucie-Smith, Peiris, Pontzen, **Halder**, Schaye, Schaller, Helly, McGibbon, Elbers (2025)\
*Cosmological feedback from a halo assembly perspective*\
[arXiv:2505.18258](https://arxiv.org/abs/2505.18258) &nbsp; [PRD](https://doi.org/10.1103/vh8n-9cr2)

&nbsp;

### Quantifying cosmological information

<img src="images/c3nn_architecture.png" alt="Architecture of the Cosmological Correlator Convolutional Neural Network (C3NN)" style="float:left; padding-bottom:12px" />

Going beyond 2-point statistics raises a practical question: how much information does each statistic carry, and how reliably can we extract it? With the Cosmological Correlator Convolutional Neural Network (C3NN), we fused a convolutional neural network with the framework of cosmological N-point correlation functions, so that the outputs of the network can be written explicitly in terms of analytically tractable correlation functions (see image above; figure courtesy: *Gong et al. 2024*). This opens the machine-learning "black box": we can rank how much each order of correlation function contributes to a task, such as distinguishing weak lensing convergence maps with different dark energy equations of state. I am also using random matrix theory to understand how noise in estimated covariance matrices affects cosmological inference.

Gong, **Halder**, Bohrdt, Seitz, Gebauer (2024)\
*C3NN: Cosmological Correlator Convolutional Neural Network, an interpretable machine-learning framework for cosmological analyses*\
[arXiv:2402.09526](https://arxiv.org/abs/2402.09526) &nbsp; [ApJ](https://doi.org/10.3847/1538-4357/ad582e)

&nbsp;
