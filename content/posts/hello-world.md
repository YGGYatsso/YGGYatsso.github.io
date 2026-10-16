---
title: "Hello World"
date: 2026-10-16T22:30:00+05:30
tags: ["meta"]
categories: ["General"]
summary: "Welcome to my new blog — how this site was built and what to expect."
math: true
draft: false
---

Welcome to my corner of the internet. This site is built with [Hugo](https://gohugo.io/) and the [PaperMod](https://github.com/adityatelange/hugo-PaperMod) theme — the same stack behind [Lil'Log](https://lilianweng.github.io/), hosted for free on GitHub Pages.

## What to expect

I'll be writing about topics I'm learning and working on:

- **Machine learning** — architectures, training dynamics, inference
- **Computer vision & 3D** — neural rendering, pose estimation, SLAM
- **Mathematics** — probability, statistics, and the theory I need to understand papers properly
- **GPU programming** — CUDA kernels, memory hierarchies, and performance

## Writing a post

New posts go in the `content/posts/` directory as Markdown files named `YYYY-MM-DD-title.md`. This file itself is an example — copy it to get started.

Code blocks work out of the box:

```python
import torch

def attention(q, k, v):
    scores = q @ k.transpose(-2, -1)
    return torch.softmax(scores / q.size(-1) ** 0.5, dim=-1) @ v
```

Math renders too (enabled with `math: true` in the front matter):

$$
\mathcal{L}(\theta) = -\mathbb{E}_{x \sim p_\theta}[\log p_\theta(x)]
$$

Thanks for reading — more soon.
