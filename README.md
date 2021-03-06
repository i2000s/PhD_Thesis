# README
See the front-matter page for license information. Most of previous publications may be open-source (see below).

# Dispersive Quantum Interface with Atoms and Nanophotonic Waveguides

[Comments](https://github.com/i2000s/PhD_Thesis/issues) and [editorial inputs](https://github.com/i2000s/PhD_Thesis/pulls) are highly welcome!

Some data of plots are compiled into TikZ files.
Some data and scripts can be found in our previous paper repositories, for example, including [the repo for our Faraday spin squeezing protocol paper](https://github.com/CQuIC/FaradaySqueezingProtocol) (CC By 4.0),
and [the repo for the simulations of Green's tensors and spontaneous emission rates with waveguides](https://github.com/i2000s/simnanophotonics) (Jupyter notebooks with Julia v0.6 as the scripting language, MIT license).

Some of my handwritten notes that may or may not be included in this thesis are in the `temp` folder.

## Releases:
+ [Latest release](https://github.com/i2000s/PhD_Thesis/releases) -- v1.0.3 (June 7, 2018):
    + Use a general form of Green's tensors and mention the specific case for the BEM program we use in a footnote.
    + submit to the university repository for official release.

+ v1.0.2 (May 26, 2018):
    + fix the compiling process instruction.
    + add some notes on the conventions of reduced matrix elements.

+ v1.0.1 (May 17, 2018):
    + update official graduation month to July as requested.
    + add minor notes on some technical points.

+ v1.0 (May 10, 2018): official submission attempt.

+ Dissertation submission pre-release for committee review: April 10, 2018.

## Build
Dependence: [LaTeX 2e](https://www.latex-project.org/get/), [GNU Make](https://www.gnu.org/software/make/), and [Git](https://git-scm.com/downloads).

To compile the whole thesis:
```
git submodule init
git submodule update
cd main && make all clean
```
A PDF called `main.pdf` should be generated in the `main` folder.
The first two lines of the commands are to download the bibliography file.

To compile in a GUI editor, use the parameters defined in the `main/Makefile` code for `pdflatex`, `LuaLaTeX` and other commands.
Chapters can be compiled separately using the `.tex` files in the chapter folders.

## To Cite
[![DOI](https://zenodo.org/badge/91208437.svg)](https://zenodo.org/badge/latestdoi/91208437)

## Table of Content:

+ Chapter 1: Introduction
    + 1.1 Motivation
    + 1.2 Our toolbox: Atom-waveguide interface
    + 1.3 Quantum measurement, entanglement and spin squeezing with an atomic ensemble
    + 1.4 Outline of This Dissertation

+ Chapter 2: Atom-waveguide interface
    + 2.1 Introduction
    + 2.2 Polarization spectroscopy and dispersive light shift measures
        + 2.2.1 Measuring the polarization state of light in free space
        + 2.2.2 Polarization spectroscopy on waveguide interfaces
        + 2.2.3 Birefringence and Faraday effects caused by atom-light interactions
    + 2.3 Dispersive light response in the perspective of Green's function
        + 2.3.1 Eigenmodes of a dielectric waveguide
        + 2.3.2 Dyadic Green's functions of dipole radiations in presence of a dielectric waveguide
        + 2.3.3 Example Green's function of the nanofiber
    + 2.4 Phase shift and polarizability transformation
        + 2.4.1 Compare to the free-space case

+ Chapter 3: Spontaneous emission of atoms near a nanophotonic waveguide
    + 3.1 Polarizability of atoms
        + 3.1.1 Dipole oscillation and emission of polarized light
        + 3.1.2 Polarizability of alkali atoms
        + 3.1.3 Irreducible tensor representation of atomic polarizability
    + 3.2 Modification of decay rates of atomic transitions
        + 3.2.1 Free-dipole decay rates of multiplets and equivalent dipole method
        + 3.2.2 Waveguide-mediated decay rates
    + 3.3 Geometric effects of dielectric waveguide interfaces
        + 3.3.1 Modified decay rates from the perspective of waveguide geometry
        + 3.3.2 Enhanced anisotropy of guided modes with different geometries of waveguides

+ Chapter 4: QND measurement and spin squeezing using nanowaveguides
    + 4.1 Introduction
    + 4.2 Atom-light coupling with waveguide modes
    + 4.3 Some special states of alkali atoms
        + 4.3.1 Clock states and clock space
        + 4.3.2 Stretched states and their squeezing subspace
        + 4.3.3 Spin coherent states, Dicke states and spin squeezed states
    + 4.4 Spin squeezing induced by QND measurement

+ Chapter 5: Dispersive response theory, QND measurement and spin squeezing
    + 5.1 Introduction
    + 5.2 Dyadic Green's function and input-output field response
    + 5.3 Heisenberg-Langevin-picture solution and atomic response
    + 5.4 QND measurement of atoms based on the birefringence effect
        + 5.4.1 Dispersive atom number measurement
        + 5.4.2 Collective spin squeezing via QND measurement
        + 5.4.3 Decoherence due to optical pumping
    + 5.5 Summary and Outlook

+ Chapter 6: Enhanced cooperativity for measurement-induced spin squeezing
    + 6.1 Introduction
    + 6.2 QND measurement and cooperativity via the Faraday effect
    + 6.3 Spin-squeezing dynamics
    + 6.4 Summary and Outlook

+ Chapter 7: Conclusion and Outlook
    + 7.1 Summary
    + 7.2 Outlook
