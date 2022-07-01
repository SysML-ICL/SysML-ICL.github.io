---
title: "Seminar #2 - Alexander Renz-Wieland - NuPS (SIGMOD'22)"

location: Huxley 315 - Imperial College London
#address:
#  postcode: 'Room 145'


summary: Alexander Renz-Wieland will present his work on Adaptive Parameter Servers and NuPS (SIGMOD'22)
abstract: |
  To keep up with increasing dataset sizes and model complexity, distributed
training has become a necessity for large machine learning tasks. Parameter
servers (PSs) ease the implementation of distributed parameter management, but
can induce severe communication overhead. In some cases, distributed performance
may even fall behind that of single node baselines. In this talk, I present our
work on making PSs more communication-efficient by adapting to the underlying
workload. I discuss (i) how PSs can adapt parameter allocation dynamically to
exploit access locality, (ii) how PSs can tailor their management techniques to
individual parameters, and (iii) how PSs can do this adaptation automatically,
without requiring tuning. Experimentally, such adaptation drastically improved
PS efficiency, resulting in near-linear speed-ups over single node baselines. 

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: '2022-07-28T10:30:00Z'
date_end: '2022-07-28T11:30:00Z'
all_day: false

# Schedule page publish date (NOT talk date).
publishDate: '2022-06-21T00:00:00Z'

authors: []
profile: false
tags: ['Parameter Servers', 'DL Training', 'Parameter Management', 'Sampling', 'Skew', 'Non-uniform Parameter Access']
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

{{% cta cta_link="https://teams.microsoft.com/l/meetup-join/19%3aLiP6Evh3ssJQ3g41q8vAsBNwwOFTzp7d_qq1y7oTo7A1%40thread.tacv2/1654597085925?context=%7b%22Tid%22%3a%222b897507-ee8c-4575-830b-4f8267c3d307%22%2c%22Oid%22%3a%228d261fd5-be8f-44eb-b630-d5b230fc5ec3%22%7d" cta_text="Join Session!" %}}

# Speaker Bio

Alexander Renz-Wieland is a PhD student working on large-scale machine learning
student in the Database Systems and Information Management (DIMA) group at
Technische Universität Berlin since September 2017. He is supervised by Volker
Markl and Rainer Gemulla (Universität Mannheim). Prior to his PhD, he completed
a M. Sc. Business Informatics with a specialization in Data and Web Science at
Universität Mannheim, with a semester at VU Amsterdam (with courses from CWI).
In his Master's thesis, he worked on scalable sequential pattern mining.

---

<h5 style="text-align: center;">Share</h5>
