# Hands-On Large Language Models (LLMs)

Welcome to the **Hands-On LLM** repository — a practical series of experiments, tutorials, and real-world applications using large language models (LLMs). This repo demonstrates how to use open LLMs from Hugging Face and beyond in NLP workflows, covering tasks like chat-based interaction, generation, prompt engineering, and fine-tuning.

---

## Projects

### 1. Chat Templates with Real-World Examples

**Notebook**: [`chatTemplatesWithRealWorldExamples.ipynb`](./chatTemplatesWithRealWorldExamples.ipynb)  
**Project**: Demonstrates how to use Hugging Face `ChatTemplate` to structure chat-style messages for open LLMs. The notebook includes real-world examples such as customer support dialogs, and assistant-style prompts.  
**Focus**: Prompt formatting and chat template handling with different models (like SmolLM2, Mistral).  
**Tools**: Hugging Face Transformers, ChatTemplate, Open LLMs  

---

### 2. Supervised Fine-Tuning (SFT)

**Notebook**: [`SupervisedFineTuning(SFT).ipynb`](./SupervisedFineTuning(SFT).ipynb)  
**Project**:  Fine-tune the [`HuggingFaceTB/SmolLM2-135M`](https://huggingface.co/HuggingFaceTB/SmolLM2-135M) model using the SFTTrainer from the trl library.  
**Task**: Supervised instruction-following for open-ended QA/dialog tasks.  
**Dataset**: [`HuggingFaceTB/smoltalk`](https://huggingface.co/datasets/HuggingFaceTB/smoltalk) and [`bigcode/the-stack-smol`](https://huggingface.co/datasets/bigcode/the-stack-smol)  
**Fine-Tuned Model**: [`Mhammad2023/SmolLM2-FT-MyDataset`](https://huggingface.co/Mhammad2023/SmolLM2-FT-MyDataset) for smoltalk data and [`Mhammad2023/SmolLM2-FT-BigCode-Python`](https://huggingface.co/Mhammad2023/SmolLM2-FT-BigCode-Python) for bigcode data.  
**Tools**: Transformers, PEFT, TRL, bitsandbytes, Hugging Face Hub

---

### 3. LoRA (Low-Rank Adaptation) with LLaMA-2

**Notebook**: [`LoRA(Low_Rank_Adaptation).ipynb`](./LoRA(Low_Rank_Adaptation).ipynb)  
**Dataset**: [`HuggingFaceTB/smoltalk`](https://huggingface.co/datasets/HuggingFaceTB/smoltalk) and [`bigcode/the-stack-smol`](https://huggingface.co/datasets/bigcode/the-stack-smol)  
**Base Model**: [`HuggingFaceTB/SmolLM2-135M`](https://huggingface.co/HuggingFaceTB/SmolLM2-135M)    
**Task**: Perform parameter-efficient fine-tuning with LoRA adapters using QLoRA (4-bit quantization).  
**Tools**: PEFT, Transformers, TRL, BitsAndBytes, Hugging Face Hub  
**Highlights**:
- Efficient training on consumer-grade hardware
- Reduces GPU memory requirements with 4-bit precision
- Modular adapter training with LoRA

---




