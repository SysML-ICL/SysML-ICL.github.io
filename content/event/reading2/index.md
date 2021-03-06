---
title: "Reading Group Session #2"

location: Huxley 315 - Imperial College London
#address:
#  postcode: 'Room 145'

summary: Gato (arXiv'22)
abstract: "We discuss Gato, a new generalist model and its implications for systems designers."

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: '2022-06-23T10:30:00Z'
date_end: '2022-06-23T11:30:00Z'
all_day: false

# Schedule page publish date (NOT talk date).
publishDate: '2022-06-19T00:00:00Z'

authors: []
profile: false
tags: ["Transformers", "DL Training", "Multi-Modal", "Multi-Task", "AGI", "Embeddings"]
categories: ['Reading Group']

# Is this a featured talk? (true/false)
featured: false

image:
  caption: 'Image credit: [**DeepMind**](https://www.deepmind.com/publications/a-generalist-agent)'
  focal_point: Center

header:
  image: "featured.png"
  caption: 'Image credit: [**DeepMind**](https://www.deepmind.com/publications/a-generalist-agent)'

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



# <h5 style="text-align: center;">Share</h5>
---
{{% cta cta_link="https://teams.microsoft.com/l/meetup-join/19%3aLiP6Evh3ssJQ3g41q8vAsBNwwOFTzp7d_qq1y7oTo7A1%40thread.tacv2/1654597085925?context=%7b%22Tid%22%3a%222b897507-ee8c-4575-830b-4f8267c3d307%22%2c%22Oid%22%3a%228d261fd5-be8f-44eb-b630-d5b230fc5ec3%22%7d" cta_text="Join Session!" %}}

# Papers

[A Generalist Agent](https://arxiv.org/pdf/2205.06175.pdf?fs=e&s=cl), arXiv'22

**Paper Abstract:**
Inspired by progress in large-scale language modeling, we apply a similar approach towards building a single generalist agent beyond the realm of text outputs. The agent, which we refer to as Gato, works as a multi-modal, multi-task, multi-embodiment generalist policy. The same network with the same weights can play Atari, caption images, chat, stack blocks with a real robot arm and much more, deciding based on its context whether to output text, joint torques, button presses, or other tokens. In this report we describe the model and the data, and document the current capabilities of Gato.


# Discussion Notes

Gato is a new take on how to achieve multi-task agents based on autoregressive modeling of sequence data.

This paper was perhaps a bit out of scope for a SysML group, but we came up with a few future directions from the reading.

## Input pipeline

The input pipeline in Gato is far more complex than a conventional Supervised Learning input pipeline

The inputs come from a large number of datasets (604, one per task) all which have large corpora.
Are available sampling mechanisms able to scale to these dimensions?

Furthermore, on each iteration it requires tokenization, linearization and embedding of multi-modal inputs such that a batch containing a mix of tasks is formed.
While images are embedded using a ResNet block, text, actions and observations are embedded through a learned embedding.
Are existing libraries such as tf.data capable of such complex input pipelines? Can they maintain good throughput with these unbalanced tasks?


## Democratizing Fine-Tuning

A common pattern nowadays seems to be that large research groups will pre-train extremely large general models (language models) and other groups will then fine-tune them to achieve good performance on a specific task (fine-tuning).
How is the workload of fine-tuning different from pre-training? Would it be possible to democratize fine-tuning such that it can be done on a laptop?

## Attention, Memory and Context Windows

To maintain a memory of the recent past, Gato uses a sliding window of recent observations and actions.
To achieve the long-term planning needed for general RL, an infinitely sized window would be needed.
However, growing the window size in current Transformer implementations would grow memory and compute requirements too.
Are Transformers the correct approach to RL? Could transformers be augmented with a long-term memory component? Or could their training systems be fundamentally altered such that they can handle larger windows without growing memory requirements?



