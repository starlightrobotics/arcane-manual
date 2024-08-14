# Challenges for LLM development and adoption

## What we need in LLMs
* **Faster and Cheaper LLMs** - an ongoing field of optimisation and improvement. in 2023-2024 the jump in scale and improvement of quality is stunning.
* **More context size for local models** and **Better long-term memory** - many models are reported to have larger context window, but they fail to actually use it.
    * Is addressed through techniques like *Self-extend* and *Flash Attention*, although not many models are compatible yet.
* **Better character preservation** - over time as the conversation carries on, the character sheet needs to be re-injected into the conversation, to refresh the behaviour.
     * Is addressed through better long-term memory.
* **Better logic** - LLMs are language models, not logic models. They write text well and they are fascinating about how much they can do, but are not explicitly designed for logical tasks.
    * Language models are not directly designed to solve logical problems. Currently they do not even solve those problems, but rather predict the most popular reply to that question.

## LoRAs and Finetunes
* Many loras are compatible only with a specific model.
* Fine-tunes sometimes break the quality of the base model
