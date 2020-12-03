---
date: 2019-05-15
published: true
sitemap: false
title: "Research of Analysis Methods"
description: "A novel method for computing sensitivity with a moments-based formulation"
categories: moments, finite element method, geometry, analysis, sensitivity, optimization, PDE
disciplines: adjoint-based sensitivity, moment-based representation, finite element method, topology optmization, computational geometry, Python
media: All geometric representations
ownership:
client: Intact Solutions Inc.
time_period: 2019
thumbnail: "/projects/intact/mixed_representation_square.png"

website:
  button_text: Visit Intact Solutions
  url: https://www.intact-solutions.com/pnp/

intro: |
  This work was supported by Intact Solution Inc., a research company specializing in providing fully automated and customized software solutions to engineering problems. Their technology relies on an [innovative approach](https://www.sciencedirect.com/science/article/abs/pii/S0010448518302549) that is agnostic to input geometric representations, allowing unprecedented ease of engineering analysis services.

  As a research & development graduate student intern, I formulated a mathematical method for sensitivity calculations within the flagship product Intact.Simulation™. This work was possible through extensive literature reviews and subject matter expert interviews within the topology optimization and the adjoint-based sensitivity formulaiton spaces.

  Fully agnostic to the input geometric design space representation, the novel sensitivity method employs moments theory to evaluate derivatives of integral properties. This moments approach incorporates diverse geometric representations and objective functions into a single system. This new architecture for engineering analysis brings topology optimization, shape optimization, and material field design within reach.

  _A publication on this work is forthcoming._



content_layout:
  - section_layout: 1col
    images:
      - caption:
        description: 'Moment-based sensitivity approach'
        url: '/projects/intact/moment_derivatives_method.png'
        width:
        height:

  - section_layout: text
    content: |
      This voxelized representation of a bracket showcases a local sensitivity calculation via a SIMP approach. Structural compliance and a themal compliance cases are shown in here.

  - section_layout: 2col
    images:
      - caption:
        description: 'Bracket structural compliance BC'
        url: '/projects/intact/structural_bracket_bc.png'
        width:
        height: 
      - caption:
        description: 'Structural compliance  sensitivity  field'
        url: '/projects/intact/hi-res-bracket-structural.png'
        width:
        height:

  - section_layout: 2col
    images:
      - caption:
        description: 'Bracket thermal compliance BC'
        url: '/projects/intact/bracket_thermal.png'
        width:
        height: 
      - caption:
        description: 'Thermal compliance sensitivity field'
        url: '/projects/intact/hi-res-bracket-thermal.png'
        width:
        height:

  - section_layout: 1col
    images:
      - caption:
        description: 'Intact Solutions logo'
        url: '/projects/intact/intact-logo-white.png'
        width:
        height:
---
