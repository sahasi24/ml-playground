# TrOCR Handwriting OCR + Inference Benchmark

Mini ML Engineering project demonstrating fine-tuning, evaluation, and inference benchmarking of a transformer-based OCR model.

---

## Dataset
- Teklia/IAM-line (handwritten English text)
- 1000 train / 200 val / 200 test subset

---

## Model
- microsoft/trocr-base-handwritten
- Fine-tuned for 3 epochs on Colab T4 GPU

---

## Results

### Accuracy
- CER: 0.086
- WER: 0.332

### Inference Benchmark (T4 GPU)

Single-image inference (max_length=64):
- Mean latency: 264 ms
- P50 latency: 248 ms
- P95 latency: 361 ms

Throughput:
- Batch size 1: 2.36 images/sec
- Batch size 2: 4.14 images/sec (best)
- Batch size 4: 3.73 images/sec
- Batch size 8: 3.47 images/sec

Preprocessing latency: ~6 ms per image.

---

## What This Demonstrates

- Transformer fine-tuning for OCR
- CER vs WER analysis
- Latency profiling (p50/p95)
- Throughput scaling
- GPU inference benchmarking
