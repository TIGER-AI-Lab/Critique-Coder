# Critique-Coder

<p align="center">
| 
<a href="https://arxiv.org/abs/2509.01055"><b>Paper</b></a> |
<a href="https://github.com/TIGER-AI-Lab/verl-tool/blob/main/assets/docs/install.md"><b>Quick Start</b></a> |
<a href="https://github.com/TIGER-AI-Lab/verl-tool/tree/main/examples/train"><b>Training Recipes</b></a> |
<a href="https://deepwiki.com/TIGER-AI-Lab/verl-tool"><b>DeepWiki</b></a> |
<a href="https://github.com/TIGER-AI-Lab/verl-tool/tree/main/assets/imgs/wechat_group.jpg"><b>WeChat Group</b></a> |
<a href="https://discord.gg/CUARJFJ8"><b>Discord</b></a>
|
</p>

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
