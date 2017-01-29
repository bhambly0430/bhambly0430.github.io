---
layout: post
title: "Voltammogram Model"
date: 2017-01-28
---

### Voltammogram Model
For the past few weeks, I have been working on a model that describes the voltammogram for a microdisk electrode. This model has the unique ability to describe the theoretical steady-state response that is typical for a microdisk electrode, but the model also has the ability to describe non-ideal conditions; e.g., very low or high diffusion coefficients and scan rates.

The current description of modern linear sweep voltammetry falls under one of two regimes: diffusion limited current or steady-state current. Large electrodes (macro electrode - millimeter size radius) produce the diffusion limited currents and produce a peak, and the maximum value of this peak is described by the *Randles-Sevick* equation. Small electrodes (microelectrode - micrometer size radius) do not show the same diffusion limited peak shape. Instead, microelectrodes produce a steady-state (sigmoidal) shape curve which is described by the *microelectrode* equation (great name right!). 

The differences between these two equations boil down to the dominating geometry of their concentration gradients. Macro electrodes have a linear diffusion geometry which microelectrode have a hemispherical dominating diffusion geometry. A problem arises when the experimental conditions do not match with the ideal conditions assumed in the microelectrode and Randles–Sevcik equation. 

In 1984 Aoki and Osteryoung developed a model that describes linear sweep voltammograms for small microelectrodes under various conditions. The complexity of this model has limited its use when compared to other more easily calculatable models; e.g., Randles–Sevcik, microelectrode, and Nicholson-Shain. Aoki and Osteryoungs model can be seen below.

![Aoki-Osteryoung Model][bhambly0430.github.io / _posts / 2017-01-28-photo.PNG ]

Where n is the number of electrodes in the reaction, F is Faraday's number, r is electrode radius, R is the gas constant, D is the diffusion coefficient, T is the temperature, v is the scan rate, t is the time, c is the concentration, E_i is the initial potential, and E^o is the standard redox potential.

As you can see this you can not plug this model into excel or your calculator to generate voltammograms. It was important that I was able to generate theoretical voltammograms using this model, so I created a piece of software to just that. You can download the software from the project's [GitHub Page](www.github.com/bhambly0430/Voltammogram_App).
