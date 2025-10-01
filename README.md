# Critique-Coder

| [**🚀Project Page**](https://tiger-ai-lab.github.io/Critique-Coder/) | [**📖Paper**](https://arxiv.org/abs/2509.22824) | [**🤗Data**](https://huggingface.co/datasets/TIGER-Lab/rStar-Critique-Data) | [**🤗Model**](https://huggingface.co/collections/TIGER-Lab/critique-coder-68dbdcdf09dbf87ed11822e4) |

## Overview
![./assets/images/crl_teaser.jpg](./assets/images/crl_teaser.jpg)

## Get Started
### Installation
```bash
git clone https://github.com/TIGER-AI-Lab/Critique-Coder.git
cd Critique-Coder
conda create --name critique-coder python=3.10
conda activate critique-coder
pip install -e verl
pip install -e ".[vllm,acecoder]"
pip install "flash-attn<2.8.0" --no-build-isolation
```

### Dataset Preparation
```bash
hf download TIGER-Lab/rStar-Critique-Data --local-dir ./data/critique-coder-dataset --repo dataset
```

### Training
```bash
bash examples/train/train_qwen3_4b_16k.sh
```
### Evaluation
We use [EvalPlus](https://github.com/evalplus/evalplus), [BigCodeBench](https://github.com/bigcode-project/bigcodebench), [Aider-Polyglot](https://github.com/Aider-AI/aider/tree/main/benchmark), [LiveCodeBench](https://github.com/LiveCodeBench/LiveCodeBench) for the evaluation of EvalPlus, BigCodeBench, Aider-Polyglot, LiveCodeBench, respectively.

## Citations
If you find this work helpful, please cite us with:
```
@article{ruan2025critiquecoder,
    title={Critique-Coder: Enhancing Coder Models by Critique Reinforcement Learning},
    author={Ruan, Chi and Jiang, Dongfu and Wang, Yubo and Chen, Wenhu},
    journal={ArXiv},
    year={2025},
    volume={2509.22824}
}
```
