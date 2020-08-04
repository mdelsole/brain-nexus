---
layout: page
status: publish
published: true
title: 'Memory'
date: '2011-05-12 19:21:49 +0200'
date_gmt: '2011-05-12 19:21:49 +0200'
categories: []
order: 40
tags: []
---

What do you think of when think about "memory"? For most people, they think about **episodic memory**; memory of specific events. You remember things like your 10th birthday and the time you broke your arm. Although this type of memory is the most noticeable, it's actually just one of many different types of memory.

A big division in memory we can make, at least mechanics-wise, is between **weight-based** and **activation-based** forms of memory. Weight-based memory is a result of *synaptic plasticity*, and is generally long lasting (from hours up to years). Activation-based memory is a result of *ongoing neural activity*. It's much more transient and fleeting, but also more flexible. 

Weight-based memory exists at every modifiable synapse in the brain. Because of this, it can manifest in innumerable ways. In this chapter, we'll focus on many of these ways.

You've probably heard of the **hippocampus**. This region of the brain plays a critical role in **episodic memory**. What is it that makes the hippocampus so good at episodic memory? See, a major strength of our cortex is also a major problem. The cortex is all about organizing knowledge to have *overlap*, so that we can recognize when things are similar. The problem is that similar memories will interfere with each other; they'll share connections and it will be impossible to isolate the memories from each other. 

The hippocampus solves this with **highly sparse** patterns of neural activity; relatively few neurons are active at a time. This allows similar memories to have distinct, **non-overlapping** neural representations. The biggest enemy of memory is interference, and having distinct neural patterns dramatically reduces it.

The brain must have come to a crossroads when evolving: These distributed, overlapping representations of the neocortex are really useful for general learning, but they produce catastrophic interference when they try to encode new knowledge too fast. On the other hand, it is this rapid one-shot encoding that is required for episodic memory. The solution evolution came up with was to leverage **two** specialized complementary learning systems: The **hippocampus** for rapid encoding of new **episodic memories**, and the **neocortex** for slow acquisition of rich webs of **semantic knowledge**. The hippocampus would need non-overalapping encoding and rapid learning rates, while the neocortex would need overlapping encoding and slower learning rates.

Before we oversimplify it too much, we need to remember memory is a highly distributed phenomena. Billions of synapses throughout the brain are tweaked by any given experience. Learning new memories of specific information is possible even in people with significant hippocampal damage. 

An essential aspect to remember is that memory retrieval depends critically on how the brain is probed. We’ve all had the experience of a flood of memories coming back as a result of visiting a childhood place; the myriad of cues available enable recall of memories that otherwise are not quite strong enough to rise to the surface. The memories encoded without the benefit of the hippocampus are weaker and more vague, but they do exist.

In addition to being highly distributed, memory in the brain is also highly interactive. Information that is initially encoded in one part of the brain can influence other parts of the brain, if those memories are reactivated and these other brain areas get the chance to learn them. The classic example of this is that episodic memories initially encoded in the hippocampus can be integrated into the surrounding neocortical areas through repeated retrieval of those memories. This is a big chunk of what goes on while you sleep. Furthermore, influences of the prefrontal cortex can significantly influence the encoding and retrieval of memory. Memory in the brain is a highly dynamic, far from the static “hard drive” metaphor from computers.

# Major Types of Memory

Two neural forms of memory: Activation and Synaptic Changes

Activation: Neurons continue to fire action potentials, "remembering" what you were just seeing, thinking. When the firing stops, you forget. Transient, easily lost, but is very flexible (mental arithmetic, etc.). Fundamental basis of working memory.

Synaptic weight changes: Weight changes as a result of LTP, encodes long-term memory that lasts even after activation switches. Very high capacity, as you have so many synapses. Fundamental basis of long-term memory.

## STM Vs. LTM

Sensory Input -> Sensory Memory --(attention)-> STM --(encoding)-> LTM

1. Sensory Input
2. Sensory memory
    * Activity in sensory processing areas
    * Short-term trace of the sensory input; residual activity (e.g. closing your eyes and still seeing shapes)
    * Loses unattended info
3. STM (short-term memoryl, i.e. working memory)
    * Activity in higher-level areas
    * Semantic representations (e.g. "cat")
    * Need rehearsal to maintain information
    * Loses unrehearsed info
4. LTM (long-term memory)
    * Synaptic changes in hippocampus and slower cortical changes
    * Long-term memory is stored in the cortex; it doesn't have an off-site storage
    * Short-term memory is just the active portion of your long-term memory
    * Hippocampus stores episodic memories, but the knowledge is out there in your cortex
    * Loses info from interference 
    
## Memory in the Brain

The brain IS memory. Memory is located in every single synapse in the brain. This is one of the main differences between brains and computers: neurons have the processing and the memory in the same place, the connections between the neurons. It's not a separate thing like it is in computers.

There's as many different kinds of memory as there are neurons and synapses and brain areas.

Sensory memory is just neural firing in the sensory brain. Short-term memory is neural firing in higher level brain areas that represent the specific thing you're remembering. Long-term memory is everywhere; it's the sum of all the information stored in your synaptic weights. There's no "grandmother cell" for every memory, it's just synaptic weight changes

We're consciously aware of things from our temporal lobe more so than from our parietal lobe due to the temporal lobe housing things that can be easily described by language (in addition to housing language itself).

Tpyes of Memory:
* Episodic memory: events, facts, etc.
      * Hippocampus
* Familiarity-based recognition
      * Perirhinal cortex
* Weight-based priming
      * Subconscious, can be very long-lasting
* Weight-based priming
      * Also subconscious, but transient

## Long-Term Memory

In the classic model, there are two types of long-term memory:

* Explicit (declarative)  memory: Conscious
   * Episodic memory (personal experience)
   * Semantic memory (facts about the world)
* Implicit memory: Not conscious
   * Procedural memory (how to do things)
   * Repetition (improvement from exposure)
   * Priming, conditioning 
   
While this model is intuitive, it's very egocentric. It's another one of these psycology models made be people who don't have a deep understanding of the brain and beleive consciousness is all there is.

## Episodic Memory

Episodic memory is autobiographical memory (life events) and arbitrary new memories (e.g. facts you learn in class). 

If for aribitrary new memories there is more than one pairing, interference can happen. As you start to learn items on the A-C pairing list, you see a systematic amount of interference on the A-B list.

Standard neural networks suffer catastrophic interference, meaning as A-C list is learnt the A-B list is completely forgotten. Parameters need to be changed to fix it.

The fundamental problem is that the same neurons and same synapses are getting re-used to learn about the A-C items as were used to learn the A-B items. The A-B knowledge, stored in the synaptic weights, are getting overwritten. Interference is caused by re-use and overwriting of the old synapses.

The question becomes how do we make the network use different neurons and synapses for new memories? By having fewer active neurons, like we saw in the cerebellum. We could increase the amount of inhibition. 

Really we want to encourage the network to use different neurons. We can increase the strength of the neural pathway, but more importantly we can increase the size of the hidden layer.

Overall solution: Give plenty of room for the network to use different neurons. Increase the size of the hidden layer, increases the sparsity of the neurons that become active.

## The Hippocampus

The hippocampus is the system in charge of our episodic memories.

How does the hippocampus solve the catostrophic interference problem?

The hippocampus has three main subsections: Dentate gyrus (DG), CA3, and CA1. All three of these subsections get their input from the **entorhinal cortex**.

The parietal cortex (dorsal "where" stream) feeds into the parahippo cortex. The IT cortex (ventral "what" stream) feeds into the perirhinal cortex. Both the parahippo and the perirhinal cortex feed bidirectionally into the entorhinal cortex, giving the input to the hippocampus.

The entorhinal cortex feeds into all three subsections of of the hippocampus (impacting memory encoding), but there is a main flow of information. Information enters the DG, where **pattern separation** occurs. The DG feeds uni-directionally into CA3, where **pattern completion** happens. CA3 also feeds back into itself. CA3 feeds uni-directionally into CA1.

[Insert picture]

The key part is the completed pattern in CA1 is able to be unpacked into the corresponding cortical neurons. The DG has the job of separating the memory into unique neurons. The CA3 has the job of storing what's basically a hashcode. CA1 has the job of unpacking that memory into corresponding cortical neurons when recall is needed.

CA1 also connects to both the entorhinal cortex and subiculum, which connects it to subcortical regions tying emotion to the memory.

Sparse firing prevents interference. CA3 has very sparse firing, compared to the entorhinal cortex which has dense firing. People equate this sparse firing to place cells, but in the hippocampus where the firing happens is almost entirely random and does not correspond to spatial locations. They're memories, not maps.



