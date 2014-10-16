---
layout: post
title: Machine Learning Notes
---

## Notes from news in machine learning.

### October 8, 2014


[Shotton on Deep
Networks and Decision Jungles](http://blogs.technet.com/b/machinelearning/archive/2014/08/20/machine-learning-meet-computer-vision-part-2.aspx):


> Recently, we have been taking baby steps towards addressing particularly the
> latter two of these opportunities. We’re particularly excited by our recent
> work on decision jungles: ensembles of rooted decision DAGs. You can think of
> a decision DAG as a decision tree in which child nodes have been merged
> together so that nodes are allowed to have multiple parents. Compared to
> decision trees, we’ve shown that they can reduce memory consumption by an
> order of magnitude while also resulting in considerably improved
> generalization. A DAG also starts to look a lot like a neural network, but
> does have two important differences: firstly, the structure is learned jointly
> with the parameters of the model; and secondly, the DAG retains the idea from
> decision trees of efficient conditional computation: a single test example
> follows a single path through the DAG, rather than traversing all nodes as
> would be the case with a neural network. We’re actively investigating whether
> decision jungles, perhaps in conjunction with other forms of deep learning
> including stacking and entanglement, can offer an efficient alternative to
> deep neural networks.


[Joesph Sirosh on ML](http://blogs.technet.com/b/machinelearning/archive/2014/06/26/the-joy-and-hard-work-of-machine-learning.aspx):

> However, building ML systems is slow, time-consuming and error prone. Even
> though we are able to analyze very large data sets these days and deploy at very
> high transaction rates, several bottlenecks remain:
> 
> - ML system development requires deep expertise. Even though the core principles
>   of ML are now accessible to a wider audience, talented data scientists are as
>   hard to hire today as they were two decades ago.
> - Practitioners are forced to use a variety of tools to collect, clean, merge
>   and analyze data. These tools have a steep learning curve and are not
>   integrated. Commercial ML software is expensive to deploy and maintain.
> - Building and verifying models requires considerable experimentation. Data
>   scientists often find themselves limited by compute and storage because they
>   need to run a large number of experiments that generate considerable new data.
> - Software tools do not support scalable experimentation or methods for
>   organizing experiment runs. The act of collaborating with a team on
>   experiments, sharing derived variables, scripts, etc. is manual and ad-hoc,
>   without tools support. Evaluating and debugging statistical models remains a
>   challenge.



[Chris Burges on Boosted Decision Trees (BDTs)](http://blogs.technet.com/b/machinelearning/archive/2014/09/10/from-stumps-to-trees-to-forests.aspx):

> greedily trained trees aren’t likely to work as well on tasks for which the label depends only on combinations of many features

> three classic machine learning issues: generalization, feature design, and
> greedy learning...fourth classic machine learning issue: choice of a cost
> function...fifth major issue in machine learning: regularization, or the
> avoidance of overfitting.

[Chris Burges on ML](http://blogs.technet.com/b/machinelearning/archive/2014/07/11/machine-learning-for-industry-a-case-study.aspx?WT.mc_id=Blog_MachLearn_General_DI):

> We have already touched on one of the keystones of progress: the ability to do
> rapid experimentation. If you have what you think is a good idea, ideally you’d
> like experimental evidence, one way or the other, immediately. Thus even if a
> model initially does not perform quite as well as what one already has, if it is
> much faster to train and test, overall progress can be much faster, and this
> alone will often enable the model to quickly surpass the current one in accuracy
> and speed.

> Today, a family of models called Boosted Decision Trees (BDTs) are particularly
> popular.
> Logs collected on an ML service that is used internally within Microsoft show
> that, over the past year alone, there were over 670,000 training runs using BDTs
> throughout Microsoft.
> In 2010, Yahoo! organized a learning to rank challenge...the most interesting
> takeaway was that the top 5 systems all used ensembles of decision trees, and
> boosting, in one form or another (in fact our system was an ensemble of BDTs and
> neural nets). So, if you’re thinking of training a fixed model to solve a
> predictive task, it’s worth considering BDTs.

> The hardest challenges of doing research are asking the right question, and
> getting good validation of the ideas (in addition to the time-honored method of
> publication, which as a validation test can be quite noisy). Working on real
> problems that matter to millions of people is a pretty good way of getting help
> with both of these challenges.

> Some of the advantages that BDTs offer over neural nets, two of which are:
> - The ability to more naturally handle features whose ranges vary hugely from
>   one feature to another, and
> - Faster training, and hence faster experimentation turnaround time. 
> Subsequently a team led by Ofer Dekel showed how to engineer BDTs so that
> training became approximately two orders of magnitude faster than for the
> neural nets, and also able to handle much larger datasets.



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

> Different machine learning problems have different characteristics. Boosted algorithms in particular are sensitive to overfitting if the data is noisy -- boosting exhibits higher variance (in the sense of the bias-variance tradeoff discussed here: http://en.wikipedia.org/wiki/Sup...), but when it does work, it works well. 
> 
> Random forests, on the other hand, show very low variance, because the ensembles are not built on the residuals the way Gradient-boosted Machines does. 
> 
> In short: you have to try both out on your problem domain; sometimes random forests will match the data's biases better and sometimes GBM will.

> There is one fundamental difference between the two that may force you to choose Random Forests over Gradient Boosted Machines (GBMs). That is, Random Forests can be easily deployed in a distributed fashion due to the fact that they can run in parallel, whereas Gradient Boosted Machines only run trial after trial. So, if you are constrained either by the size of the data or the number of trials you want to try, you may have to go with random forests.



#### What are common classifiers?

#### Any online plug-n-play ML solutions?

#### Is deep learning (R-CNNs) good because of its hierachical structure + lots of data?


