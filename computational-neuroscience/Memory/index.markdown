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

# Episodic Memory

The reason most people think of episodic memory when thinking of memory is because it's such a big part of our conscious lives. Everyone with a functioning hippocampus has this remarkable “tape recorder” constantly encoding everything that happens during their lives. We don’t have to use lots of effort to recall what happened 20 minutes or a few hours ago, it's just automatically there. 

Most people end up forgetting the vast majority of the daily events of our lives. In general, we retain only the particularly noticeable or meaningful events. However, a small amount of people have exceptional memory, called **hyperthymesia**. It is *not* the hippocampus itself that differentiates these people, but rather the **obsessive rehearsal and retrieval** of episodic memories. People with hyperthymesia have areas of their **basal ganglia** enlarged (a feature which is associated with OCD). We’ll see in the executive chapter that the basal ganglia participate not only in motor control and reinforcement learning, but also the reinforcement of **updating** and **maintenance** of active memory. 

In normal human brains, the hippocampus has the raw ability to encode and remember every moment of our lives in great clarity. But, most people just don’t bother to rehearse these memories to the point where they can all be reliably retrieved. When you encounter a situation that you give extreme attention to, you'll find yourself playing it over and over in your head after the event has ended. This is your brain recording the event, making sure the memory is strong so it can't be lost.

## Principles of the Hippocampus

Why is the hippocampus necessary? And what makes it so good at episodic memory? 

To answer the first question, we look at the failure of a “generic” cortical neural network model. It can not exhibit any kind of useful episodic memory ability. 

This failure was first documented using a generic backpropagation network trained on the AB-AC paired associate list learning task. This task involves learning an initial list of arbitrary word pairs, called the AB list. For example:
* locomotive - dishtowel
* window - reason
* bicycle - tree
People are tested on their ability to recall the B associate for each A item. Training on the AB list ends when they achieve perfect recall. Then, they start learning the AC list, which involves new associates for the previous A items:
* locomotive - cloud
* window - book
* bicycle - couch 
After a few iterations of learning this AC list, people are tested on their ability to recall the original AB items. The results show that there is a significant amount of **interference** on the AB list as a result of learning the AC items, due to the considerable overlap between the two lists. 

In people, even after several iterations through the AC items, we can still recall about 50% of the AB list. In contrast, the network model exhibits **catastrophic interference**; performance on the AB list went to **0%** immediately. 

Ressearchers may have jumped ship a bit too quickly, because they concluded that this invalidated all neural network models of human cognition, since obviously people have much better episodic memory abilities. Fortunately this kind of whole-sale abandonment of neural networks is unjustified. Indeed, there are certain **network parameters** that reduce the levels of interference. The problem is, changing these parameters makes the general cortical network not work as well. This is where the hippocampus comes in: The hippocampal system is an **additional** neural network with its parameters different than the cortex.

The most important parameter manipulation required is to **increase** the level of **inhibition** so that fewer neurons are active. This greatly **reduces the overlap** between the internal representation of the AB and AC list items, thus allowing the system to learn AC without overwriting the prior AB memories. The hippocampal system exploits this inhibition trick to an extreme degree, allowing it to make distinct, non-overlapping memory engrams.

## Pattern Separation

The hippocampus is specifically optimized to rapidly record episodic memories using **highly sparse** representations (few neurons active at a time). The idea is this minimizes overlap and thus interference. This principle is called **pattern separation**. 

### Hippocampus Anatomy

The anatomy of the hippocampus and the areas that feed into it is shown below. The hippocampus is one of two **summits** on top of the hierarchy of cortical areas (from the bottom sensory input areas like V1 to the top semantic areas like IT). The other summit is the prefrontal cortex, explored in the executive chapter. 

Indeed, the input to the hippocampus neural netowrk is proccessed semantic knowledge from IT (ventral stream) and the parietal cortex (dorsal stream). Thus, it possesses a critical feature for episodic memory: access to a **high-level summary** of everything important going on at the moment. The ventral streams feeds into the **perirhinal** cortex (PRC), while the dorsal stream feeds into the **parahippocampal** area (PHC). These two areas then feed into the **entorhinal** cortex (EC), which serves as the input to the hippocampus itself. 

The major hippocampal areas include the **dentate gyrus** (DG) and the areas of **cornu ammonis** (CA) **CA3** and **CA1**. CA2 turns out to be the same as CA3, so we lump it in. All of these strange names have to do with the shapes of these areas, including the term “hippocampus” itself, which refers to its seahorse shape.

The basic episodic memory encoding story goes like this:
* The high-level summary of everything in the brain is activated in EC, which then drives the DG and CA3 areas via the **perforant pathway**. The end result of this is a highly sparse, **distinct** pattern of neural firing in **CA3**, which represents the main **“engram”** in the hippocampus. 
* The EC also drives activity in CA1, which is in charge of being able to **re-activate** this same EC pattern all by itself.
* These patterns of activity then drive **synaptic plasticity** (learning) in all the interconnected synapses, most importantly in the synaptic connections among CA3 neurons in the CA3 recurrent pathway, as well as the connections between CA3 and CA1 (the Schaffer collateral pathway). 
* These plastic changes effectively **“glue together”** the different neurons in the CA3 engram, and associate them with the CA1 invertible pattern, so that subsequent retrieval of the CA3 engram can then activate the CA1, then EC, and back out to the cortex. 

Thus, the primary function of the hippocampus is to **bind together** all the separate elements of an episode, and then be able to retrieve this conjunctive memory and reinstate it out into the cortex during recall. This is how a memory comes to you; it floods back from CA3 to CA1 to EC to cortex, reactivating something approximating the original brain pattern at the time the memory was encoded. The memory is stored in CA3, and CA1 neurons act as "pointers" from the hippocampal neurons to the cortical neurons that *actually* make up the memory. Technically, hippocampal neurons have no meaning to "you".

[insert picture]

The system is a lot to take in. A quick symmary before moving on:
* The semantic summary of what's currently going on converges into EC
* EC drives DG and CA3 to form a distinct set of neurons dedicated to this memory's engram
* EC also drives CA1 at the same time, forming the connections that will be needed trace this memory engram to its corresponding cortical neurons 

EC driving activity causes synaptic plasticity (since this is still a neural network). This binds together the CA3 neurons, forming the engram, via the CA3 recurrent pathway. It also binds the CA1 neurons to the respective CA3 neurons, as well as to the respective EC neurons, forming the path from CA3 to CA1 to EC for memory recall. If there could ever be considered a "memory bank" of the brain, CA3 is it.

The synaptic changes all the way through the cortical pathways into and out of the hippocampus “greases” the retrieval process. Indeed, if a memory pattern is reactivated frequently, then these cortical connections can be strong enough to drive reactivation of the full memory, without the benefit of the hippocampus at all. We discuss this **consolidation** process in detail soon. Finally, the retrieval process can be enhanced by **controlled retrieval** of memory using top-down strategies using the **prefrontal cortex**. I still need to write stuff on controlled retrieval here, but it depends on a combination of activation and weight based memory analogous to some features we will explore in executive Chapter.

## Hippocampal Neurons: Sparseness, Pattern Separation

It is clear that CA3 and CA1 neurons fire much less often than those in the cortex (entorhinal cortex and subiculum). This is what we mean by **sparseness** in the hippocampal representation: for any given episode, only a relatively few neurons are firing. Furthermore, each neuron only fires under a very specific circumstance. 

We first noticed this firing behavior in rats. Yes, rats have a "hippocampus", but its not like our hippocampus at all; the firing of neurons in rats tends to be identifiable as spatial locations. The rat hippocampus is home to **place cells** that map out where the rat is according to the canvas made up of **grid cells**. This however is not generally true of primate hippocampus, as ours are much more random.

This sparseness results from **high levels of GABA inhibition**. It keeps many neurons below threshold, as well as requires neurons to receive a high level of excitatory input to overcome this inhibition. It must get *really* activated to overcome the inihibition. 

The direct benefit of this sparseness is that the engrams for different episodes won't overlap almost ever, just from basic probabilities. For example, the probability of a neuron being active for a given episode in DG is typically 1%. Then, the probability for any two random episodes is that value squared, which is .01%. In comparison, if the probability is higher like 25% (typical of cortex), then there is a 6.25% chance of overlap for two episodes.

The connection between activity levels and pattern separation can also be observed within the hippocampus itself, by comparing the firing properties of DG vs. CA3 neurons. DG neurons have the sparsest activity levels (1%), even compared to the less sparse CA3 (2-5% activity level). The DG exhibits more pattern separation than the CA3.

Another factor that contributes to effective pattern separation is the broad and diffuse connectivity from EC to DG and CA3, via the **perforant pathway**. This allows many different features in EC to be randomly combined in DG and CA3, enabling them to be sensitive to combinations or conjunctions of inputs. Because of the high inhibitory threshold associated with sparse activations, this means a given neuron in these areas must receive significant excitation from multiple of these diffuse input sources. In other words, these neurons have **conjunctive representations**; all features must be present for the neuron to become active.

Pattern separation is important for enabling the hippocampus to rapidly encode novel episodes with a minimum of interference on prior learning, because the patterns of neurons involved overlap relatively little.

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



