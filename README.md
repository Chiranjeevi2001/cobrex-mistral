# Finetuning Mistral 7b instruct model for COBREX
This work deals with the finetuning of the popular LLM `Mistral-7b` on business rules JSON database which was manually created through few-shot prompting with `Gemini Pro`. We aim to automate the process of extracting Business rules from legacy COBOL code and use it to better understand the business logic embedded within the code. With this, a way to streamline modernization tasks can be formed which revolves around the idea of extracting and understanding the business rules embedded within legacy code base. 

## Finetuning:
Mistral-7b base instruct model can be found [here](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2).

<br>

Dataset used to finetune the model can be found [here](https://huggingface.co/datasets/Chiranjeevi2001/cobol_br_instruct_dataset).

<br>

The model has been trained using [QLoRA](https://medium.com/@levxn/lora-and-qlora-effective-methods-to-fine-tune-your-llms-in-detail-6e56a2a13f3c) technique, which enables large models to be trained on GPU-poor machines.
