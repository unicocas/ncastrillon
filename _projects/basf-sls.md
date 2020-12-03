---
date: 2018-01-1
published: true
sitemap: false
title: "Material Temperature Sensitivity"
description: "Sensitivity quantification of a powder bed manufacturing process"
categories: SLS, nylon, discrete element method, BASF, heat equation, voxels, additive manufacturing
disciplines: Discrete element method, Forward Euler, 3D heat equation, C++
media: Nylon-6, PA-6
ownership:
client: BASF SE
time_period: 2018
thumbnail: "/projects/basf-sls/A_131_LS_330W_high_def.gif"

website:
  button_text: Read my paper
  url: https://asmedigitalcollection.asme.org/manufacturingscience/article/141/8/081012/956045/Variability-of-Targeted-Material-Thermal-Responses?casa_token=S60dOSTjZdIAAAAA:diYAQy9I9C-eHBo9seW2gWz0I2L5_MsiiHnPcUTnRPwU5z7TNcsezPOVWdpa5-DLIqXGRyc

intro: |
  I wrote a finite difference (FD) thermal field solver from scratch in C++, with a forward Euler (explicit) time integration scheme. The thermal FD solver was formulated for both a lumped-mass model and for a 3D domain. Both models were applied to a selective laser sintering (SLS) process, which is an additive manufacturing technique where a laser scans and melts the top surface of a powder bed, sequentially building components layer-by-layer.

  Additionally, I built a wrapper that ran multiple deterministic simulations for quantifying the sensitivity of the thermal field based on slight input paramenter changes. In this case, the laser power input setting was perturbed.

  BASF SE provided the financial support for this study. Their material research division employed my thermal FD solver as a tool to aid their scientists develop the Ultrasint® PA6 product line for SLS processing.

  

content_layout:
  - section_layout: 1col
    images:
      - caption:
        description: 'Temperatures of the powder bed.'
        url: '/projects/basf-sls/A_131_LS_330W_high_def.gif'
        width:
        height:

  - section_layout: text
    content: |
      Here, we see a voxelized representation of a randomly deposited powder bed. Each spherical particle is discretized into a collection of voxels. Above, a cross section of colored voxels representing local material temperatures and phases. Below, a perspective view of the material particles, showing evidence of irradiation by a static, overhead Gaussian laser beam.

  - section_layout: 1col
    images:
      - caption:
        description: 'Top view of the powder bed.'
        url: '/projects/basf-sls/3D_temps.png'
        width:
        height:

  - section_layout: 1col
    images:
      - caption: Sensitivity of final material temperatures of the lumped-mass model from perturbations of the laser power setting for the following cases. (1) without thermal contributions – no cooling, (2) with all thermal contributions, and (3)-(5) with isolated thermal contributions.
        description: 'Lumped mass sensitivities'
        url: '/projects/basf-sls/sensitivity-trends.jpg'
        width:
        height:

  - section_layout: text
    content: |
      Above is the sensitivity of final material temperatures of a lumped-mass model (single particle) for different thermal model cases. (X) Without any thermal contributions – no cooling, (–) with all thermal contributions, and (▴)-(●) with isolated thermal contributions.

  - section_layout: 1col
    images:
      - caption:
        description:
        url: '/projects/basf-sls/BASF-logo-blue.png'
        width:
        height:
---
