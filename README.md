# Neural Flow Diffusion Models

Neural Flow Diffusion Models (NFDM) is a framework that generalizes conventional diffusion models. 
The key idea in NFDM is to define the forward process' conditional SDE implicitly 
via a learnable transformation $F_\varphi(\varepsilon, t, \mathbf{x})$ 
that defines the marginal distributions. 
This lets the user define a broad range of continuous time- and data-dependent forward processes, 
that the reverse process will learn to invert. 
Importantly, NFDM retains crucial properties of conventional diffusion models, 
like likelihood-based and simulation-free training.

Check out the [paper](https://arxiv.org/abs/2404.12940) for more details.

## Setup

We provide a `requirements.txt` file for a pip environment. 

```bash
pip install -r requirements.txt
```

## Getting started

The best way to understand our method is to look at [the notebook](https://github.com/GrigoryBartosh/neural_diffusion/blob/main/nfdm_from_scratch.ipynb) which contains a simple implementation of the NFDM model on a toy dataset.

## Citation

If you find our work useful, please consider citing our paper:

```bibtex
@article{bartosh2024neural,
  title={Neural flow diffusion models: Learnable forward process for improved diffusion modelling},
  author={Bartosh, Grigory and Vetrov, Dmitry P and Andersson Naesseth, Christian},
  journal={Advances in Neural Information Processing Systems},
  volume={37},
  pages={73952--73985},
  year={2024}
}
```