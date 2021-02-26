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

MRPOD could also be applied to extract sub-noise level features. Check out the [documentation](https://mrpod.readthedocs.io/en/latest/intro.html) for more details and tutorials.

## [CARSpy](https://github.com/chuckedfromspace/carspy)

`carspy` is a python module for synthesizing and fitting experimental spectra obtained with Coherent Anti-Stokes Raman Spectroscopy (CARS).

## Laser Absorption Tomography

This is a python module for tomographic reconstruction of laser absorption measurements with irregular arrangement of the laser lines. It will be made open source on my GitHub page soon.

## [Pythonize](https://github.com/chuckedfromspace/pythonize)
