# AWS SageMaker LLM Samples

This repository contains a collection of sample projects and notebooks for deploying, fine-tuning, and using large language models (LLMs) on AWS SageMaker. These samples have been used with customers over the past two years and cover a variety of popular open-source LLMs and related tools.

## Directory Structure

- **sagemaker_llm_samples/**
  - **baichuan/**: Notebooks for deploying, fine-tuning, and pretraining Baichuan models on SageMaker.
  - **bloomz/**: Example notebook for training Bloomz-7B on SageMaker.
  - **codegen/**
    - General code generation LLM deployment and fine-tuning samples.
    - **code_intereptor/**: Demos and scripts for code generation agents and web APIs.
    - **text2sql/**: Notebooks and scripts for text-to-SQL generation using codegen models.
  - **Falcon/**: Notebooks for deploying Falcon models, including OpenBuddy Falcon 7B, on SageMaker.
  - **langchain/**: Integration samples with LangChain, including SQL agent demos and ingestion pipelines.
  - **qwen/**: Notebooks for deploying and running inference with Qwen models on SageMaker.
  - **text2sql/**: End-to-end text-to-SQL pipeline samples, including GUI, database setup, and deployment scripts.
  - **vicuna/**: Notebooks for deploying, training, and running inference with Vicuna and Llama models on SageMaker.

## Example Contents

### baichuan/

- `baichuan2-7b-base-sagemaker-finetune-dist.en.ipynb`: Fine-tuning Baichuan 2 7B on SageMaker.
- `baichuan2-7b-base-sagemaker-infer-endpoint.en.ipynb`: Inference endpoint deployment.
- `baichuan_7B_deploy.ipynb`, `baichuan_fine_tune_lora.ipynb`, `baichuan_pretrain.ipynb`: Additional deployment and training notebooks.

### bloomz/

- `sagemaker-trainging-bloomz-7B.ipynb`: Training Bloomz-7B on SageMaker.

### codegen/

- `bge_zh_deploy.ipynb`, `codellama-13b_deploy.ipynb`, `sqlcoder-15b_deploy.ipynb`, `wizardcoder-15b-sagemaer-finetune-dist.en.ipynb`, etc.: Deployment and fine-tuning for various code generation models.
- **code_intereptor/**: Agent demos, utility scripts, and web API for code generation.
- **text2sql/**: Text-to-SQL generation demos and scripts.

### Falcon/

- `Falcon_deploy.ipynb`, `OpenBuddy_Falcon_7B_deploy.ipynb`: Falcon model deployment samples.

### langchain/

- `func.py`, `intension_ingestion.ipynb`, `lanchain_SqlAgent_demo.ipynb`, `langchain_sqlDataBaseChain_demo.ipynb`, etc.: LangChain integration and SQL agent demos.

### qwen/

- `sagemaker_inference_qwen_deploy.ipynb`, `sagemaker_inference_qwen_stream.ipynb`: Qwen model deployment and streaming inference.

### text2sql/

- `Dockerfile`, `build_and_push.sh`, `ddl.sql`, `func.py`, `requirements.txt`, `setup.sh`, `text2sql_gui.py`, `text2sql_sqlAgent_workshop.ipynb`, `text2sql_with_meta_retreve.py`: Complete text-to-SQL pipeline, including GUI, database setup, and deployment scripts.

### vicuna/

- `sagemaker-inference-7B.ipynb`, `sagemaker-inference-llama2-13B-Chinese.ipynb`, `sagemaker-inference-rollingbatch-pagedattn.ipynb`, `sagemaker-inference-server-batch-v2.ipynb`, `sagemaker-inference-vllm-llama2-13b-v3.ipynb`, `sagemaker-inference-vllm-llama2-70b-v2.ipynb`, `sagemaker-inference-vllm-llama2-stream.ipynb`, `sagemaker-inference-vllm.ipynb`, `sagemaker-llama-training-with-wandb.ipynb`, `sagemaker-vicuna-training.ipynb`: Comprehensive deployment, training, and inference samples for Vicuna and Llama models.

---

## Getting Started

1. Clone this repository.
2. Explore the subdirectories for model-specific or use-case-specific samples.
3. Open the Jupyter notebooks (`.ipynb`) in SageMaker Studio or your preferred Jupyter environment.
4. Follow the instructions in each notebook to deploy, fine-tune, or use the models.

## Requirements

- AWS account with SageMaker access
- Sufficient instance quota for large models (e.g., ml.p3, ml.p4, ml.g5)
- Python 3.8+
- See individual subdirectory `requirements.txt` files for additional dependencies

## License

This repository is intended for educational and demonstration purposes. Please review the license terms of each model and dataset before use in production.
