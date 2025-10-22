# Large Language Models

## LLM Quantization:
Quantization is a compression technique that involves mapping high precision values to the lower precision one. For an LLM, that means modifying the presion of weights and activations making it less memory intensive. But remember this is surely going to have an impact on the capabilities of LLMs including accuracy. Quantization basically reduce memory bandwidth requirement and increase cache utilization.

#### How does quantization works?
LLM are generally trained with full(float32) or half percision(float16) floating point numbers. One float has 16 bits which is 2 bytes. So, it takes 2 gigabytes for one billion parameters model trained on FP16.

The process of quantization thus works on finding a way to represent the range which is [min, max] for the datatype of FP32 weight values