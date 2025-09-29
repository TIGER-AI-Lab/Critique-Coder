# Critique-Coder

## install
'''
conda create --name critique-coder python=3.10
conda activate critique-coder
pip install -e verl
pip install -e ".[vllm,acecoder]"
pip install "flash-attn<2.8.0" --no-build-isolation
'''
