---
layout: page
title: A Closest Point Method for PDEs on Manifolds with Interior Boundary Conditions for Geometry Processing
img: assets/img/publication_preview/CPM_IBC_GP.png
importance: 1
category: Peer-Reviewed
related_publications: false
publisher: ACM Transactions on Graphics, 2024
---

##### [Nathan King](https://nathandking.github.io), [Haozhe Su](https://soldierdown.github.io/), [Mridul Aanjaneya](https://orionquest.github.io/), [Steven Ruuth](https://steveruuth.org/), and [Christopher Batty](https://cs.uwaterloo.ca/~c2batty/)

##### ACM Transactions on Graphics 2024

{% include figure.liquid loading="eager" path="assets/img/CPM_IBC_GP_Teaser.png" title="example image" class="img-fluid rounded z-depth-1" %}

[<img src="https://raw.githubusercontent.com/FortAwesome/Font-Awesome/6.x/svgs/solid/file-pdf.svg" width="30" height="30">](https://arxiv.org/pdf/2305.04711) [<img src="https://raw.githubusercontent.com/FortAwesome/Font-Awesome/6.x/svgs/brands/github.svg" width="30" height="30">](https://github.com/nathandking/cpm-ibc)

<hr>
### Abstract

Many geometry processing techniques require the solution of partial differential equations (PDEs) on manifolds embedded in $$\mathbb{R}^2$$ or $$\mathbb{R}^3$$, such as curves or
surfaces. Such manifold PDEs often involve boundary conditions (e.g., Dirichlet or Neumann) prescribed at points or curves on the manifold’s interior or
along the geometric (exterior) boundary of an open manifold. However, input manifolds can take many forms (e.g., triangle meshes, parametrizations,
point clouds, implicit functions, etc.). Typically, one must generate a mesh
to apply finite element-type techniques or derive specialized discretization
procedures for each distinct manifold representation. We propose instead
to address such problems in a unified manner through a novel extension
of the closest point method (CPM) to handle interior boundary conditions.
CPM solves the manifold PDE by solving a volumetric PDE defined over the
Cartesian embedding space containing the manifold, and requires only a
closest point representation of the manifold. Hence, CPM supports objects
that are open or closed, orientable or not, and of any codimension. To enable
support for interior boundary conditions we derive a method that implicitly
partitions the embedding space across interior boundaries. CPM’s finite
difference and interpolation stencils are adapted to respect this partition
while preserving second-order accuracy. Additionally, we develop an efficient sparse-grid implementation and numerical solver that can scale to
tens of millions of degrees of freedom, allowing PDEs to be solved on more
complex manifolds. We demonstrate our method’s convergence behaviour
on selected model PDEs and explore several geometry processing problems:
diffusion curves on surfaces, geodesic distance, tangent vector field design,
harmonic map construction, and reaction-diffusion textures. Our proposed
approach thus offers a powerful and flexible new tool for a range of geometry
processing tasks on general manifold representations.

<hr>
### Video


<iframe width="720" height="405" src="https://www.youtube.com/embed/Yicp5KdTlp4" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<hr>
### Citation


```
@article{king2024closest,
  title={A Closest Point Method for PDEs on Manifolds with Interior Boundary Conditions for Geometry Processing},
  author={King, Nathan and Su, Haozhe and Aanjaneya, Mridul and Ruuth, Steven and Batty, Christopher},
  journal={ACM Transactions on Graphics},
  year={2024},
  publisher={ACM New York, NY},
  doi={http://dx.doi.org/10.1145/3673652},
}
```