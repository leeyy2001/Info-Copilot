# Info-Copilot
Repository for code and text generation using open source Large Language Models

## Overview
1. The implementation of the models are found in the models folder. You can refer to the huggingface website for the documentation on how to use it. 
2. Code to install the models canbe found in the model-downloader notebook

## Troubleshooting guide
1. Taking too long to run the models. \
'''
model = AutoModelForCausalLM.from_pretrained(model_path, trust_remote_code=True).to(device)

inputs = tokenizer.encode("def print_hello_world():", return_tensors="pt").to(device)
'''
