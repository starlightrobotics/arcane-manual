# Hardware requirements

Performance by HuggingFace can be found in [🤗 LLM-Perf Leaderboard 🏋️](https://huggingface.co/spaces/optimum/llm-perf-leaderboard)

## CPU/RAM vs GPU/VRAM

In practice you do not need GPU for VRAM. If you have access to CPU with an equivalent VRAM, then you can get away with slower, but still functional system.

**Example:** Falcon 180B will not fit into NVidia 4090, but it will fit into a system with 128 Gb of RAM in some cases (see below).

RAM considerations: 1 DIMM per 1 memory channel. If your Motherboard has 2 channels - even if you have 8 RAM sticks, it is not going to change much. Long story short: 2x48 Gb > 4x32 Gb in some cases.

## What can I run on Nvidia 4090 / 24 Gb VRAM?


As of October 2023, 4090 can handle most 30B LLMs.

8bit ExLlama2 Mythomax-13B with extended context and still have vram to spare, with performance being ~40 t/s.

Mistral model uses something called grouped query attention to reduce VRAM utilization for the context, so it would use less.
This is the max quality exl2 [Mythomax](https://huggingface.co/QMB15/mythomax-13B-8.13bit-MAX-exl2).
It's ~18GB at 4k context, ~16GB with flash attention library installed, or alternatively [MythoMax-L2-13B-exl2](https://huggingface.co/R136a1/MythoMax-L2-13B-exl2).


[Llama2-70B](https://huggingface.co/turboderp/Llama2-70B-exl2) can be potentially run on 4090 with [ExLlama2](https://github.com/turboderp/exllamav2#exl2-quantization)


## What kind of hardware would it take to run falcon 180b

Mac Studio M2 Ultra with 192GB of RAM. It can run a Q5_K_M of Falcon 180b, but it comes absolutely nowhere near 15 tokens per second; closer to 2-4 tokens per second.

To run a q3 of the 180b, you need close to 90GB of RAM.

Locally, outside of the SUPER expensive workstation devices, 4x 4090s could probably do it. I'm not sure even four 3090s could hit 15 tokens

## LLaMA hardware requirements
*source: [r/LocalLLaMMa](https://www.reddit.com/r/LocalLLaMA/comments/11o6o3f/how_to_install_llama_8bit_and_4bit/)*
**8-bit Model Requirements for GPU inference**

| Model	              | VRAM Used	| Card examples	| RAM/Swap to Load | 
| LLaMA 7B / Llama 2  7B |	10GB	| 3060 12GB, 3080 10GB	| 24 GB| 
| LLaMA 13B / Llama 2 13B	| 20GB	 | 3090, 3090 Ti, 4090	| 32 GB |
| LLaMA 33B / Llama 2 34B	| ~40GB	 | A6000 48GB, A100 40GB	| ~64 GB |
| LLaMA 65B / Llama 2 70B	| ~80GB | 	A100 80GB	| ~128 GB | 

*System RAM, not VRAM, required to load the model, in addition to having enough VRAM. Not required to run the model. You can use swap space if you do not have enough RAM.

4-bit Model Requirements for GPU inference
Model	Minimum Total VRAM	Card examples	RAM/Swap to Load*
LLaMA 7B / Llama 2 7B	6GB	GTX 1660, 2060, AMD 5700 XT, RTX 3050, 3060	6 GB
LLaMA 13B / Llama 2 13B	10GB	AMD 6900 XT, RTX 2060 12GB, 3060 12GB, 3080, A2000	12 GB
LLaMA 33B / Llama 2 34B	~20GB	RTX 3080 20GB, A4500, A5000, 3090, 4090, 6000, Tesla V100	~32 GB
LLaMA 65B / Llama 2 70B	~40GB	A100 40GB, 2x3090, 2x4090, A40, RTX A6000, 8000	~64 GB

*System RAM, not VRAM, required to load the model, in addition to having enough VRAM. Not required to run the model. You can use swap space if you do not have enough RAM.
