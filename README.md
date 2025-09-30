# Critique-Coder

<a target="_blank" href="https://github.com/TIGER-AI-Lab/CritiqueFineTuning">
<img style="height:22pt" src="https://img.shields.io/badge/-Code-black?style=flat&logo=github"></a>
<a target="_blank" href="https://arxiv.org/abs/2501.17703">
<img style="height:22pt" src="https://img.shields.io/badge/-Paper-green?style=flat&logo=arxiv"></a>
<a target="_blank" href="https://tiger-ai-lab.github.io/CritiqueFineTuning">
<img style="height:22pt" src="https://img.shields.io/badge/-🌐%20Website-red?style=flat"></a>
<a target="_blank" href="https://huggingface.co/datasets/TIGER-Lab/WebInstruct-CFT">
<img style="height:22pt" src="https://img.shields.io/badge/-🤗%20Dataset-red?style=flat"></a>
<a target="_blank" href="https://huggingface.co/collections/TIGER-Lab/critiquefinetuning-679b25e1528e75180f55e5c4">
<img style="height:22pt" src="https://img.shields.io/badge/-🤗%20Models-red?style=flat"></a>
<br>

## Installation
```bash
git clone https://github.com/TIGER-AI-Lab/Critique-Coder.git
cd Critique-Coder
conda create --name critique-coder python=3.10
conda activate critique-coder
pip install -e verl
pip install -e ".[vllm,acecoder]"
pip install "flash-attn<2.8.0" --no-build-isolation
```

## Dataset Preparation
```bash
hf download chiruan/crl_test --local-dir ./data/critique-coder-dataset --repo dataset
```

## Training
```bash
bash examples/train/train_qwen3_4b_16k.sh
```
