# API for Open LLMs



[Original Document](./raw_README.md)

## Quick Deployment
### Install Dependencies
```bash
conda env create -f ./server.yml

```
### Modify Configuration (Optional)
Modify the local `.env` file, refer to
```
PORT=10086

# model related
MODEL_NAME=internlm2
MODEL_PATH=AI4Chem/ChemLLM-7B-Chat-1.5-DPO
EMBEDDING_NAME=jinaai/jina-embeddings-v2-base-zh
CONTEXT_LEN=32000
LOAD_IN_8BIT=false
LOAD_IN_4BIT=false
USING_PTUNING_V2=false
STREAM_INTERVERL=2
PROMPT_NAME=

# device related
DEVICE=

# "auto", "cuda:0", "cuda:1", ...
DEVICE_MAP=auto
GPUS=
NUM_GPUs=2
DTYPE=half


# api related
API_PREFIX=/v1

USE_STREAMER_V2=false

# vllm related
ENGINE=default
```
### Inference
```
conda activate server
python server.py
```

[原文档](./raw_README.md)
## 快速部署
### 安装依赖
```bash
conda env create -f ./server.yml

```
### 修改配置（可选）
修改本地`.env`文件，参考
```
PORT=10086

# model related
MODEL_NAME=internlm2
MODEL_PATH=AI4Chem/ChemLLM-7B-Chat-1.5-DPO
EMBEDDING_NAME=jinaai/jina-embeddings-v2-base-zh
CONTEXT_LEN=32000
LOAD_IN_8BIT=false
LOAD_IN_4BIT=false
USING_PTUNING_V2=false
STREAM_INTERVERL=2
PROMPT_NAME=

# device related
DEVICE=

# "auto", "cuda:0", "cuda:1", ...
DEVICE_MAP=auto
GPUS=
NUM_GPUs=2
DTYPE=half


# api related
API_PREFIX=/v1

USE_STREAMER_V2=false

# vllm related
ENGINE=default
```
### 推理
```
conda activate server
python server.py
```
