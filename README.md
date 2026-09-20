# Localize, Edit, Unlearn

**Structural Interventions and Data-Level Control in Foundation Models**

Ph.D. thesis defense slides — Keivan Rezaei, University of Maryland, College Park, 17 September 2026.

📄 **[Download the slides](https://github.com/k1rezaei/thesis-slides/releases/latest)**

## About the talk

Where does a foundation model keep what it knows, and what can we do once we find it?

The talk runs in three parts:

- **Localize** — finding the handful of cross-attention layers in a diffusion model, or the handful of blocks in a diffusion transformer, that carry a particular style, object or fact.
- **Edit** — rewriting those layers in closed form, or fine-tuning only those blocks, to remove a style, swap a trademarked object or correct an outdated fact.
- **Unlearn** — turning the same question on the training data: what did one slice of it do to the model, and can that effect be undone? This part introduces a benchmark that asks for *recovery* rather than silence, and a method that reads the model's own checkpoint history.

A closing section covers mechanism design for placing advertising inside LLM outputs.

The deck is 63 slides, plus an appendix of backup material and references.

### Work presented

| Paper | Venue |
|---|---|
| On Mechanistic Knowledge Localization in Text-to-Image Generative Models | ICML 2024 |
| Localizing Knowledge in Diffusion Transformers | NeurIPS 2025 |
| RESTOR: Knowledge Recovery through Machine Unlearning | TMLR 2025 |
| Revisiting the Past: Data Unlearning with Model State History | ICLR 2026 |
| Ad Auctions for LLMs via Retrieval Augmented Generation | NeurIPS 2024 |
| Online Advertisements with LLMs: Opportunities and Challenges | SIGecom Exchanges 2025 |

## About me

I am a Ph.D. candidate in Computer Science at the University of Maryland, advised by
[Soheil Feizi](https://www.cs.umd.edu/~sfeizi/) and
[MohammadTaghi Hajiaghayi](https://www.cs.umd.edu/~hajiagha/).
My research is on the interpretability of generative models, from both a model perspective
(localizing knowledge, explaining failure modes) and a data perspective (machine unlearning,
data selection for pretraining).

🔗 [k1rezaei.github.io](https://k1rezaei.github.io/)

## Building

```
latexmk -pdf main.tex
```

`main.tex` holds the slides; `header.tex` holds the preamble, theme and custom macros.
The Damion font files (`damion.tfm`, `t1damion.fd`, `Damion-Regular.ttf`) must stay in the
repository root — they typeset the RESTOR wordmark.

## Credits

Built on the [Beamer template](https://github.com/sleepymalc/LaTeX-Template/tree/main/Beamer)
by [Pingbang Hu](https://github.com/sleepymalc). Thank you.

Figures are taken from the papers listed above; logos are public-domain files from Wikimedia
Commons, used to identify their organizations.

---

<sub>README written by Claude Code, verified by Keivan Rezaei.</sub>
