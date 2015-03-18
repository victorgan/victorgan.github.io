---
layout: post
title: Active Machine Learning
---

A braindump of machine learning, given some interaction with the world.

Specifically, I want to predict a good track of a wheelchair given a combination of: 

- its past track
- training data
- some update ability of what it actually does

## Key Words

active learning, Markov decision processes, influence diagrams, causality, and reinforcement learning


## Kalman filters

- Given sensor data of previous time steps, estimate given states
- Kalman Filter is a Hiddem Markov Model where (states -> observations) z -> s, x -> y, 
- recursive algorithm: 1) predict, 2) update