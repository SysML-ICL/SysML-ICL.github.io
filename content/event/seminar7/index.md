---
title: "Seminar #7 - Fan Mo - PPFL (MobiSys'21)"

location: Huxley 315 - Imperial College London
#address:
#  postcode: 'Room 145'


summary: "Fan Mo will present his work PPFL: Privacy-preserving Federated Learning with Trusted Execution Environments (MobiSys'22)"
abstract: |
  Although user data are not collected at a centralized location in federated learning (FL), adversaries can still execute various types of privacy attacks to retrieve sensitive information from the FL model parameters themselves, thus breaking the initial privacy promises behind FL.
  
  PPFL, a practical, privacy-preserving federated learning framework, is proposed to protect clients’ private information against known privacy-related attacks. PPFL adopts greedy layer-wise FL training and updates layers always inside Trusted Execution Environments (TEEs) at both server and clients. We implemented PPFL with mobile-like TEE (i.e., TrustZone) and server-like TEE (i.e., Intel SGX) and empirically tested its performance. For the first time, we showed the possibility of fully guaranteeing privacy and achieving comparable ML model utility with regular end-to-end FL, without significant communication and system overhead.

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: '2023-02-09T14:00:00Z'
date_end: '2023-02-09T15:00:00Z'
all_day: false

# Schedule page publish date (NOT talk date).
publishDate: '2023-01-10T00:00:00Z'

authors: []
profile: false
tags: ['Federated Learning', 'Trusted Execution Environments', 'Privacy', 'Intel SGX', 'Adversarial Attacks']
categories: ['Seminar']

# Is this a featured talk? (true/false)
featured: true

image:
  caption: ''
  focal_point: Right

url_code: ''
url_pdf: 'https://dl.acm.org/doi/abs/10.1145/3458864.3466628?casa_token=J6ja1oF8qmoAAAAA:UA_3MRt-a66Q98kNg5-gEL_KdNBlLVNupGoV3nE89NvuSKuaP45Y6App8OzGztUP1R7iQ4zGcq2yHQ'
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
<a title="Add to Calendar" class="addeventatc" data-id="wM15912240" href="https://www.addevent.com/event/wM15912240" target="_blank">Add to Calendar</a>
	<script type="text/javascript" src="https://cdn.addevent.com/libs/atc/1.6.1/atc.min.js" async defer></script>
{{< /rawhtml >}}
{{< /center >}}

# Speaker Bio

Fan Mo is a Senior Researcher at Trustworthy AI Lab, Huawei. Before that, he completed his PhD at Imperial College London in 2022, advised by Professor Hamed Haddadi. He also worked for a short time in Nokia Bell Labs, Arm Research, and Telefónica Research. His research focuses on data privacy and trustworthiness in machine learning at the edge, machine learning in confidential computing, and distributed machine learning on lightweight mobile/IoT devices.
