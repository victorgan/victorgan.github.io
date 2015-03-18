---
layout: post
title: Bag of Little Bootstraps
---


Bootstrapping also described in [resampling methods]({% post_url 2014-10-06-resampling-methods %}).


Random Forests: Bootstrap Aggregating with CART Trees.

New RF: Bag of Little Bootstraps with CART Trees.

## To Do

one note notes

- [Bagging + RF Slides](http://pegasus.cc.ucf.edu/~xsu/CLASS/STA5703/notes11.pdf)
- [CART + random forests](http://docs.salford-systems.com/AdeleCutler.pdf):

> CART Pros
> 1. Applicable for both classification and regression with no formal
>    assumptions on the data structure.
> 2. Can be applied to large datasets.
> 3. Handles missing data effectively.
> 4. Deals with categorical variables efficiently
> 5. The picture of the tree can give valuable insights into which variables are
>    important and where.
> 6. The terminal nodes suggest a natural clustering of data into homogeneous
>    groups.
> 
> CART Cons
> Accuracy: stateまofまtheまart methods have much lower
> error rates than CART.
> 
> Instability: if you change the data a little, the tree
> picture can change a lot, so the interpretation is built
> on shifting sands.
