---
title: "Seminar #6 - Michael Kuchnik - Plumber (MLSys'22)"

location: Huxley 315 - Imperial College London
#address:
#  postcode: 'Room 145'


summary: Michael Kuchnik will present his work on Plumber (MLSys'22)
abstract: |
  Input pipelines, which ingest and transform input data, are an essential part of training Machine Learning (ML) models.
  However, it is challenging to implement efficient input pipelines, as it requires reasoning about parallelism, asynchrony, and variability in fine-grained profiling information.
  Our analysis of over two million ML jobs in Google datacenters reveals that a significant fraction of model training jobs could benefit from faster input data pipelines.
  At the same time, our analysis indicates that most jobs do not saturate host hardware, pointing in the direction of software-based bottlenecks.

  Motivated by these findings, we propose Plumber, a tool for finding bottlenecks in ML input pipelines.
  Plumber uses an extensible and interpretable operational analysis analytical model to automatically tune parallelism, prefetching, and caching under host resource constraints.
  Across five representative ML pipelines, Plumber obtains speedups of up to 47x for misconfigured pipelines.
  By automating caching, Plumber obtains end-to-end speedups of over 50% compared to state-of-the-art tuners.


# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: '2022-010-13T14:00:00Z'
date_end: '2022-010-13T15:00:00Z'
all_day: false

# Schedule page publish date (NOT talk date).
publishDate: '2022-09-15T00:00:00Z'

authors: []
profile: false
tags: ['DL Training', 'Input Pipelines', 'Optimization', 'Analytical Modelling', 'Data Parallelism']
categories: ['Seminar']

# Is this a featured talk? (true/false)
featured: false

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

{{% cta cta_link="https://us02web.zoom.us/j/85119887982?pwd=dU9udXRoc1lJNEhQR2xwOVN3SEJxZz09" cta_text="Join Zoom Session!" %}}
{{< center >}}
{{< rawhtml >}}
<a title="Add to Calendar" class="addeventatc" data-id="MF14974081" href="https://www.addevent.com/event/MF14974081" target="_blank">Add to Calendar</a>
	<script type="text/javascript" src="https://cdn.addevent.com/libs/atc/1.6.1/atc.min.js" async defer></script>
{{< /rawhtml >}}
{{< /center >}}

# Speaker Bio

Michael is a final year PhD student in the Computer Science Department of Carnegie Mellon University advised by George Amvrosiadis and Virginia Smith. He received his bachelor's degree from Georgia Institute of Technology, and his research was supported by an NDSEG fellowship. He is broadly interested in computer systems and is currently working on systems for machine learning, with a particular emphasis on data pipelines (e.g., data augmentations, I/O formats, and pipeline design).

