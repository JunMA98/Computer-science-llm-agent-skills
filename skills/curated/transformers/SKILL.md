---
name: transformers
description: Work with transformer models for CS research and development. Use when loading, fine-tuning, evaluating, or serving language, vision, audio, multimodal, embedding, or LLM-style models for tasks such as generation, classification, retrieval, instruction tuning, benchmarking, or agent backends.
---

# Transformers

Use this skill for Hugging Face Transformer workflows in research, prototyping, and model-backed systems.

## Common Uses

- run inference with pretrained checkpoints
- fine-tune encoders or generators on custom datasets
- benchmark LLMs or embedding models
- build retrieval, reranking, or classification pipelines
- configure tokenization, batching, and generation
- use open models as components inside agent or tool systems

## Local References

Read only what matches the task:
- `references/models.md`
- `references/tokenizers.md`
- `references/generation.md`
- `references/training.md`
- `references/pipelines.md`

## Working Rules

- Match model family to the actual task and latency budget.
- Make truncation, padding, and prompt formatting explicit.
- Record checkpoint version, tokenizer, and generation settings for reproducibility.
- Distinguish quick pipeline usage from training-grade code paths.
- If gated models or hub operations are involved, call out token requirements explicitly.

## Default Output

When the user asks for transformer help without more detail, return:
1. model/task fit recommendation
2. inference or training setup notes
3. data and tokenization considerations
4. reproducibility or deployment caveats