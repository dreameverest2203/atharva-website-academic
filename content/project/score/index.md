---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Score-based Generative Models"
summary: "We show that diffusion models based on a score matching objective are improved with a multi-sample training objective."
authors: []
tags: ["Generative Models"]
# categories: ["Generative Models"]
date: 2022-08-28T21:37:52-07:00

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_code: "https://github.com/dreameverest2203/score_matching_refined"
url_pdf:  "https://drive.google.com/file/d/1Tr3mZGBAQfFYm-p1TYECzo6oTc9NfqjK/view?usp=sharing"
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---
Score-based Generative Models (SGMs) have been considered by some as the new competitor to GANs in Generative Modeling. They have been able to give high quality samples without any adversarial sampling, while also providing the facility to compute exact likelihood. In this project, we propose a further improvement in their score estimation framework by utilizing multiple noisy inputs instead of just one. We build our idea over the well-known equivalence between score matching and denoising autoencoders and show that the model along with Tweedie's formula can be easily extended to multiple samples, thus giving it the capacity to obtain better score estimates close to true distribution scores for langevin dynamics sampling.