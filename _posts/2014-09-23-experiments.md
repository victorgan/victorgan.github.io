---
layout: post
title: Experiments
---

## Experiment 1

### Goal
Determine if motion history image culling or my proposed culling method is
better.

### Procedure
Used 7 identified keyframes, see if they overlap

1. Find isFlagged for MHI
2. Apply windowing function for 1.

### Results
For MHI with windowing function:

- Frames culled: 0.8444
- Recall: 0.8571

Worse frames culled, better recall.

### Comments
Experiment seems brittle; 7 significant events are too low.

## Experiment 2

### Goal
Create a baseline, MHI images

### Procedure
1. Get energy per frame: Run motion history on training data with parameters (30,30).
2. Calculate a threshold on min energy for frame to be flagged; allow 90% of
   frames to not be flagged.
3. Run MHI on test video; use calculated threshold
4. Run windowing function on it

### Results
- Threshold is 0.2.

### Comments
None.

## Experiment 3a

### Goal
See if full body detections is better than head + body, then connect.

### Procedure

1. Find large bounding boxes for full giraffes
    - [x y width height] to [x1 y1 x2 y2]
    - ymax(head rect, body rect) and xmax(head, body)

### Results
Found. Stored in GiraffeTests/20140925 Full Giraffes

### Comments
None

## Experiment 3b
### Goal
Find suitable box size for comparing full giraffes

### Procedure
1. Find average height and average width; find minimum height and minimum width
2. Use the minimum rounded to 8, 16, 32, 64?
3. imresize to fit 64x64?
### Results

#### Average/min width and height
>> mean(giraffeRectAMatrix(:,4:5),1)
   53.8377   52.6849

>> min(giraffeRectAMatrix(:,4:5))
    47    31

>> mean(giraffeRectBMatrix(:,4:5),1)
   61.1944   61.2942

>> min(giraffeRectBMatrix(:,4:5))
    47    50

#### Ratio

>> mean(giraffeRectBMatrix(:,4)./giraffeRectBMatrix(:,5))
    1.0056

>> mean(giraffeRectAMatrix(:,4)./giraffeRectAMatrix(:,5))
    1.1957

### Comments
Finding minimum might not work. Perhaps find the optimal resizing ratio. Or just
do a square; that seems alright.
Taking the Min doesn't say anything because it doesn't match the body-heads.
Taking a square size, perhap the minimum for efficiency reasons, will work.
47 by 31 is the size of the body. Use 48 by 48.

## Experiment 3c

### Goal
Train classifier on Video A, 8 rounds of hnm

### Procedure
Run on hardnegativemining function; imresize to 48 by 48
Change featuresFromRectsIndicies(featureImage, rectangles)
Change BaseBoxSize

### Results
It's training.
Training is done.

### Comments
I'm trashing my code. Note to self: make smaller functions.
Minor bug in display and calculating prec/recall, but it seems to work. Have
classifier file.

## Experiment 3d

### Goal
Test on Video B, record precision/recall

### Procedure
1. Change file stuff
2. Since featuresFromRectsIndicies and baseBoxSizes already changed, don't have
   to do much
3. Fix errors
E:\Personal Documents\2014 Disney\GiraffeTests\0926TestOut\clsfy-hog-svm-VideoA-VideoB_001fps\thresh_0.6\images

### Results
2014-09-26 Fri 04:49 PM
Very good results. Hm...

### Comments

### Experiment 3

## Goal
4. Compare with head + body + culling
4. run hard negative mining on all images
5. test on X

## Procedure

## Results

## Comments
