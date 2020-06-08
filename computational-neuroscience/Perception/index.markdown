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

Perception is our window into reality.

# Biology of vision

The reason we constantly move our eyes around is because we can see relatively little of the world in high resolution. We can coarsly sample a wide area, then move our eyes to view spots of interest in detail. It takes many, many receptors to see at high resolution.

Right in the retina, the brain starts encoding information in a very efficent way: in terms of contrast. Instead of encoding in *absolute values* we encode in *relative* values. 

There are two types of retinal cells: **on-center** and **off-center**. They can be modeled computationally as a difference of gaussians (DOG). They are sensitve to contrast; if you shine a light on the whole thing, there is no activity.

An alignment of these on-center off-center neurons is created in the connections to a particular V1 neuron, establishing an oriented edge detector. The can be light to dark or dark to light; two different polarities.

We only need to coarsly sample 4 orientations, because as with color we can interpolate the intermediate angles as a relative activity between these 4 different encodings of angles. 

These V1 simple cells can be modeled with gabor filters (wavy function) times a gaussian, which localizes the receptive field to a point in space.

In the superficial layers of V1, there are V1 complex cells. These are combinations of different simple cells organized to achieve a more specific filtering. We use these so the system doesn't have to learn it from scratch, although we'll see how these complex cells are learned initially.

# V1 Receptive Fields

 
