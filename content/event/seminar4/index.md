---
title: "Seminar #4 - Artem Artemev - Memory Safe Computations with XLA Compiler "

location: Huxley 315 - Imperial College London
#address:
#  postcode: 'Room 145'


summary:  Artem Artemev will present his work on eXLA
abstract: |
  Software packages like TensorFlow and PyTorch are designed to support linear algebra operations, and
  their speed and usability determine their success. However, by prioritising speed, they often neglect memory
  requirements. 

  As a consequence, the implementations of memory-intensive algorithms that are convenient
  in terms of software design can often not be run for large problems due to memory overflows. Memory-
  efficient solutions require complex programming approaches with significant logic outside the computational
  framework. This impairs the adoption and use of such algorithms. To address this, we developed an XLA
  compiler extension that adjusts the computational dataflow representation of an algorithm according to
  a user-specified memory limit.

  We show that k-nearest neighbour and sparse Gaussian process regression
  methods can be run at a much larger scale on a single device, where standard implementations would have
  failed. Our approach leads to better use of hardware resources. We believe that further focus on removing
  memory constraints at a compiler level will widen the range of machine learning methods that can be
  developed in the future.

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: '2022-09-01T10:30:00Z'
date_end: '2022-09-01T11:30:00Z'
all_day: false

# Schedule page publish date (NOT talk date).
publishDate: '2022-08-25T00:00:00Z'

authors: []
profile: false
tags: ['Domain Specific Languages', 'Compilers', 'Dataflow', 'XLA', 'JAX', 'Memory Safety', 'Memory-Efficiency', 'Algorithms']
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

{{% cta cta_link="https://imperial-ac-uk.zoom.us/j/98692000316?pwd=SnBNV21oQ2VGaGJDem51SVRlWG9pZz09" cta_text="Join Zoom Session!" %}}
{{< center >}}
{{< rawhtml >}}
<a title="Add to Calendar" class="addeventatc" data-id="Ji14783117" href="https://www.addevent.com/event/Ji14783117" target="_blank">Add to Calendar</a>
	<script type="text/javascript" src="https://cdn.addevent.com/libs/atc/1.6.1/atc.min.js" async defer></script>
{{< /rawhtml >}}
{{< /center >}}

# Speaker Bio

Artem Artemev is at his second year PhD research in Imperial College London, with Mark van der Wilk as his supervisor. Before starting PhD, Artem has worked as Machine Learning Researcher and Engineer for start-up companies. His primary interest lies in machine learning theory and approximate Bayesian inference, particularly non-parametric machine learning methods like Gaussian processes. His recent work addresses the scalability of Gaussian processes while retaining the predictive properties of that model when approximations are involved.
