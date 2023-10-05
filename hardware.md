# Nvidia 4090 / 24 Gb VRAM

As of October 2023, 4090 can handle most 30B LLMs.

I run a 8bit exl2 Mythomax-13B with extended context and still have vram to spare, with performance being ~40 t/s.
Mistral actually uses something called grouped query attention to reduce vram utilization for the context
So it would use less
This is the max quality exl2 I used - https://huggingface.co/QMB15/mythomax-13B-8.13bit-MAX-exl2
It's ~18GB at 4k context, ~16GB with flash attention library installed
I use it because I can, it probably isn't much better than a smaller quant, such as 6 bpw
https://huggingface.co/R136a1/MythoMax-L2-13B-exl2

[Llama2-70B](https://huggingface.co/turboderp/Llama2-70B-exl2) can be potentially run on 4090 with [ExLlama2](https://github.com/turboderp/exllamav2#exl2-quantization)
