---
title: "Parallel Automatic Differentiation Talk"

location: Huxley 145

summary: HiPEDS Centre hosting seminar on Parallel Automatic Differentiation by William Moses.
abstract: ''

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: '2022-05-13T11:00:00Z'
date_end: '2022-05-13T12:00:00Z'
all_day: false

publishDate: '2022-05-11T00:00:00Z'

authors: []
profile: false
tags: ["Automatic Differentiation", "Compilers", "GPU", "LLVM"]
categories: ['News']

featured: false

image:
  caption: 'Image credit: [**Author Page**](https://wsmoses.com)'
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
**Talk Title:** Enzyme: High-Performance, Cross-Language, and Parallel Automatic Differentiation

[Zoom Link](https://imperial-ac-uk.zoom.us/j/97378427420?pwd=VENub3h5eVJscXVTbDk5cG9sVGFMdz09)

## Author Bio


William Moses is a Ph.D. Candidate at MIT, where he also received his M.Eng in electrical engineering and computer science (EECS) and B.S. in EECS and physics. William's research involves creating compilers and program representations that enable performance and use-case portability, thus enabling non-experts to leverage the latest in high-performance computing and ML. He is known as the lead developer of Enzyme (NeurIPS '20, SC '21), an automatic differentiation tool for LLVM capable of differentiating code in a variety of languages, after optimization, and for a variety of architectures and the lead developer of Polygeist (PACT '21), a polyhedral compiler and C++ frontend for MLIR. He has also worked on the Tensor Comprehensions framework for synthesizing high-performance GPU kernels of ML code, the Tapir compiler for parallel programs (best paper at PPoPP '17), and compilers that use machine learning to better optimize. He is a recipient of the U.S. Department of Energy Computational Science Graduate Fellowship and the Karl Taylor Compton Prize, MIT's highest student award.


## Abstract
Automatic differentiation (AD) is key to training neural networks, Bayesian inference, and scientific computing. Applying these techniques requires rewriting code in a specific machine learning framework or manually providing derivatives. This talk presents Enzyme, a high-performance automatic differentiation compiler plugin for the low-level virtual machine (LLVM) compiler capable of synthesizing gradients of programs expressed in the LLVM intermediate representation (IR). Enzyme differentiates programs in any language whose compiler targets LLVM, including C/C++, Fortran, Julia, Rust, Swift, etc., thereby providing native AD capabilities in these languages with state-of-the-art performance. Unlike traditional tools, Enzyme performs AD on optimized IR. On a combined machine-learning and scientific computing benchmark suite, AD on optimized IR achieves a geometric mean speedup of 4.2x over AD on IR before optimization. This talk will also include work that makes Enzyme the first fully automatic reverse-mode AD tool to generate gradients of existing GPU kernels. This includes new GPU and AD-specific compiler optimizations, and an algorithm ensuring correctness of high-performance parallel gradient computations. We provide a detailed evaluation of five GPU-based HPC applications, executed on NVIDIA and AMD GPUs.

---

<h5 style="text-align: center;">Share</h5>
