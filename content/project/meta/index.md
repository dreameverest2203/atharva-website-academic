---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Instance Specific Data Augmentation for Meta Learning"
summary: "We design a novel data augmentation module for meta learning that creates instance specific augmentations in a few shot setting."
authors: []
tags: ['Meta Learning', 'Deep Learning']
categories: []
date: 2022-12-21T10:30:45-08:00

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: "Top"
  preview_only: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_code: "https://github.com/anujnag/learn2aug"
url_pdf: "https://drive.google.com/file/d/1S5323QkUL6OA-4cfpkAj6EUs1Vh1UNOF/view?usp=sharing"
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---
Meta-learning frameworks are usually trained in a few-shot setting and suffer from data scarcity. A straightforward solution to this problem is using data augmentation to expand our support set used for training the meta-learning parameters. But applying the same augmentation for all input instances can be problematic. For instance, applying the same 180-degree rotation to a dataset of images may change a 6 to a 9, or applying the same color jitter may change a lemon to a lime. While prior works in data augmentation have largely focused on instance-agnostic augmentation strategies, we propose a novel technique for generating instance-based augmentations called AutoInstanceAug which is adapted for meta-learning setup where we don’t have sufficient data to train.