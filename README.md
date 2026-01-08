## Guiding Token-Sparse Diffusion Models
[![arXiv](https://img.shields.io/badge/arXiv-2601.01608-b31b1b.svg)](https://arxiv.org/abs/2601.01608)
[![Project Page](https://img.shields.io/badge/Project-Page-blue)](https://compvis.github.io/sparse-guidance/)
[![Code](https://img.shields.io/badge/Code-CompVis%2Ftread-black)](https://github.com/CompVis/tread?tab=readme-ov-file#-guiding-tread)

[Felix Krause](https://x.com/felix_m_krause) · [Stefan Andreas Baumann](https://stefan-baumann.eu) · [Johannes Schusterbauer](https://johfischer.com/) · [Olga Grebenkova](https://scholar.google.com/citations?user=OBeGHt4AAAAJ&hl=en) · [Ming Gui](https://scholar.google.com/citations?hl=en&user=Uiv6gU8AAAAJ) · [Vincent Tao Hu](https://taohu.me) · [Björn Ommer](https://ommer-lab.com/people/ommer)

CompVis @ LMU Munich, Munich Center for Machine Learning (MCML)

![Sparse Guidance overview](https://compvis.github.io/sparse-guidance/static/images/title_fig.png)

**TL;DR:** Token-sparse diffusion models (masking/routing) train fast and can be strong conditionals, but Classifier-free Guidance (CFG) often breaks at inference.
We introduce Sparse Guidance (SG), a finetune-free guidance rule that uses token sparsity as the guidance signal:
combine a strong low-sparsity conditional prediction with a weak high-sparsity conditional prediction.
On ImageNet-256, SG reaches 1.58 FID with 25% fewer FLOPs and enables up to 58% FLOP savings at matched baseline quality.
SG also scales to a 2.5B text-to-image model, improving human preference and throughput.

> [!NOTE]
> This repository is a landing page for **Sparse Guidance** and primarily exists to host the project website.
> 
> **➡️ The official code lives in [`CompVis/tread`](https://github.com/CompVis/tread?tab=readme-ov-file#-guiding-tread).**  
> Please refer to that repository for code, setup, and inference instructions.

## 🎓 Citation

```bibtex
@misc{krause2026guidingtokensparsediffusionmodels,
      title={Guiding Token-Sparse Diffusion Models}, 
      author={Felix Krause and Stefan Andreas Baumann and Johannes Schusterbauer and Olga Grebenkova and Ming Gui and Vincent Tao Hu and Björn Ommer},
      year={2026},
      eprint={2601.01608},
      archivePrefix={arXiv},
      primaryClass={cs.CV},
      url={https://arxiv.org/abs/2601.01608}, 
}
```
