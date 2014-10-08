---
layout: post
title: Machine Learning Notes
---

## Notes from news in machine learning.

### October 2014

Deep Learning: Methods and Applications 

- [2014-09-19-deeplearning]({{ site.url }}/assets/posts/2014-09-19-deeplearning.pdf)

[Deep Learning Bandwagon](http://www.pyimagesearch.com/2014/06/09/get-deep-learning-bandwagon-get-perspective/):



> However, the latest article by Google, Intriguing properties of neural
> networks, has suggested there is a gaping hole lurking in every deep neural
> net.
> 
> In their paper, the authors are able to construct “adversarial images” — that
> is, taking an image and perturbing the pixel values in such a way that it makes
> it (effectively) identical to human eye, but can lead to a mis-classification by
> the deep net.
> 
> These adversarial images were constructed in a fairly involved manner — the
> authors purposely adjusted pixel values in an image to maximize the network’s
> prediction error, leading to an “adversarial image”, that when used as input to
> the net, is nearly always misclassified, even when applied to different neural
> nets trained on different subsets of the data.


[ADMM vs Gradient Descent](http://www.quora.com/Convex-Optimization/Whats-the-advantage-of-alternating-direction-method-of-multipliers-ADMM-and-whats-the-use-case-for-this-type-of-method-compared-against-classic-gradient-descent-or-conjugate-gradient-descent-method):

> Now, the answer: in general, gradient descent / conjugate gradient descent can
> only be used for differentiable and unconstrained optimization problems. ADMM
> can be used for any convex problem.
> 
> However, what ADMM does get you is the ability to perform distributed
> optimization without any apology (i.e., it will work for any convex problem). It
> lets you break up a larger problem into smaller, more manageable chunks. The
> smaller chunks can be solved using your favorite solver (including gradient
> descent). 

> Advantages
> 1. ADMM is more general than other methods in the sense that the loss function
>    doesn't need to be differentiable. Hence, it just works out of the box for
>    many problems. For example, traditional methods (such as GD, SGD, or Newton)
>    just don't work for optimization with L_1 regularization
> 2. Simple to implement
> 3. Simple to parallelize. Parallelizing L-BFGS, for example, is less trivial.
>    Parallelizing SGD is even trickier (if not impossible, without compromise).
> Disadvantages
> 1. Its convergence rate is poor


[UT Predictive Modeling Course](http://hercules.ece.utexas.edu/courses/pm14/index.html)


### September 2014

Data Mining vs Machine Learning (Mark Schmidt on Piazza Discussion):

> Great question, and thanks for the answers contributed by students. Machine
> learning and data mining have many similarities (as do other fields like
> statistics and signal processing), and the similarity is increasing due to the
> 'arXiv' effect (people from both fields can now easily read each other's papers
> and are using standard notation).
>  
> However, as a subjective answer I would say that the focuses are different. Data
> mining is broader in scope and includes things like how to organize data, models
> that simply look up answers or are based on counting (KNN and naive Bayes are
> also often covered in data mining, and in data mining there is a greater focus
> on interpretable models), and tasks like information visualization. Machine
> learning is more narrow, focusing largely on the modeling aspect, generalization
> error, and using methods that rely on numerical optimization or high-dimensional
> integration (that may not necessarily be interpretable).
>  
> Another subjective comment would be that data mining often focuses on tools that
> help professionals analyze their data, while machine learning often focuses on
> automating data analysis. E.g., here is a recent very-interesting project by
> some machine learning folks from Cambridge and MIT:
> http://www.automaticstatistician.com/
> 

(http://image-net.org/challenges/LSVRC/2014/slides/GoogLeNet.pptx)

[Microsoft ML Hackathon](http://blogs.technet.com/b/machinelearning/archive/2014/09/16/microsoft-machine-learning-hackathon-2014.aspx): 

> it was important to be working in teams and to be thoughtful about how to
> split a given ML challenge between team members.  Assigning roles and having
> clarity on what tools to use were critical considerations.

> We have seen similar patterns in other cases too, and boosted trees are a
> strong candidate on many ML tasks. If you have some special or temporal
> structure to the data, it may be easier to encode it using neural-nets
> (although exploiting it may be non-trivial). However, if there is no structure
> to the features or if you have a limited amount of time to spend on a problem,
> one should definitely consider boosted trees.

> In fact one of our Top 5 teams comprised entirely of summer interns who were
> new to this space.

## Questions
Questions I have, or once had.

#### What's the difference between boosted trees and random forests?

They both combine many decision trees.
Boosted trees uses boosting, random forest uses bagging.

#### What are common classifiers?

#### Any online plug-n-play ML solutions?

#### Is deep learning (R-CNNs) good because of its hierachical structure + lots of data?


