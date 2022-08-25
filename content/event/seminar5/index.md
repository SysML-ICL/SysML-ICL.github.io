---
title: "Seminar #5 - Colin Unger - Unity (OSDI'22)"

location: Huxley 315 - Imperial College London
#address:
#  postcode: 'Room 145'


summary: Colin Unger will present his work on Unity (OSDI'22)
abstract: |
  This paper presents Unity, the first system that jointly optimizes algebraic
  transformations and parallelization in distributed DNN training.
  Unity represents both parallelization and algebraic transformations as
  substitutions on a unified parallel computation graph (PCG), which 
  simultaneously expresses the computation, parallelization, and communication
  of a distributed DNN training procedure.
  
  Optimizations, in the form of graph substitutions, are automatically generated
  given a list of operator specifications, and are formally verified correct using
  an automated theorem prover. Unity then uses a novel hierarchical search algorithm
  to jointly optimize algebraic transformations and parallelization while 
  maintaining scalability. The combination of these techniques provides a generic
  and extensible approach to optimizing distributed DNN training, capable of integrating
  new DNN operators, parallelization strategies, and model architectures with
  minimal manual effort.
  
  We evaluate Unity on seven real-world DNNs running on up to 192 GPUs on 32 nodes
  and show that Unity outperforms existing DNN training frameworks by up to 3.6×
  while keeping optimization times under 20 minutes. Unity is available to use
  as part of the open-source DNN training framework FlexFlow at
  [https://github.com/flexflow/flexflow](https://github.com/flexflow/flexflow).

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: '2022-09-08T10:30:00Z'
date_end: '2022-09-08T11:30:00Z'
all_day: false

# Schedule page publish date (NOT talk date).
publishDate: '2022-07-23T00:00:00Z'

authors: []
profile: false
tags: ['Compilers', 'DL Training', 'Pipeline Parallelism', 'Tensor Parallelism', 'Data Parallelism', 'Algebraic Optimization', 'Verification', 'Strategy Search']
categories: ['Seminar']

# Is this a featured talk? (true/false)
featured: true

image:
  caption: ''
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

{{% cta cta_link="https://imperial-ac-uk.zoom.us/j/96569969529?pwd=anprUE80SkFvcFh5ajE4OG45V1J1Zz09" cta_text="Join Zoom Session!" %}}
{{< center >}}
{{< rawhtml >}}
<a title="Add to Calendar" class="addeventatc" data-id="uf14485709" href="https://www.addevent.com/event/uf14485709" target="_blank">Add to Calendar</a>
	<script type="text/javascript" src="https://cdn.addevent.com/libs/atc/1.6.1/atc.min.js" async defer></script>
{{< /rawhtml >}}
{{< /center >}}

# Speaker Bio

Colin Unger is a second year PhD student at Stanford advised by Alex Aiken. He received his bachelor's degree from UC Santa Barbara, where he worked with Giovanni Vigna and Christopher Kruegel on binary analysis. He is broadly interested in compilers, program analysis, and optimization, especially in emerging applications, and is currently focused on hardware-aware optimization of deep learning workloads.
