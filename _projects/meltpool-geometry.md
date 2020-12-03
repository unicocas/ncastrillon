---
date: 2020-05-01
published: true
sitemap: false
title: "Shape Characterization"
description: "A moments-based approach for material melt pool shape characterization"
categories: moments, geometry, melt pool, finite difference method
disciplines: Moments theory, Shape reconstruction, Gauss-Hermite polynomials
media: Voxelized 3D geometry
ownership:
client: Personal work
time_period: 2020
thumbnail: "/projects/meltpool-geometry/Laser_track.gif"

intro: |
  I built a Python-based, object-oriented tool from scratch to extract uncertainty quantification (UQ) information from shape data via a moments approach.

  My ultimate interest is to generate sets of moments data from the geometries of manufactured parts, and to apply UQ methods directly on this data. This will help link perturbations of process input parameters to their effects on final part geometries. It is my hypothesis that moments hold a richer and more accessible trove of information about shape versus an attempt to measure bulk dimensions, such as width, depth, radius, and others. The readiness of moments data will allow itself to be analyzed for UQ: slight changes of the as-manufactured part geometry will be evident by a direct comparison across sets of moments matrices.

  In this study, I use the paper by [Ganeriwala & Zohdi](https://link.springer.com/article/10.1007/s10035-016-0626-0) to recreate a sample problem. In this example, a set of discrete powder particles is deposited stochastically over a substrate that has been previously melted and has solidified. Then, a laser scans directly over head in a single track. The heat equation is solved via a coupled discrete element-finite difference method in 3D to evolve particle and substrate temperatures. Voila! I have generated a material melt pool geometry. Then, I generate the moments matrix for the shape with my moments calculation tool. I can repeat the process several times with slightly different sets of manufacturing process inputs to extract UQ information on this process.

content_layout:
  - section_layout: 1col
    images:
      - caption:
        description: 'laser scan animation'
        url: '/projects/meltpool-geometry/Laser_track.gif'
        width:
        height:

  - section_layout: text
    content: |
      The sample problem above generates a voxelized geometry of melted material (below), which is used for generating a unique _(p+1) x (p+1) x (p+1)_ moments matrix, where _p_ is the maximum moment order. This moments matrix will later be analyzed for quantifying uncertianty of the manufacturing process. In this case, for selective laser sintering (SLS) processing.

  - section_layout: 1col
    images:
      - caption:
        description: 'melt pool of processed powder'
        url: '/projects/meltpool-geometry/melt-pool-track.png'
        width:
        height:
---
