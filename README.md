## LLMs as a valid tool for patient education/patient information pre-surgery

This project investigates two questions: 
- Are LLMs, like openELM, capable of effectively educating patients about pre-transplantation surgery on mobile devices? 
- Among specialized models, fine-tuned models, and foundation models, which is more suitable for patient education purposes?


## Efficient LLMs for mobile devices

Trend in development of LLMs to make them more efficient to use for deployment on mobile devices. 

Models considered: 
- microsoft/Phi-3-mini-4k-instruct (3.82B params)
- TinyLlama/TinyLlama-1.1B-Chat-v0.1 (1.1B params)
- apple/OpenELM-3B (3.04B params)
- google/gemma-2b-it (2.51B params)

1000 surgery questions from MedMCQA (consists of various medical entrance exam questions) (HF: `openlifescienceai/medmcqa`):

| Model | Accuracy |
|-------|----------|
|phi-3  | 66.8%    |
|llama  | 26.0%    |
|openelm| 28.7%    | 
|gemma  | 32.7%    | 

1000 multiple choice questions from `GBaker/MedQA-USMLE-4-options` USMLE dataset

| Model | Accuracy |
|-------|----------|
|phi-3  | 63.7%    |
|llama  | 22.4%    |
|openelm| 27.1%    |
|gemma  | 30.4%    |