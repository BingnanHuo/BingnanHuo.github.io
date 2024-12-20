---
title: "Learning Transferable Sub-goals by Hypothesizing Generalizing Features"
authors:
- Anita De Mello Koch
- Akhil Bagaria
- Bingnan Huo
- Cameron Allen
- Zhiyuan Zhou
- George Konidaris
date: 2024-10-01
doi: ""

publishDate: 2024-10-01

publication_types: ["1"]

publication: "International Conference on Learning Representations"
publication_short: "ICLR"

abstract: |
  Transfer is a key promise of hierarchical reinforcement learning, but requires first learning transferable skills. For an agent to effectively transfer a skill it must identify features that generalize and define the skill over this subset. However, this task is under-specified from a single context as the agent has no prior knowledge of what future tasks may be introduced. Since successful transfer requires a skill to reliably achieve a sub-goal from different states, we focus our attention on ensuring sub-goals are represented in a transferable way. For each sub-goal, we train an ensemble of classifiers while explicitly incentivizing them to use minimally overlapping features. Each ensemble member represents a unique hypothesis about the transferable features of a sub-goal that the agent can use to learn a skill in previously unseen portions of the environment. Environment reward then determines which hypothesis is most transferable for the given task, based on the intuition that useful sub-goals lead to better reward maximization. We apply these reusable sub-goals to MiniGrid and Montezuma's Revenge, allowing us to learn previously defined skills in unseen parts of the state-space.

summary: We use a diverse ensemble to generalize a given sub-goal to relearn previously discovered skills.

tags:
- Reinforcement Learning
- Feature Learning
- Transfer Learning
- Hierarchical Reinforcement Learning
- Skill Learning

featured: true

links:
- name: Lab
  url: http://irl.cs.brown.edu/
url_pdf: 'paper.pdf'
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''
---