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

*GGML:* GPT-Generated Mixed List format

*GGUF:* GPT-Generated Unified Format

*GPTQ:* GPT Quantization format

## Quantization Details (sometimes included):

Quantization Parameters: This might provide specifics about the chosen quantization method, such as the bit-depth used (e.g., 8-bit). However, this level of detail is less frequently included in the name itself.


#### Examples

*Name:* Mixtral-8x22B-Instruct-v0.1-GGML

*Model Name:* Mixtral

*Version Number:* v0.1

*Parameter Count:* 8x22B

Quantization Format: GGML (GPT-Generated Mixed List format)
