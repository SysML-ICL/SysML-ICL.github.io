---
title: "Reading Group Session #1"

location: Huxley 217 - Imperial College London
#address:
#  postcode: 'Room 145'

summary: vPipe (TPDS'21) & Alpa (OSDI'22)
abstract: "We discuss two recent works focused on distributed DL training. vPipe is a virtualized memory manager for pipeline parallel training. Alpa is a runtime capable of autoparallelization of large deep networks."

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: '2022-06-09T10:30:00Z'
date_end: '2022-06-09T11:30:00Z'
all_day: false

# Schedule page publish date (NOT talk date).
publishDate: '2022-06-06T00:00:00Z'

authors: []
profile: false
tags: ["DL Training", "Memory Management", "Distributed", "Compilers", "Auto-parallelization"]
categories: ['Reading Group']

# Is this a featured talk? (true/false)
featured: true

image:
  caption: 'Image credit: [**Google AI**](https://ai.googleblog.com/2022/05/alpa-automated-model-parallel-deep.html)'
  focal_point: Center

header:
  image: "featured.png"
  caption: 'Image credit: [**Google AI**](https://ai.googleblog.com/2022/05/alpa-automated-model-parallel-deep.html)'

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

# Papers
Papers covered will be: 
1. [vPipe: A Virtualized Acceleration System for Achieving Efficient and Scalable Pipeline Parallel DNN Training](https://ieeexplore.ieee.org/iel7/71/9497774/09472938.pdf), TPDS'21
2. [Alpa: Automating Inter-and Intra-Operator Parallelism for Distributed Deep Learning](https://arxiv.org/pdf/2201.12023), OSDI'22


# Discussion Notes

In these discussion notes we attempt to summarize points made during the discussion on possible future directions.

## vPipe

### Online partitioning

vPipes justification for the need for an online repartitioning algorithm is Neural Architecture Search (NAS).
Very few systems are using online partitioning nowadays. The question is, is there a need for them?
What are other motivating reasons for online partitioning?
- To deal with failures
- To support elasticity
- NAS 
- Dynamic networks

In short, any source of dynamism in the training is justifiable.
What are other sources of dynamism in training?

### PCIe Usage

In vPipe PCIe is shared by swapping and inter-host activation communication.
The algorithm which decides the swap-recompute plan attempts to fill all the PCIe bandwidth but ignores activation communication traffic.
Is this optimal? Won't this cause stalls by oversubscribing the PCIe bus?
Still, vPipe prioritizes inter-host activation communication.


## Alpa

### Device Meshes

Alpa maps computations to a 2D mesh of devices. This seems to be due to the fact
that there are 2 layers in the device hierarchy, intra-host and inter-host,
where communication intra-host is faster than inter-host.
If there were a third level in this hierarchy, perhaps a 3D mesh of devices would make sense.

## Both papers

We noticed that both papers attempt to solve the NP-Complete task of parallelizing
a computational graph across several devices for optimal performance.
This task is too difficult to solve directly.
To tackle this, both papers use a decomposition approach, instead solving two subproblems optimally:
- Alpa first uses inter-op parallelism, then intra-op parallelism on each stage.
- vPipe first uses inter-op parallelism, then computes a swap/recompute plan for each stage.

Why can't it be solved directly? Is it simply too large a search problem?
Are we losing something by not solving the original problem optimally?

### Heterogeneous Clusters

Heterogeneous clusters are a reality in several organizations which over time accumulate several generations of accelerators.
Furthermore, CPUs are a largely unused resource that is available.
Both papers, and other systems, generally target homogeneous clusters only.
We believe there is space for novel systems targeting Heterogeneous clusters, though the problem of partitioning and parallelizing becomes more difficult.

