# mambaGPT
State space model based GPT  


## Setup - Local Conda
```bash
git clone https://github.com/Monarch-25/mambaGPT.git
conda create -y --name mambaGPT python=3.11
conda activate mambaGPT
pip install torch --index-url https://download.pytorch.org/whl/cu121
pip install tiktoken==0.7.0
pip install datasets==2.20.0
pip install transformers
cd mambaGPT
git clone https://github.com/state-spaces/mamba.git
pip install packaging==24.1
pip install causal-conv1d #Requires an NCCL backend 
cd mamab && pip install -e . && cd ..
pip install wandb==0.17.1
```

test dependencies
```bash
python3 train.py
```

## Setup - Docker




