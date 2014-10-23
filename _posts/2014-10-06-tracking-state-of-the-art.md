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



## Initial Thoughts

- State of the Art RGB Trackers
    - Struck is one of the best 2D algorithms for 2011
    - TLD[16], CT[29], MIL[3],
semi-B[13], Struck[14] and VTD[17] ([song2013tracking]({{ site.url }}/assets/papers/song2013tracking.pdf))
- There is 'RGB Trackers' (initial bounding box), 'tracking-by-detection' (training data)
- Tracking by detection pipeline
    - Get detections (not fully accurate)
    - Connect detections into tracks (Hungarian algorithm, MRFs)

### Research Communities
- RGBD Object Detection
    - not a lot of machine learning has been done here
- Pedestrian Detection
- Object Detection in General
- RGB Tracking
- Tracking-By-Detection

### How things Relate
- RGBD object detection lags behind generic pedestrian detection
    - May give better results, but room for transferring knowledge of generic pedestrian detection to RGBD object detection
- Point cloud based features are a lot easier to track because they're already somewhat segmented.

## People

- Princeton seems to have a good RGBD tracking group
- Washington has RGBD detection (Dieter Fox's Group)
- Piotr knows pedestrian detection

## Papers

### song2013tracking

- Princeton Tracking Benchmark
- [song2013tracking]({{ site.url }}/assets/papers/song2013tracking.pdf)
- [http://tracking.cs.princeton.edu/](http://tracking.cs.princeton.edu/)
- 100 RGBD videos
- 15 evaluated algorithms
    - baseline does the best
- mostly traditional generic 'tracking', no 'tracking-by-detection'

### Spinello's Dataset
- [spinello](http://www2.informatik.uni-freiburg.de/~spinello/RGBD-dataset.html)

### xiao2013sun3d

- [xiao2013sun3d]({{ site.url }}/assets/papers/xiao2013sun3d.pdf)
- big database of human-view RGBD videos, annotated
- 3d construction/labelling tool
- [http://sun3d.cs.princeton.edu/](http://sun3d.cs.princeton.edu/)


### danelljan2014adaptive

- [danelljan2014adaptive]({{ site.url }}/assets/papers/danelljan2014adaptive.pdf)
- Adaptive Color Attributes for Real-Time Visual Tracking


### velocity from RGB-D

- Dataset: [http://cs.stanford.edu/people/teichman/stc/](http://cs.stanford.edu/people/teichman/stc/)
- Towards 3d object recognition via classification of arbitrary object tracks (RSS 2013)

## Realtime and Robust Hand Tracking from Depth

- Microsoft's CVPR 2014 hand tracking paper
- [qian2014realtime]({{ site.url }}/assets/papers/qian2014realtime.pdf)
- Local optimization + Initialization by part detection

> Tracking from only the last frame is fragile. Recent advances in human body tracking [24, 1, 15, 30, 27] have
> proven that the capability of re-initialization on every frame
> is critical for robust tracking.

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

- [schmidt2014dart]({{ site.url }}/assets/papers/schmidt2014dart.pdf)
    - parts-based ("articulated") object tracking, similar to kinect
    - human body, human hand, visual servoing

- [lai2013rgb]({{ site.url }}/assets/papers/lai2013rgb.pdf)
    - Book chapter on RGBD Object Detection

- [munaro2012tracking]({{ site.url }}/assets/papers/munaro2012tracking.pdf)
    - Tracking people within groups with RGB-D data
