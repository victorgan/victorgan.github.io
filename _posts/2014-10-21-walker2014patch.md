---
layout: post
title: Paper Review: Patch to the Future: Unsupervised Visual Prediction (walker2014patch)
---

- PDF: [walker2014patch]({{ site.url }}/assets/papers/walker2014patch.pdf)
- Video: [tech talk](http://techtalks.tv/talks/patch-to-the-future-unsupervised-visual-prediction/60335/)

## My Summary

Problem:

- predict future track and pose of cars
- given training data of cars
- given reward function

## Introduction

- Humans can infer what is happening next in an image

## This Work

- 1) What is active, and 2) How activity unfolds
- Builds on 'mid-level elements' [28]
- Model movements/transitions, an how the appearances of these elements change
- Advantages: 
    a. makes no asumption about what acts as an agent in the scene
    b. uses patched-based representation to learn models of visual prediction completely unsupervised
    c. mid-level elements
- Limitations
    - goal-driven behaviors
    - assume all elements in scene are static
    - limited to cars (tested/trained on cars)
- Pixels/HOG?
    - (low level features)
- High level features: human labelled cars, for example
- Mid level features (singh et al): data-derived HOG features

- Assume car patch can move in 8 different directions; eg. high probability of moving NW
- patches may also transition to different patch type (eg different car pose)
- scene interaction ( non-parametric reward function): likely to move on pavement, not other cars/buildings/etc.

- Given reward function and transition function, quantify decision
- Create a connected graphs of all possible states, weight each edge by expected reward
    - Do this for every patch entity
    - connect these individual graphs through appearance transitions
    
- Use dijstrka's algorithm to find series of decisions with least cost
- remove non-moving detections using transition probabilities
- Find optimal paths to every edge in the scene, rank paths by average expected reward
- combine to create a distribution of possibilities

### How do you train the transition and reward functions?

- transition function is learned through tracking entitites (KLT tracking), vote if it's appearance transition or a movement
- reward function based on texture information: in training, have a texture patch associated with each car template. Then propogate patch throughout testing frame. 

### Experiments

- first dataset: 300 minutes of youtube car chases
- distance of planned path vs real path taken (modified Hosteroff distance first mentioned in Kitani et al.)
- tested against data-driven baseline and agent-centric baseline
- second dataset: VIRAT dataset; they are state of the art

### Conclusion

- unsupervised method for prediction
- no explicit modeling of semantics
- predict appearance changes

### Questions

- How do you handle occlusions? It doesn't. Only for bird's eye view 2d.
- 

## Related Work

- previous methods: optical flow or point objects
- humans can predict motion and how appearances change with the movement, mental image of prediction
- Two main thrusts:
    1. Yuen et al 2010 (data driven)
    2. Agent-centric approach (kitani et al 2012) Markovian model describing future



