---
title: "Zip-NeRF: Anti-Aliased Grid-Based Neural Radiance Fields"
date: "April 23, 2023"
tags: 
  - NeRF
  - Neural Radiance Field
  - Zip-NeRF
---

#Abstract
Neural Radiance Field training can be accelerated through the use of grid-based representations in NeRF's learned mapping from spatial coordinates to colors and volumetric density. However, these grid-based approaches lack an explicit understanding of scale and therefore often introduce aliasing, usually in the form of jaggies or missing scene content. Anti-aliasing has previously been addressed by mip-NeRF 360, which reasons about sub-volumes along a cone rather than points along a ray, but this approach is not natively compatible with current grid-based techniques. We show how ideas from rendering and signal processing can be used to construct a technique that combines mip-NeRF 360 and grid-based models such as Instant NGP to yield error rates that are 8%-76% lower than either prior technique, and that trains 22x faster than mip-NeRF 360.

link: https://jonbarron.info/zipnerf/
