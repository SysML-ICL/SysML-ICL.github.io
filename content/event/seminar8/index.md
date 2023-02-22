---
title: "Seminar #8 - Roger Waleffe - MariusGNN (EuroSys'23)"

location: Huxley 315 - Imperial College London
#address:
#  postcode: 'Room 145'


summary: "Roger Waleffe will present his work MariusGNN: Training Graph Neural Networks over Billion-Scale Graphs on a Single Machine (EuroSys'23)"
abstract: |
  In this talk, I will present MariusGNN, a system for training Graph Neural Networks (GNNs) on a single machine. Using only one GPU, a machine with 60GB of RAM, and a large SSD, MariusGNN can learn vector representations for all 3.5B nodes (web pages) in the Common Crawl 2012 hyperlink graph containing 128B edges (hyperlinks between pages). 

  To support such billion-scale graphs, MariusGNN utilizes pipelined mini-batch training and the entire memory hierarchy, including disk. This architecture requires MariusGNN to address two main challenges. First, MariusGNN optimizes GNN mini-batch preparation to make it as efficient as possible on a machine with fixed resources. Second, MariusGNN employs techniques to utilize disk storage during training without bottlenecking throughput or hurting model accuracy. This talk will highlight how MariusGNN with one GPU can achieve the same level of model accuracy up to 8x faster than existing industrial systems when they are using up to eight GPUs. By scaling training using disk storage, MariusGNN deployments on billion-scale graphs are up to 64x cheaper in monetary cost than those of the competing systems.


# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: '2023-04-20T14:00:00Z'
date_end: '2023-04-20T15:00:00Z'
all_day: false

# Schedule page publish date (NOT talk date).
publishDate: '2023-02-22T00:00:00Z'

authors: []
profile: false
tags: ['GNN', 'DL Training', 'Pipelining', 'Graphs', 'Big Data', 'GNN Training', 'Graph Neural Network', 'Memory Hierarchy', 'Scale-up']
categories: ['Seminar']

# Is this a featured talk? (true/false)
featured: true

image:
  caption: ''
  focal_point: Right

url_code: ''
url_pdf: 'https://arxiv.org/abs/2202.02365'
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

{{% cta cta_link="https://imperial-ac-uk.zoom.us/j/92338545627?pwd=WUp0OWd5bUJOVno0cXNXM2g2enhMZz09" cta_text="Join Zoom Session!" %}}
{{< center >}}
{{< rawhtml >}}
<a title="Add to Calendar" class="addeventatc" data-id="HM16232967" href="https://www.addevent.com/event/HM16232967" target="_blank">Add to Calendar</a>
	<script type="text/javascript" src="https://cdn.addevent.com/libs/atc/1.6.1/atc.min.js" async defer></script>
{{< /rawhtml >}}
{{< /center >}}

# Speaker Bio
Roger Waleffe is a PhD student at the University of Wisconsin-Madison working under the supervision of Theodoros Rekatsinas. His work focuses on the intersection of systems and algorithmic challenges for IO-aware training of large-scale ML models. Roger is a lead in the Marius project (https://marius-project.org/) which aims to make the use of Graph Neural Networks and Graph Embeddings over billion-scale graphs easier, faster, and cheaper. Roger holds a B.S. and M.S. in computer science from UW-Madison and is a recipient of the UW-Madison departmental graduate research fellowship and Goldwater scholarship.
