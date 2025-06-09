# Fine-Tuning-LLM-using-Soft-Prompting-Adapter-Techniques-with-PEFT
Large Language Models (LLMs) have shown
outstanding performance on a vast array of Natural
Language Processing (NLP) tasks. Nonetheless, their
applicability in practical scenarios is still limited in
low-resource settings owing to the computational
requirements of end-to-end fine-tuning, especially in the
context of GPU memory (VRAM) and training time. This
paper presents a hybrid and memory-efficient LLM
fine-tuning framework for LLMs, specifically in the context
of Google's Gemma 2B model, for the sentiment analysis
task. The suggested method combines a number of
state-of-the-art parameter-efficient fine-tuning (PEFT)
techniques, including Soft Prompting, Quantized
Low-Rank Adaptation (QLoRA), Low-Rank Adaptation
(LoRA), and Progressive Layer Dropping (PLD). Soft
Prompting provides light task adaptation without updating
base model weights, whereas LoRA and QLoRA update
selective low-rank matrices in attention layers with fewer
precision settings. Progressive Layer Dropping also speeds
up training further by dynamically pruning less effective
transformer layers. The whole process is streamlined for
memory-constrained settings like Kaggle and Google Colab,
where VRAM availability becomes a key limitation.
Empirical testing on the IMDb Sentiment Analysis
benchmark shows that the suggested approach attains
competitive accuracy and F1-scores with respect to full
fine-tuning, while significantly decreasing memory
consumption and training time. This paper offers a
scalable, modular, and accessible PEFT-based approach
towards democratizing fine-tuning of LLMs in low-resource
environments.
