# Decoding model names

## Main name

*Model Name:* This is the core identifier, often descriptive (e.g., Bard) or brand-oriented (e.g., Jurassic-1 Jumbo).

*Version Number:* This indicates the model’s development stage (e.g., v3.1).

## Additional Information (often included):

*Architecture:* This describes the model’s internal structure (e.g., Transformer-XL). Numbers following the architecture might indicate specific configurations (e.g., 12-layer).

*Parameter Count:* This signifies the model’s size and complexity, typically denoted in billions (e.g., 137B).

*Context Size:* This refers to the amount of text the model considers for each prediction, influencing its ability to capture context (e.g., 2048 tokens).

*Quantization Format:* This indicates if the model has been optimized for efficiency by converting its weights to a lower precision format. 

#### Examples

* *GGML:* GPT-Generated Mixed List format
* *GGUF:* GPT-Generated Unified Format
* *GPTQ:* GPT Quantization format

## Quantization Details (sometimes included):

Quantization Parameters: This might provide specifics about the chosen quantization method, such as the bit-depth used (e.g., 8-bit). However, this level of detail is less frequently included in the name itself.


#### Examples

* *Name:* Mixtral-8x22B-Instruct-v0.1-GGML
* *Model Name:* Mixtral
* *Version Number:* v0.1
* *Parameter Count:* 8x22B

Quantization Format: GGML (GPT-Generated Mixed List format)

# Base names

* GPT family - by OpenAI
    - GPT3 - 170B+ model, 2020
    - GPT3.5
    - GPT4, GPT4-Turbo, GPT4-V(ision)
* Claude family - by Anthropic
    - Claude, Claude 2, Claude 3 Haiku, Sonnet, Opus
* Qwen family - by Alibaba
    - Qwen
    - Qwen-VL
* Gemini family, Bard, PaLM family - by Google
   - PaLM (Pathways Language Model) - 540B precursor of Gemini, but also has spin-off projects like MedPaLM
   - Gemma - opensource
   - BERT - transformer-based
   - Lamda - 2021
* Mistral/Mixtral - by Mistral
    - Mistral
    - Mixtral
* NeuralChat - by Intel
* Command, Rerank and Embed - by Cohere
* Ernie - by Baidu
* Falcon - by Technology Innovation Institute, transformer-based
* Orca, Phi - by Microsoft
    - Orca - 13B competitor of GPT4
    - Phi-1 - 1.3B, transformer-based
* StableLM - by Stability AI that specialises in image generations with Stable Diffusion
* Vicuna - by LMSYS, derived from Llama, at 33B is a little less powerful as GPT4

[LLM Survey Feb 2024](https://arxiv.org/abs/2402.06196)

# Mixes and Fine-tunes

* **OpenHermes** - OpenHermes 2.5 is a 7B model, fine-tuned by Teknium on Mistral, surpasses all previous versions of **Nous-Hermes** 13B and below.
* **Alpaca** 7B, a model fine-tuned from the **LLaMA** 7B
* **Moistral** and **Cream-Phi** - Fine-tuned Mistral and Phi by [TheDrummer](https://huggingface.co/TheDrummer)
