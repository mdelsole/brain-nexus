---
layout: page
status: publish
published: true
title: 'Motor'
date: '2011-05-12 19:21:49 +0200'
date_gmt: '2011-05-12 19:21:49 +0200'
categories: []
order: 35
tags: []
---

* TOC
{:toc}

For motor control, our brain uses two core primitive systems: The **basal ganglia** (BG) and the **cerebellum**. 

Each region responds to two basic forms of learning: **reward** and **error**. These two sources of learning are what you need for core survival in the wild.

The hippocampus and neocortex are more advanced systems, with the BG and cerebellum being core older systems.

People say the BG is a motor system, but it's more accurate to say that it's a decision making and reinforcement learning system. It's about deciding what you want to do, which of course is liinked to motor control.

The cerebellum supports predictive learning. It's the core motor control system, while the BG is the higher-level "outer-loop" of "what should I do".

Both of these systems work by using "separator" systems. The cerebellum works by taking the information they learn and memorizing each particular case by separating it and encoding it into unique engrams. The cerebllum memorizes for each possible configuration of the motor system what the right command is, in a look-up table of sorts. The BG not quite as much to the same extent, but the cerebellum does do this separation religously. Even if two patterns have overlap in the cortex, they will be distinct patterns in the cerebellum.

The hippocampus has a similar mechanism, which we'll talk about later.

## Summary 
Cerebellum contains unique engrams of the right command for each situation of the motor system (why it has half the neurons in the brain). The BG is an outer-loop, in charge of determining what action to take.

# Cerebellum

The cerebellum is an extremely stereotyped circuit that is repeated over and over again. 

The cerebellum has half of the neurons in the brain. Most of these neurons are **granule cells**. They get activated by the processed sensory information from other brain regions. It gets separated out by having many, many different possible granule cells that could represent it. These granule cells are all competing in an inhibitory way, ensuring a very different combination of granule cells is active for every different combination of information coming in.

If you have a lot of inhibition, then only a few can get active, and it's very unlikely that the sparse patterns of output will overlap for different sensory inputs.

The granule cells feed into purkinje cells. These cells receive up to 100,000 synapses from granule cells into a singl purkinje cell. They sample a hug range of granule cells.

The idea is that the information is getting blown-up into a very high-dimensional space in the granule cell layer, and it's the job of the purkinje cell to collapse that information space back into the original lower dimensional space that's important for motor control. The purkinje cells relate to specific muscle fibers. 

The cerebellum is transforming the sensory inputs it gets in great abundance, then transforming them into this motor coordinate system, which is the output of the purkinje cells that feeds into actual motor control.

The cerebellum is fundamentally a motor system. There are some cognitive contributions, but the vast majority is for motor.

The other important part is the presence of climbing fibers. These fibers wrap around the purkinje cells and provide the learning signal for the cerebllum. It's an **error** signal that tells the cerebullum when an error has been made (delta-rule error learning)

The changes it makes is akin to a **support vector machine**. [insert explanation of SVM]. In 2D, it might be difficult to fully separate patterns. But as you add more and more dimensions, it gets easier to find a way to separate them. 

This is what the cerebellum accomplishes by blowing up the dimensionality with granule cells. It allows you to learn a function that does one thing with one pattern and another thing with another pattern. These patterns might overlap a lot in low dimensionality (small amounts of granule cells), but in higher dimensionality it's much easier to get distinct patterns.

The cerebellum, unlike the neocortex, is a feed-forward circuit. Input (PN) -> granules -> purkinje -> output (DCN). There is no recurrent connectivity (a recurring theme with the early brain systems), and thus no attractor dynamics.

When an error occurs, it is associated with the inputs that happened about 100 ms earlier. Importantly, the purkinje cells try to anticipate the error before it happens, and so the pattern that gets corrected "100 ms prior" is the one happening in the present. The purkinje cells try to anticipate an error, then correct the error before it happens using the error signals.

There's a motor plan of 'what we want the system to end up in' produced by the cortex, a target for the overall muscle position we're trying the achieve. The details are tuned and shaped by the cerebellum, while the plan is maintained by the cortex.

Each granule cell becomes tuned to a particular random muscle state represented by the cortex.

If we implement a self-inhibition so that the cells turn off after a short period of time, it allows a new cell to become active (presumably the next muscle state), and gives the system a much finer temporal resolution. Each engram (collection of active cells) is a discrete state, so the system must transition to the next engram rapidly in order to create smooth movement, otherwise you'll just be stuck in that muscle state.

The purkinje cells take in a ton of granule cells, recollapsing the information into reasonable dimensionality. The inferior olivary signal is produced when the system experiences an error (e.g. an overshoot of the hand grabbing an apple). Once the error is *increasing over time*, that's when we know there's an error. When the error is detected in the future, the purkinje cells will decreaase their connection strength with the granule cells from 100 ms earlier.

In the cerebellum, learning is mostly a decrease in weights rather than an increase. Additionally, it's mostly disinhibiting rather than exciting.

## Summary:
Order of operations:
Mossy fiber (sensory inputs) -> Granule cells (high-dimensional encoding, pattern separation) -> Purkinje cells -> Motor outputs

The cerebellum is a feedforward circuit. It receives processed sensory input from the cortex via mossy fibers. These activate granule cells, which are an extremely large set of cells the perform pattern separation, blowing up the input into high-dimensionality and randomly grabbing a non-overlapping subset. The granule cells feed into purkinje cells, which collapse the dimensionality back down to a reasonable level and trigger specific motor neurons.

# Basal Ganglia

The basal ganglia acts as a wall, blocking possible actions that the cerebral cortex is coming up with of things we could do, picking only one (usually the most rewarding). It's an integrated system; you need the cortex to come up with the possible actions, and the basal ganglia to choose.

You become consciously aware of the basal ganglia's decision 300 ms after the fact. This is what we mean when we say you become aware of the decision after it's already been made. It is still "you" making the decision, just a different part of you. The basal ganglia is feedforward, not having a recurrent component that we think is critical for consciousness.

The basal ganglia has to competing pathways: "Go" and "no-go". There are separate neurons in the no-go and go pathways.

The dopamine system is wired so that it reinforces the "go" pathway. If you make a go decision and the outcome is positive, you get a positive dopamine signal and reinforce the go pathway. A negative dopamine signal (decrease) reinforces the "no-go" pathway.

## Action Selection

There are 5 core loops of the basal ganglia. All of them are essentially the same, but control action selection of 5 different areas.

The loops have 3 parts: One in the cortex, one in the striatum, and one in the thalamus.

The first 2 loops are centered around actions

**Loop 1: Motor**. Interestingly, the motor loop is with the secondary motor area, not the primary motor area. It's not interested in the fine grain detail, just "what should I do".

**Loop 2: Occulumotor** (where you're going to look)

The second 3 loops are centered around goals.

**Loop 3: Prefrontal** (plans). The most expanded part in humans

**Loop 4: Orbitalfrontal** (value, outcomes). Encodes how valuable things are

**Loop 5: Cingulate** (utility). Intermediating between desired outcomes of the orbitofrontal cortex and the plans, the ways of getting those outcomes. Considers the costs and feasability of the plan vs. the outcome.

Motor/Occulumotor <-|-> Prefrontal <--> Cingulate <--> Orbitalfrontal

Many parts of your decision making are informed by subcortical inputs. In fact the medial frontal area of the cortex has a whole map of values. Its subcortical regions represent many different factors:

* SMA: Proximal actions (next few secs)
* pdACC: Associated values
* rdACC: Associated values, integrates vm inputs
* dlPFC: Broad action plans, strategies
* pgACC: Arousal, drive
* sgACC: Active avoidance (negative outcomes)
* mOFC: Active approach (positive outcomes); appetitive, consumative
    * Integrated with IOFC taste areas (abstract "I like this taste") 
* rmPFC: Episodic affective context <--> hippocampus, considering past and future alternatives
* IOFC: Sensory-driven values ("what" "I like")
* vlPFC: WM and control over sensory ("what")

In general, the PFC areas encode what plan is going to be taken, and the ACC area it is connected to enocodes the effort assoicated with that and whether it is worth it

## The BG Disinhibitory Circuit
