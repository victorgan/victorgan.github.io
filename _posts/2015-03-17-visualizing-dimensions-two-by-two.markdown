---
layout: post
title: Visualizing Dimensions, Two-by-Two
---

I want to visualize stuff in high dimensions.

Plotting the first two [principle
components](https://www.google.ca/search?q=principal+component+analysis&tbm=isch) is an
option.  [T-SNE](https://www.google.ca/search?q=t-sne&tbm=isch) is another, a
method that clusters points that are close in high dimensional space. But I want
even more intuition! So I made a way to generate a video that shows *every*
pair of dimensions, with smooth rotations between pairs.

![A spiral in 4D]({{ site.url }}/assets/posts/2015-03-17-visualizing.gif)
Above you're seeing all 2D projections of some 4D spiral. Even though it has
four dimensions, you're seeing all 2D projects of it.

Here's how it works. I display two dimensions at a time, then transition to two
more.  I need to choose which dimensions to display, and what pair of dimensions
to display next. To avoid sudden viewpoint changes, only one dimension should
change between successive dimension pairs. In this way, I'm always displaying
three dimensions. 

Making sure I display every possible dimension pair in an order where only one
of the two dimensions change every iteration is similar to the concept of
[gray codes](http://en.wikipedia.org/wiki/Gray_code). Gray codes involve
counting in binary where successive values only differ by one bit.  For example,
a 2-bit gray code ordering could look like:

| Binary | Gray Code |
|--------+-----------|
| 00     | 00        |
| 01     | 01        |
| 10     | 11        |
| 11     | 10        |

(Notice how only one bit changes per row for the gray code.) 

In fact, my exact problem is called the gray code combination problem, or the
revolving door problem.

![2-revolving door problem. Image derived from Knuth's "Art of Computer Programming"]({{ site.url }}/assets/posts/2015-03-17-revolving-door.png)
2-revolving door problem: Imagine there are 2 of $$d$$ people separated by a
revolving door. When someone enters the right room, somebody else must enter the
left room at the same time. Can we find a sequence of moves so that each
combination of pairs of people occur exactly once?

For example, if the number of people $$d$$ (or in my problem, the number of
dimensions) is 4, these sequences of moves could work:

| 2-Combination Gray Code | Dimension # |
|-------------------------+-------------|
| 0011                    | 1, 2        |
| 0110                    | 2, 3        |
| 0101                    | 1, 3        |
| 1100                    | 3, 4        |
| 1010                    | 2, 4        |
| 1001                    | 1, 4        |

Notice how one dimension is consistent between neighbouring rows.

Now, say I'm showing dimensions 1 and 2 and want to show dimensions 2 and 3. I
need to make dimension 3 appear and dimension 1 disappear. Fortunately, the
components in the z-axis pointing out of the screen don't affect what's being
displayed, something I can exploit to do some disappearing dimension tricks.  I
can consider the invisible z-axis to be the dimension to appear (dimension 3 in
my example) and rotate the axis correponding to the disappearing dimension (2)
to it so the disappearing dimension becomes the new z-axis, becoming invisible.
This is done with a rotation around the remaining axis of the three. 

Then, as long as I keep our axis to dimension assignments consistent between
transitions, I can rotate to each successive dimension pair smoothly. Voila,
you're seeing in high dimensions!

MATLAB code can be found at:
[https://github.com/victorgan/dimensions-two-by-two](https://github.com/victorgan/dimensions-two-by-two)

