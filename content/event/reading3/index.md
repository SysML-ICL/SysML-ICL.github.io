---
title: "Reading Group Session #3"

location: Huxley 315 - Imperial College London
#address:
#  postcode: 'Room 145'

summary: "Pathways: Asynchronous distributed dataflow for ML (MLSys'22)"
abstract: "Marcel Wagenlander presents Pathways, a new large scale orchestration layer for accelerators using a sharded dataflow graph of asynchronous operators outputting futures."

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: '2023-01-19T14:00:00Z'
date_end: '2023-01-19T15:00:00Z'
all_day: false

# Schedule page publish date (NOT talk date).
publishDate: '2023-01-10T00:00:00Z'

authors: []
profile: false
tags: ["Dataflow", "Distributed", "Asynchronous", "DL Training", "Accelerators", "Gang-Scheduling", "Networking", "SPMD", "Pipeline Parallelism", "Data Parallelism", "Model Parallelism", "TPU"]
categories: ['Reading Group']

# Is this a featured talk? (true/false)
featured: false

image:
  caption: 'Image credit: [**Pathways Paper**](./featured.png)'
  focal_point: Center

header:
  image: "featured.png"
  caption: 'Image credit: [**Pathways Paper**](./featured.png)'

url_code: ''
url_pdf: 'https://proceedings.mlsys.org/paper/2022/hash/98dce83da57b0395e163467c9dae521b-Abstract.html'
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



# <h5 style="text-align: center;">Share</h5>
---
# Pathways

{{% cta cta_link="https://us02web.zoom.us/j/85119887982?pwd=dU9udXRoc1lJNEhQR2xwOVN3SEJxZz09" cta_text="Join Zoom Session!" %}}

[Paper Link](https://proceedings.mlsys.org/paper/2022/hash/98dce83da57b0395e163467c9dae521b-Abstract.html), SysML'22

**Paper Abstract:**

We present the design of a new large scale orchestration layer for accelerators. Our system, Pathways, is explicitly designed to enable exploration of new systems and ML research ideas, while retaining state of the art performance for current models. Pathways uses a sharded dataflow graph of asynchronous operators that consume and produce futures, and efficiently gang-schedules heterogeneous parallel computations on thousands of accelerators while coordinating data transfers over their dedicated interconnects. Pathways makes use of a novel asynchronous distributed dataflow design that lets the control plane execute in parallel despite dependencies in the data plane. This design, with careful engineering, allows Pathways to adopt a single-controller model that makes it easier to express complex new parallelism patterns. We demonstrate that Pathways can achieve performance parity (~100% accelerator utilization) with state-of-the-art systems when running SPMD computations over 2048 TPUs, while also delivering throughput comparable to the SPMD case for Transformer models that are pipelined across 16 stages, or sharded across two islands of accelerators connected over a data center network.


# Discussion Notes

TBD
