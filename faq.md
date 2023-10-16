# Frequently Asked Questions

1. **What do I need to start?** -
   * **Locally** - [Hardware](hardware.md) + User Interface + LLM
   * **Cloud** - User Interface + API
   * **Web services** - [List](online-servces.md)

3. **Do I need GPU?** - You do not need GPU to run LLMs. You can run them on CPU + Equivalent RAM. GPU makes models run faster.

4. **GGUF vs GGML?** - GGUF is positioned as an upgrade to GGML, offering more flexibility, extensibility, and compatibility. It aims to simplify the user experience and accommodate various models beyond llama. cpp. GGML, while a valuable early effort, had limitations that GGUF seeks to overcome.

5. **What do perplexity numbers mean?** - A lower perplexity score indicates better predictability and understanding of the language, while a higher perplexity score suggests a higher degree of uncertainty and less accurate predictions

6. **What do "13b q4" or "Q4_0" mean?** - quantization measurements. The basic model is unquantized. 
    * q4_0 = 32 numbers in chunk, 4 bits per weight, 1 scale value at 32-bit float (5 bits per value in average), each weight is given by the common scale * quantized value.  
    * q4_1 = 32 numbers in chunk, 4 bits per weight, 1 scale value and 1 bias value at 32-bit float (6 bits per value in average), each weight is given by the common scale * quantized value + common bias.
    * q4_2 = same as q4_0, but 16 numbers in chunk, 4 bits per weight, 1 scale value that is 16-bit float, same size as q4_0 but better because chunks are smaller.
    * q4_3 = already dead, but analogous: q4_1 but 16 numbers in chunk, 4 bits per weight, scale value that is 16 bit and bias also 16 bits, same size as q4_1 but better because chunks are smaller.
    * q5_0 = 32 numbers in chunk, 5 bits per weight, 1 scale value at 16-bit float, size is 5.5 bits per weight
    * q5_1 = 32 numbers in a chunk, 5 bits per weight, 1 scale value at 16 bit float and 1 bias value at 16 bit, size is 6 bits per weight.
    * q8_0 = same as q4_0, except 8 bits per weight, 1 scale value at 32 bits, making total of 9 bits per weight.
