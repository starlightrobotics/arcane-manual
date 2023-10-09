# Hardware requirements

Performance by HuggingFace can be found in [🤗 LLM-Perf Leaderboard 🏋️](https://huggingface.co/spaces/optimum/llm-perf-leaderboard)

## CPU/RAM vs GPU/VRAM

In practice you do not need GPU for VRAM. If you have access to CPU with an equivalent VRAM, then you can get away with slower, but still functional system.

**Example:** Falcon 180B will not fit into NVidia 4090, but it will fit into a system with 128 Gb of RAM.

RAM considerations: 1 DIMM per 1 memory channel. If your Motherboard has 2 channels - even if you have 8 RAM sticks, it is not going to change much. Long story short: 2x48 Gb > 4x32 Gb in some cases.

## What can I run on Nvidia 4090 / 24 Gb VRAM?


As of October 2023, 4090 can handle most 30B LLMs.

8bit ExLlama2 Mythomax-13B with extended context and still have vram to spare, with performance being ~40 t/s.

Mistral model uses something called grouped query attention to reduce VRAM utilization for the context, so it would use less.
This is the max quality exl2 [Mythomax](https://huggingface.co/QMB15/mythomax-13B-8.13bit-MAX-exl2).
It's ~18GB at 4k context, ~16GB with flash attention library installed, or alternatively [MythoMax-L2-13B-exl2](https://huggingface.co/R136a1/MythoMax-L2-13B-exl2).


[Llama2-70B](https://huggingface.co/turboderp/Llama2-70B-exl2) can be potentially run on 4090 with [ExLlama2](https://github.com/turboderp/exllamav2#exl2-quantization)
