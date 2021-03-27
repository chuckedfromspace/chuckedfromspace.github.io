---
permalink: "/projects/"
title: "Projects"
layout: page
---

## [EU-2020 SOPRANO](https://www.soprano-h2020.eu/)

Soot Processes and Radiation in Aeronautical Innovative Combustors (SOPRANO) is an [EU Horizon 2020](https://ec.europa.eu/programmes/horizon2020/) project (Grant Agreement No.690724) that aims at developing clean
and efficient combustion technologies for aircraft engines that can meet the
ambitious emission goals laid out in [Flightpath 2020](https://www.acare4europe.org/documents/latest-acare-documents/acare-flightpath-2050) by ACARE.

I am mainly involved in two of the [Work Packages (WP)](https://www.soprano-h2020.eu/about-soprano/project-structure/):

- WP2 with a focus on high-pressure sooting flames
- WP4 with a focus on new combustion technologies

Specifically for WP2, my task is to perform gas phase thermometry with Coherent Anti-Stokes Raman Spectroscopy (CARS) simultaneously with time-resolved two-color Laser-Induced Incandescence (TiReLII, led by my colleagues P. Nau and K.P. Geigle).
The main objective is to produce quantitative, correlated datasets of local soot volume fraction and gas temperature for the validation of CFD models in the
well-recognized gas turbine model combustor [FIRST](https://www.dlr.de/vt/en/desktopdefault.aspx/tabid-10814/18901_read-43897/), established at the German Aerospace Center (DLR).

For WP4, my main task is to investigate thermal effects on the injection of liquid fuels (such as kerosine or heating oil), especially in the superheated and supercritical regimes.
Besides the tuning of the high-pressure test facilities, I am responsible for carrying out (microscopic) laser shadowgraphy to quantify the changes in fuel sprays under various temperature and pressure conditions, by measuring droplet size, velocity and volume flux. Check out some of the import results in this [recent publication](https://doi.org/10.1115/GT2020-16037).

## [MRPOD](https://github.com/chuckedfromspace/mrpod)

`mrpod` is a python module developed to perform Mutiresolution Proper Orthogonal Decomposition (MRPOD) of multidimensional image time series. POD is the term often used in the field of fluid mechanics for Principle Component Analysis (PCA). The main motivation behind this project is to separate coherent flow patterns that co-exist over a wide range of frequencies in the gas turbine combustors. To achieve this goal, 2D discrete wavelet decomposition and reconstruction of the cross-correlation matrix from PCA. By careful selection and construction of composite wavelet filters, PCA can be carried out in well defined frequency domain to extract target flow features.

For instance, MRPOD can be used to recover distinct dynamics by decomposing the convoluted flow field:

<img src="https://mrpod.readthedocs.io/en/latest/_images/mov_mix.gif" width="400px"/>

and reconstructing it in specific spectral ranges:

<img src="https://mrpod.readthedocs.io/en/latest/_images/mov_pvc.gif" width="400px"/>
<img src="https://mrpod.readthedocs.io/en/latest/_images/mov_tv.gif" width="400px"/>

MRPOD could also be applied to extract sub-noise level features. Check out the [documentation](https://mrpod.readthedocs.io/) for more details and tutorials. Find out how to apply MRPOD to vector/scalar fields from experiments and CFD in these two recent publications: [Yin2020](https://doi.org/10.1017/jfm.2019.762), [Grader2020](https://doi.org/10.1016/j.proci.2020.05.019).

## [CARSpy](https://github.com/chuckedfromspace/carspy)

`carspy` is a python module for synthesizing and fitting experimental spectra obtained with Coherent Anti-Stokes Raman Spectroscopy (CARS). CARS is a gas phase thermometry with high spatial and temporal resolutions as well as accuracy (relative to other non-intrusive diagnostics).
`carspy` is not intended as a replacement to some of the well-established fitting routines. I started this project originally to learn more about CARS theories and it gradually evolved into a full-fledged program. I decided to make it open source so other CARS practitioners could examine the maths, implementation methods and potentially improve/expand it. The current structure of `carspy` is illustrated in the following:

<img src="https://raw.githubusercontent.com/chuckedfromspace/carspy/main/assets/carspy_struct.png" width="600px"/>

The core of `carspy` depends only on `numpy`. The least-square fit part is implemented using `lmfit`, which provides much more flexibilities than the basic `scipy` methods. Good agreements have been achieved between when comparing the synthesized spectra from `carspy` to other published routines:

<img src="https://raw.githubusercontent.com/chuckedfromspace/carspy/main/assets/vs_CARSFT_01.jpeg" width="500px"/>

Check out the [documentation](https://carspy.readthedocs.io/) for more details or just give it try by simply installing it via:

```console
$ pip install carspy
```

## Laser Absorption Tomography

This is a python module for tomographic reconstruction of laser absorption measurements with irregular arrangement of the laser lines. It will be made open source on my GitHub page soon.

## [Pythonize](https://github.com/chuckedfromspace/pythonize)

Pythonize is an open source knowledge base with a focus on using python for data crunching and visualization. It covers all topics that interest me personally: fluid dynamics, spectroscopy, machine learning, finance (investing) to name a few. The site is built with the [Jupyter Book project](https://jupyterbook.org/) (since I'm quite a fan of restructuredtext and `sphinx`). My goal is to slowly add posts in the form of Jupyter notebooks to it on a regular basis.
This is by no means a collection of python tutorials. There are more than enough of them on the Internet. I hope to create more original content that I think might also interest others.
