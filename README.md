# Understanding Visual Concepts Across Models

Brandon Trabucco (1), Max Gurinas (2), Kyle Doherty (3), Ruslan Salakhutdinov (1)

(1) Carnegie Mellon University, (2) University of Chicago Laboratory Schools, (3) MPG Ranch

[Website](https://visual-words.github.io) &nbsp;|&nbsp; [PDF](https://visual-words.github.io/static/understanding_visual_concepts_small.pdf) &nbsp;|&nbsp; [ArXiv](https://arxiv.org/abs/2406.07506) &nbsp;|&nbsp; [Code](https://github.com/visual-words/visual-words) &nbsp;|&nbsp; [BibTex](https://visual-words.github.io/static/bibtex.txt)

![teaser gif](images/teaser.gif)

## Abstract 

Large multimodal models such as Stable Diffusion can generate, detect, and classify new visual concepts after fine-tuning just a single word embedding. Do models learn similar words for the same concepts (i.e. <orange-cat> = orange + cat)? We conduct a large-scale analysis on three state-of-the-art models in text-to-image generation, open-set object detection, and zero-shot classification, and find that new word embeddings are model-specific and non-transferable. Across 4,800 new embeddings trained for 40 diverse visual concepts on four standard datasets, we find perturbations within an $\epsilon$-ball to any prior embedding that generate, detect, and classify an arbitrary concept. When these new embeddings are spliced into new models, fine-tuning that targets the original model is lost. We show popular soft prompt-tuning approaches find these perturbative solutions when applied to visual concept learning tasks, and embeddings for visual concepts are not transferable. Code for reproducing our work is available at: [visual-words.github.io](https://visual-words.github.io).

## Roadmap

* Release training code for generation, detection, and classification tasks.
* Release transfer evaluation code.
* Release 4,800 fine-tuned tokens for main experiments.

Check back often, we are releasing in the next 2 weeks!

## Citing our work

```
@misc{trabucco2024VisualWords,
  title={Understanding Visual Concepts Across Models},
  author={Brandon Trabucco and Max Gurinas and Kyle Doherty and Ruslan Salakhutdinov},
  year={2024},
  eprint={2406.07506},
  archivePrefix={arXiv},
  primaryClass={cs.CV},
}
```
