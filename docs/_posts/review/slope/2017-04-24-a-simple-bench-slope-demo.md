---
layout: post
title:  "FLAC3D 5.0 - A Simple Bench Slope Demo"
tags: flac3d
categories: flac3d
---

```
https://www.youtube.com/watch?v=2oDxTriFlGU&index=2&list=PLDFD1CA2F2BB818C5
```

in this video, we create a simple model of a pit slope with two benches and calculate the stability of the slope.

Benched slope in rock with a weak vertical band.

calc_fos.f3dat

```
; evaluate Fos for new geometry
delete zones
generate zone extrude
model mech mohr
prop dens 2000 bulk 1e10 shear 3e9
prop cohesion 15000 friction 40
prop cohesion 7000 firction 20 rang group 'weakrock'
fix x range x -.5 .5
fix x range x 99.5 100.5
fix y range y -.5 .5
fix y range y 39.5 40.5
fix x y z range z -.5 .5
set gravity 0 0 -10
solve fos
```

<img src="/images/factor-of-safety.png">