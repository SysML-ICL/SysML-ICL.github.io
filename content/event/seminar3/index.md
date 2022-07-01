---
title: "Seminar #3 - Abhinav Jangda - CoCoNet (ASPLOS'22)"

location: Huxley 315 - Imperial College London
#address:
#  postcode: 'Room 145'


summary: Abhinav Jangda will present his work on CoCoNet (ASPLOS'22)
abstract: |
  Recent trends towards large machine learning models require both
  training and inference tasks to be distributed. Considering the huge
  cost of training these models, it is imperative to unlock optimizations
  in computation and communication to obtain best performance. However,
  the current logical separation between computation and communication
  kernels in machine learning frameworks misses optimization
  opportunities across this barrier. Breaking this abstraction can
  provide many optimizations to improve the performance of distributed
  workloads. However, manually applying these optimizations requires
  modifying the underlying computation and communication libraries for
  each scenario, which is both time consuming and error-prone.
  
  In this talk, I will present CoCoNet, which is a domain specific
  language to express a distributed machine learning program in the form
  of computation and communication operations.
  CoCoNet provides several a set of semantics preserving transformations
  that jointly optimizes communication and computation workloads. 
  I will also present how we used CoCoNet to significantly optimize data-
  , model- and pipeline-parallel workloads in large language models with
  only a few lines of code.

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: '2022-07-28T10:30:00Z'
date_end: '2022-07-28T11:30:00Z'
all_day: false

# Schedule page publish date (NOT talk date).
publishDate: '2022-06-21T00:00:00Z'

authors: []
profile: false
tags: ['Domain Specific Languages', 'Compilers', 'DL Training', 'Communication', 'Optimization', 'Stencil Computations', 'Pipeline Parallelism', 'Tensor Parallelism', 'Data Parallelism', 'MPI', 'Collective Communication']
categories: ['Seminar']

# Is this a featured talk? (true/false)
featured: true

image:
  caption: 'Image credit: [**CoCoNet Paper**](https://dl.acm.org/doi/pdf/10.1145/3503222.3507778)'
  focal_point: Right

url_code: ''
url_pdf: ''
url_slides: ''
url_video: ''

# Markdown Slides (optional).
#   Associate this talk with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides:

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects:
---

{{% cta cta_link="https://teams.microsoft.com/l/meetup-join/19%3aLiP6Evh3ssJQ3g41q8vAsBNwwOFTzp7d_qq1y7oTo7A1%40thread.tacv2/1654597085925?context=%7b%22Tid%22%3a%222b897507-ee8c-4575-830b-4f8267c3d307%22%2c%22Oid%22%3a%228d261fd5-be8f-44eb-b630-d5b230fc5ec3%22%7d" cta_text="Join Session!" %}}

# Speaker Bio

Abhinav Jangda is a PhD student at the University of Massachusetts
Amherst and will join Microsoft Research in Fall 2022. His research
focuses on developing programming language abstractions and compilation
techniques to help programmers leverage large scale systems
efficiently. His work was invited for an article in USENIX :login;, has
received an ACM SIGPLAN Distinguished Paper Award at OOPSLA, and a Best
Paper Award at PACT.

