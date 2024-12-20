---
# Leave the homepage title empty to use the site title
title: "Bingnan Huo's Website"
date: 2024-12-11
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/cv.pdf
    design:
      css_class: dark
      background:
        color: black
        image:
          # Add your image background to `assets/media/`.
          filename: stacked-peaks.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false

  # RESEARCH OVERVIEW
  - block: markdown
    content:
      title: '🤖 Research Overview'
      subtitle: ''
      text: |-
        I am a masters student in Data Science at Brown University, where I am part of the [Intelligent Robotics Lab](http://irl.cs.brown.edu/) led by [Prof. George Konidaris](https://cs.brown.edu/people/gdk/). My research focuses on developing intelligent robotic systems that can learn and adapt to solve complex real-world tasks.

        Currently, I am working on:
        - Option generalization under Hierarchical Reinforcement Learning framework for learning reusable robotic skills
        - Applying transferable subgoals with motion planning for skill generalization across tasks using the Franka Emika Panda robot
        - Developing novel approaches for learning transferable subgoals as option termination classifiers (ICLR 2025 submission)

        Previously at Bucknell University, I worked on medical image processing using computer vision and machine learning, developing a system for diagnosing Facial Nerve Paralysis with over 80% accuracy.

        I am actively seeking collaborations in reinforcement learning, robotics, and AI. Feel free to reach out! 📫
    design:
      columns: '1'

  # Featured Publications
  - block: collection
    id: papers
    content:
      title: Featured Publications
      text: |-
        Recent research work in reinforcement learning, robotics, and machine learning.
      filters:
        folders:
          - publication
        featured_only: true
    design:
      view: article-grid
      columns: 2

  # ALL PUBLICATIONS
  - block: collection
    content:
      title: All Publications
      text: |-
        {{% callout note %}}
        [Filter publications](./publication/)
        {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: citation

  #- block: collection
  #  id: talks
  #  content:
  #    title: Recent & Upcoming Talks
  #    filters:
  #      folders:
  #        - event
  #  design:
  #    view: article-grid
  #    columns: 1
  
  # NEWS
  - block: collection
    id: news
    content:
      title: Recent News
      subtitle: ''
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: post
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: date-title-summary
      # Reduce spacing
      spacing:
        padding: [0, 0, 0, 0]
---
