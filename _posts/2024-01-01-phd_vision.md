---
layout: distill
title: My PhD Vision
description: A short overview of my PhD PLan
tags: distill formatting
giscus_comments: true
date: 2024-01-01
featured: true

authors:
  - name: Anton Wiehe
    url: "notnanton.github.io"
    affiliations:
      name: AdaLab
      name: PHAROS Labs

# bibliography: 2018-12-22-distill.bib

# Optionally, you can add a table of contents to your post.
# NOTES:
#   - make sure that TOC names match the actual section names
#     for hyperlinks within the post to work correctly.
#   - we may want to automate TOC generation in the future using
#     jekyll-toc plugin (https://github.com/toshimaru/jekyll-toc).
toc:
  - name: Overview
    subsections:
      - name: Goal
      - name: Strategy
  - name: Cognitive Architecture
    subsections:
      - name: Concept
      - name: Individual Modules and Neurological Analogies
      - name: Learning Hierarchies
  - name: Project Ideas
    # if a section has subsections, you can add them as follows:
    # subsections:
    #   - name: Example Child Subsection 1
    #   - name: Example Child Subsection 2
 # - name: Citations
 # - name: Footnotes
 # - name: Code Blocks
 # - name: Interactive Plots
 # - name: Layouts
 # - name: Other Typography?

# Below is an example of injecting additional post-specific styles.
# If you use this post as a template, delete this _styles block.
_styles: >
  .fake-img {
    background: #bbb;
    border: 1px solid rgba(0, 0, 0, 0.1);
    box-shadow: 0 0px 4px rgba(0, 0, 0, 0.1);
    margin-bottom: 12px;
  }
  .fake-img p {
    font-family: monospace;
    color: white;
    text-align: left;
    margin: 12px 0;
    text-align: center;
    font-size: 16px;
  }

---

## Overview

### Goal
An intelligent agent in direct interaction and quick in-context learning. 

### Strategy
Set up cognitive architecture with plan to train it and evolve it.
For PhD: Focus on aspects and study composites in projects.

Concrete Plan:
1. Get suitable testing ground (robot with good simulation, decent grid world)
2. Make overview of AGI architectures/plans (Sutton's Alberta Plan, Schmidhuber's Big Net, Le Cun's JEPA, etc). Write paper summarizing key ingredients, distinctions.
3. Make own plan and describe in detail how modules interact.
4. Work on most promising module. Current promise: meta-learning with adapters and MoE.
5. Select up to 3 modules that can be researched on during the PhD and publish them along with the conjoining architectural plan.

## Cognitive Architecture

### Concept
We define an overall cognitive architecture that achieves the goal. A figure will show up here, illustrating the relationships of the modules.

### Individual Modules and Neurological Analogies
- Policy network(s) - division of network of policy networks responsible for actuator regions but overall connectedness
- Value(feeling) network - output of multi-faceted reward, analogy to control of endorphins
- Intrinsic motivation network(s) - output of rewards for curiosity, pain-avoidance, beauty-seeking, death avoidance.
- Perception Network - produces input of policy network by simulating real world, applies sensory biases to filter out noise and generates internal coherent, multi-modal integration of all senses. Very robust, changes only at short beginning of life and evolutionary.
- Affordance network - (possibly integrated as a conditional mode within the perception network.) Takes in state and intention, produces projected action/series of states/world flow.
- Word model network - strongly connected to possible affordance network. Produces next state

### Learning Hierarchies
Learning at different levels:
1. **Evolutionary**: defines base reactive behavior, main cognitive biases, (basic physical "laws"), architectural improvements. Evolutionary algorithm, guided by epi-genetic variations (e.g. network node stability/importance influences allowed change of weights - See Uber Paper)
2. **Lifelong**: integration of facts, long-term memory, core behavior and automatism. Policy network is trained - maybe by meta-learning over situational episodes.
3. **Situational**: Quick adaption using adapters (LoRAs). Adapters need to be integrateable into network if they are useful enough.


## Project ideas
My **awesome** project ideas in _RL_ and _meta-learning_.

{% details Project 1 %}
Additional details, where math $$ 2x - 1 $$ and `code` is rendered correctly.
{% enddetails %}

(Legend RL=reinforcement-learning, DL=Deep Learning)
1. RL Projects:
⋅⋅*  defining architecture that can think, plan, adapt
⋅⋅*  incorporate knowledge of CLIP or LLMs into agent, using them either as
knowledge base, its token embeddings as latent space to formulate thoughts, or as generalized algorithms that can be abused in contexts where no language is necessary
⋅⋅* RL: put planning steps (interaction path of world model + policy) into LSTM memory to let it "think", then plan new paths and finally decide after planning is done.
⋅⋅*  RL: Hierarchical actor-critic on any domain using quantized/symbolized (VQ-VAE - like) options/sub-tasks
⋅⋅*  ?RL + Meta Learning: define learnability via meta-learning world model
2. Meta learning Projects
3. Other Projcets
⋅⋅*  Meta-learning: divide dataset in clusters, train neural net using MAML on it, clusters as separate "skills", increase granularity of clusters over training time
3. Deep Learning Projects
⋅⋅* DL: learning a training schedule akin to prioritized replay but also focusing on: which samples to reject entirely? Which ones combine well with which other ones to get a clean gradient?
⋅⋅*  DL: training very large models with mostly frozen weights and only train adapters to modify flow
⋅⋅*  DL: train music or video model
⋅⋅*  DL: live-reacting plazmapunk