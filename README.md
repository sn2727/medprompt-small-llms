## LLMs as a valid tool for patient education/patient information pre-surgery

This project investigates two questions: 
- Are LLMs, like openELM, capable of effectively educating patients about pre-transplantation surgery on mobile devices? 
- Among specialized models, fine-tuned models, and foundation models, which is more suitable for patient education purposes?


## Efficient LLMs for mobile devices

Trend in development of LLMs to make them more efficient to use for deployment on mobile devices. 

Models considered: 
- microsoft/Phi-3-mini-4k-instruct (3.82B params)
- TinyLlama/TinyLlama-1.1B-Chat-v0.1 (1.1B params)
- apple/OpenELM-3B (3B params)


1000 surgery questions from MedMCQA (consists of various medical entrance exam questions) (HF: `openlifescienceai/medmcqa`):

| Model | Parameters | Accuracy |
|-------|------------|----------|
|phi-3  |  3.82B     | 66.80%   |
|llama  |  1.1B      | 26.00%   |
|openelm|  3B        | 28.70%   |