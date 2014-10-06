---
layout: post
title: RPE Tracking State of the Art
---

## Goal: Find State of the Art in Tracking with RGB-D Cameras

### Procedure

1. Google Scholar Search: 'tracking'
2. List benchmarks and datasets
3. List important people and research groups
4. Take saved papers and link them here
5. Write up a brief literature review
6. Go over previous tracking papers



### Initial Thoughts

- Struck is one of the best 2D algorithms for 2011


### State of the Art RGB Trackers
- TLD[16], CT[29], MIL[3],
semi-B[13], Struck[14] and VTD[17] ([song2013tracking]({{ site.url }}/assets/papers/song2013tracking.pdf))

## Papers

### song2013tracking

- Princeton Tracking Benchmark
- [song2013tracking]({{ site.url }}/assets/papers/song2013tracking.pdf)
- [http://tracking.cs.princeton.edu/](http://tracking.cs.princeton.edu/)
- 100 RGBD videos
- 15 evaluated algorithms
    - baseline does the best
- mostly traditional generic 'tracking', no 'tracking-by-detection'

### xiao2013sun3d

- [xiao2013sun3d]({{ site.url }}/assets/papers/xiao2013sun3d.pdf)
- big database of human-view RGBD videos, annotated
- 3d construction/labelling tool
- [http://sun3d.cs.princeton.edu/](http://sun3d.cs.princeton.edu/)

## Papers To Read

- [pellegrini2009you]({{ site.url }}/assets/papers/pellegrini2009you.pdf)
    - You’ll Never Walk Alone: Modeling Social Behavior for Multi-target Tracking

- [breitenstein2009robust]({{ site.url }}/assets/papers/breitenstein2009robust.pdf)
    - Robust tracking-by-detection using a detector confidence particle filter

- [choi2013rgb]({{ site.url }}/assets/papers/choi2013rgb.pdf)
    - Particle filter RGBD tracking, efficiently on CUDA GPU (real-time)
    - uses color + 3d points and surface normal features
    - synthetic sequences =(
    - tested against PCL