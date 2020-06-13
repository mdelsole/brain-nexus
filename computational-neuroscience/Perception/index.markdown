---
layout: page
status: publish
published: true
title: 'Perception'
date: '2011-05-12 19:21:49 +0200'
date_gmt: '2011-05-12 19:21:49 +0200'
categories: []
order: 30
tags: []
---

* TOC
{:toc}

Perception is our window into reality. This section isn't really done, right now it's just some notes.

# Biology of vision

The reason we constantly move our eyes around is because we can see relatively little of the world in high resolution. We can coarsly sample a wide area, then move our eyes to view spots of interest in detail. It takes many, many receptors to see at high resolution.

Right in the retina, the brain starts encoding information in a very efficent way: in terms of contrast. Instead of encoding in *absolute values* we encode in *relative* values. 

There are two types of retinal cells: **on-center** and **off-center**. They can be modeled computationally as a difference of gaussians (DOG). They are sensitve to contrast; if you shine a light on the whole thing, there is no activity.

An alignment of these on-center off-center neurons is created in the connections to a particular V1 neuron, establishing an oriented edge detector. The can be light to dark or dark to light; two different polarities.

We only need to coarsly sample 4 orientations, because as with color we can interpolate the intermediate angles as a relative activity between these 4 different encodings of angles. 

These V1 simple cells can be modeled with gabor filters (wavy function) times a gaussian, which localizes the receptive field to a point in space.

In the superficial layers of V1, there are V1 complex cells. These are combinations of different simple cells organized to achieve a more specific filtering. We use these so the system doesn't have to learn it from scratch, although we'll see how these complex cells are learned initially.

# V1 Receptive Fields

Oriented edges are present in every image, no matter how different the images are.

Every V1 neuron recieves activity from its neighbors, with closest neighbors impacting the strongest. If one of the neighbors gets activated, the V1 neuron is more likely to get activated since it gets that extra excitation. The neighborhood relationship creates the pinwheel topography; weaker lateral connections makes much less organized topography. Each neuron just learns some random orientation coding.

# Invariant Object Recognition

The new machine learning object recognition models take from the old idea of Fukishima's neocognitron: Hierarchy of increasing **feature complexity** and **spatial invariance**.

Neurons in V2 have greater feature complexity by recongizing combinations of V1 (intersections, junctions of oriented edges), but they also recognize them over a larger range of different locations and angles/sizes. It's an incremental build-up of invariance. By the time you get to V4, you're recognizing more complex feature coding and more invariance in the features themselves. 

By doing this incrementally, you avoid the problem of binding errors; you don't want lower level features that don't actually relate to each other to be connected.

As a result of the accumulated effect, the affective receptive field that can activate a higher-level neuron is very large.

We backpropagate the IT error signal into V4 to adjust the earlier lower-level representations.

A V4 neuron recieves signals from a set area of V1 neurons; it is a 4x4 block of pools, which half-overlap with the V4 pool next to it. Each pool is one orientation. The x-axis is the orientation and the y-axis is the different types of features (polarity, end-stopping, etc.) The topography encourages the overall solution of invariance. 

## Activation-Based Receptive Fields

Similar to reverse correlation and spike-triggered averaging, we use something called an activation-based receptive field. It records the pattern of activity present when in an individual neuron is active. It's a weighted-average of how active a neuron is, from 0 to 1. We weight the corresponding pattern of activity in each of the different layers, as well as in the *input image* as a function of the activity of the individual neuron. 

This allows us to reconstruct what patterns in general tended to be present when these neurons were active, filtering out the other patterns when they weren't active. This is how we see what exactly the neurons come to represent. Because we record the activity of the input image, we can see the patters of input that activate these neurons.

The blur is evidence of spatial invariance; it's representing it across a range of spatial features.

## Attentional Mechanisms

Our ability to recognize backgrounds and our ability to filter out backgrounds are two different abilities. Many visual recognition models attempt to train with cluttered backgrounds. However, our ability to filter out backgrounds is the tied to our attentional mechanisms, rather than our ability to capture spatial invariance. 

These models end up learning texture-based representations as the way of discriminating objects that don't really match how the brain learns objects. They don't recognize shapes in the way the brain does. The learn the texture and repeated patterns, and don't have the solution to the invariance problem.

Take the classic example of "Where's Waldo?" We need to be able to focus attention on specific spatial positions. There's many distracting stimuli with similar features, and the only way we have to isolate the features of Waldo is by focusing our attention.

We have a zoomable attentional field that can focus wide or small.  

We have two pathways: One for visual object recognition, and one for "where" visual objects are. This "where" pathway also functions as a spatial processing pathway. Top-down activation from the spatial pathway can activate neurons in V1, thereby activating the proper neurons in the object recogition pathway.

Spatial attention can allow you to focus on a single object with multiple objects present in the scene. The area with more bottom-up activity will capture the spatial attention (activating it over another object), which will then feedback and make that object stand out.

Attention is just feedback neural activity plus inhibitory competition.


