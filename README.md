# ML Playground

Collection of focused ML engineering mini-projects.

---

## 📌 Modules

### 1️⃣ TrOCR Handwriting OCR + Benchmarking

Fine-tuned a transformer-based OCR model (TrOCR) on the IAM handwritten dataset and benchmarked inference performance on a T4 GPU.

**Highlights:**
- CER: 0.086
- WER: 0.332
- P50 latency: 248 ms
- Best throughput: 4.14 images/sec (batch=2)

Tech stack:
- PyTorch
- HuggingFace Transformers
- Datasets
- jiwer
- Google Colab (T4 GPU)
