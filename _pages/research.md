---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

{% include base_path %}

An up-to-date list of refereed publications can be found on [NASA/ADS]([https://ui.adsabs.harvard.edu/search/q=orcid%3A0000-0001-6180-8482&sort=date%20desc%2C%20bibcode%20desc&p_=0](https://ui.adsabs.harvard.edu/search/filter_property_fq_property=AND&filter_property_fq_property=property%3A%22refereed%22&fq=%7B!type%3Daqp%20v%3D%24fq_property%7D&fq_property=(property%3A%22refereed%22)&q=%20author%3A%22yahalomi%2C%20d%22&sort=date%20desc%2C%20bibcode%20desc&p_=0)). 

I've had the opportunity to work in a number of topics in astrophysics. I often say that my journey to exoplanet research started on the largest astrophysical scales and then slowly moved inward to smaller and less energetic phenomonema. I've lead original research in gravitational microlensing of strongly lensed supernova, self-lensing binary star systems in Kepler data and with ground-based radial velocity (RV) Doppler observations, simulating what the search for Solar System analogous planetary architectures will look like with next generation RV and astrometric surveys, and in model selection for exoplanet transit timing variations (TTVs). <br>

For a brief summary of these projects, see below:

## "Killing" the Moon Hypothesis in the Kepler-1513b System
_Advisor: [Prof. David Kipping](http://davidkipping.co.uk/) <br>
_Paper: to be posted shortly, accepted in MNRAS (09/2023)_<br>

We performed model selection on the TTVs observed in Kepler-1513b using follow-up ground-based and space (TESS) observations, and found that the complete TTV signal adding in two more transits a ~decade later was no longer consistent with the moon hypothesis. <br>

Usting nested sampling with [MultiNest](https://github.com/JohannesBuchner/MultiNest), we modeled the TTVs with N-body simulations for the planet-planet model with [SWIFT](https://www.boulder.swri.edu/~hal/swift.html) and a photodynamical planet-moon model with [LUNA](https://arxiv.org/abs/1105.3499). We find that the planet-moon model is inconsistent with one the two new transit time observations at the ~3-\sigma level. <br>

<img align="center" src="../images/astero.gif">

## Asteroseismology & Machine Learning
_Advisors: [Prof. Daniel Huber](http://www.ifa.hawaii.edu/~dhuber/) & [Prof. Melissa Ness](http://user.astro.columbia.edu/~mkness/Home.html)_ <br>
_Paper: on [NASA/ADS](https://ui.adsabs.harvard.edu/abs/2021AJ....161..170S/abstract)_<br>
_Code: on [GitHub](https://github.com/MaryumSayeed/TheSwan)_

<img align="right" src="../images/astero.gif">

The abundance of time-series observations have motivated astronomers and machine learning experts to find efficient ways of data analysis. NASA missions like Kepler and TESS have been groundbreaking for stellar and exoplanet astronomy. Tools like asteroseismology - the study of stellar oscillations - can be used to accurately characterize a star and learn about its interiors. However, applying asteroseismology on thousands of stars is not an efficient way of calculating stellar properties. But recent efforts in machine learning have made it possible to efficiently analyze the large influx of astronomy data.

By working with both asteroseismologists and machine learning experts, we created a method called `The Swan` to derive stellar surface gravities using linear regression for 20,000+ stars. `The Swan` achieves high precision and can be applied for cool stars across the Hertzsprung-Russell diagram (ie. main sequence, red clump and red giant stars). For more details about the technique, check out the paper [here](https://ui.adsabs.harvard.edu/abs/2021AJ....161..170S/abstract).

<!-- ![astero](../images/astero.gif) -->

## Solar System Seismology
_Advisor: [Prof. Jason Rowe](https://physics.ubishops.ca/exoplanets/Jason_Rowe_cv.html)_ <br>

<img align="right" src="../images/uranus.gif" width=500>

NASA's Kepler mission discovered that planets like the ice giants - Uranus and Neptune - have higher occurrence rates in our galaxy, as compared to gas giants or Earth-like planets [Burke et al. 2015](https://ui.adsabs.harvard.edu/abs/2015ApJ...809....8B/abstract). Therefore, to understand the population of discovered exoplanets, it is crucial to understand the formation, internal structure, atmosphere and evolution of Uranus and Neptune.

We used seismology to study the interior structure of Uranus. Using observations from the K2 mission, we analyzed 40 days of continuous high-cadence photometry to measure seismic waves within Uranus, study its weather patterns, and observe the Sun using reflected light. Although we were unable to detect oscillations within Uranus, we measured solar oscillations using reflected light from the sun, and used asteroseismic scaling relations to derive solar mass and radius. For a similar study, check out [Rowe et al. 2017](https://ui.adsabs.harvard.edu/abs/2017AJ....153..149R/abstract).

## Gravitational Waves
_Advisor: [Prof. Jess McIver](https://phas.ubc.ca/users/jess-mciver)_ <br>

<img align="right" src="../images/gw.gif" width=500>

Einstein's theory of General Relativity describes gravity as spacetime curvature created by massive objects. When two massive objects - such as black holes or neutron stars - accelerate towards each other, they radiate energy in the form of gravitational waves (GW), or waves that ripple through spacetime. While detecting these gravitational waves at large distances is difficult, the Laser Interferometer Gravitational-Wave Observatory (LIGO) uses laser interferometry to measure the distortion of mirror spacings as a gravitational wave passes through Earth (see [animation](https://www.ligo.caltech.edu/video/ligo20160211v6)). Click [this link](https://www.ligo.caltech.edu/video/ligo20160211v2) to hear the sound of two black holes colliding!

In order to analyze the data obtained by LIGO and differentiate random noise from coherent signal, physicists use extensive methods to remove noise - or "glitches" - from observations. I studied the impact of one of these glitches, called 'Blue Mountains' or high frequency noise, in order to understand the impact of glitches on parameter estimation of compact binary coalescence signals. Some factors that I studied are the effects of glitch proximity to the merger time, sky localization, and inferred masses and spins. I also updated the data analysis pipeline used to run parameter estimation on GW signals using a Bayesian inference software library called [LALInference](https://ui.adsabs.harvard.edu/abs/2015PhRvD..91d2003V/abstract).


## Planet Formation
_Advisor: [Prof. Nienke van der Marel](http://www.nienkevandermarel.com/)_ <br>

The gravitational attraction between a protostar and surrounding dust grains causes larger pebbles to drift inward at timescales shorter than accretion timescales that prevent planet formation (termed the radial drift problem). However, the existence of a pressure bump within a disk would trap dust grains to buy time, and allow larger planetesimals to form.

This project aimed to observe IRS 48, the first asymmetric protoplanetary disk that showed evidence of a dust trap, in multiple wavelengths to model the morphology of the disk and investigate dust growth. I applied Markov chain Monte Carlo methods to model the disk using parameters for disk location, size and orientation, and created a spectral index map to probe dust distribution.


