# Fine-tuning and Testing LLM with LLaMA Factory

This project uses [LLaMA Factory](https://github.com/hiyouga/LLaMA-Factory) for fine-tuning and evaluating a large language model (LLM), specifically Qwen2.5-7B-Instruct.

## Installation

First, install **LLaMA Factory** by running the following commands:

```bash
git clone --depth 1 https://github.com/hiyouga/LLaMA-Factory.git
cd LLaMA-Factory
pip install -e ".[torch,metrics]" --no-build-isolation
````

## Fine-tuning and Evaluation

After installation, change to the `run` directory and run the scripts to fine-tune and test the model:

```bash
cd ../run
```

* To fine-tune the model:

```bash
bash Qwen2.5-7B-Instruct_sft.sh
```

* To evaluate the fine-tuned model:

```bash
bash Qwen2.5-7B-Instruct_predict_sft.sh
```

## Script Descriptions

* `Qwen2.5-7B-Instruct_sft.sh`: Supervised fine-tuning (SFT) script for Qwen2.5-7B-Instruct.
* `Qwen2.5-7B-Instruct_predict_sft.sh`: Inference or evaluation script using the fine-tuned model.

To customize training or inference parameters, please edit the corresponding `.sh` script files.
