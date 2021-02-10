---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Multi-manned assembly line balancing"
summary: "Metaheuristics and mixed integer linear models (MILP) for multi-manned assembly line balancing (MALBP)"
authors: []
tags: []
categories: []
date: 2020-05-21T14:07:18+02:00
profile: false  # Show author profile?
commentable: true  # Allow visitors to comment? Supported by the Page, Post, and Docs content types.

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_code: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---


## Introduction to the problem

*This line is developed by PhD student Zikai Zhang and Prof. Tang from the University of Wuhan.*


Finding the best configuration of an assembly line is not trivial and the assembly line balancing problem (ALBP) models how to better balance the tasks of the line in workstations. Concretely, the ALBP aims to optimize some specific objectives such as line efficiency and workload while taking task assignment, precedence relation, and cycle time constraints into account. In this problem, each task must be assigned to only one workstation and is executed after all its predecessors complete. Additionally, the time required by the tasks of each workstation cannot exceed the cycle time.

The *multi-manned assembly line balancing problem (MALBP)* is dedicated to model large-size industries having a high volume of products such as the automotive industry. The MALBP has four advantages over the traditional ALBP: (1) effective reduction of the production line length, (2) effective use of space, (3) increased yield and (4), reduction of the time required for material handling and its setting.


## Supplementary files

{{% staticref "files/benchmark_data_MALBP.zip" "newtab" %}}Benchmark data{{% /staticref %}}







