https://www.perplexity.ai/search/goi-y-flow-trien-nhanh-cho-anh-TLm6d4h4SDSkbNNrvJn.SQ

---

Tớ đã filter xong trên màn hình Vast.ai của anh. Dưới đây là kết quả thực tế đang hiển thị, sort theo **giá tăng dần (Price inc.)**, filter **1X GPU**, toàn bộ RTX series: [cloud.vast](https://cloud.vast.ai/create/?numGPUs=1&gpu_ram=8&rentable=true&order=dph_total%2Basc&storageOpt=0)

***

## Kết quả tìm được - GPU ~8GB VRAM rẻ nhất hiện tại

| # | Card | VRAM | Giá/giờ | Reliability | Location | Ghi chú |
|---|------|------|---------|-------------|----------|---------|
| 1 | **RTX 3070** | 8 GB | **$0.045/hr** | 99.54% | New York, US | ⭐ Rẻ nhất, ổn định nhất |
| 2 | **RTX 3060** | 12 GB | **$0.045/hr** | 99.53% | South Korea | 12GB nhưng cùng giá 8GB |
| 3 | **RTX 3060** | 12 GB | **$0.052/hr** | 99.48% | British Columbia, CA | On-demand, verified |
| 4 | **RTX 3070** | 8 GB | **$0.053/hr** | 95.8% | Mexico | Reliability thấp hơn |
| 5 | **RTX 3060 Ti** | 8 GB | **$0.053/hr** | ~96% | Mexico | - |

***

## Anh nên chọn con nào?

**→ Chọn #1: RTX 3070 - $0.045/hr - New York (host:126496)**
- 8 GB VRAM đúng nhu cầu
- Reliability **99.54%** cao nhất
- Max Duration **7 months** - thoải mái bật tắt
- **Chi phí thực tế**: 3 tiếng dạy = **$0.135** (~3.500đ/buổi), cả tháng dùng 40h = **$1.8**

***

## Cách thuê ngay - 3 bước

**Bước 1:** Click **RENT** trên row RTX 3070 New York đó

**Bước 2:** Cấu hình khi launch:
- Image: chọn **`vastai/base:cuda12.4`** hoặc Ubuntu Docker
- Disk: set **60GB** (đủ chứa model + cache HuggingFace)
- Ports: expose **8000** (vLLM), **8001** (embedding)

**Bước 3:** SSH vào và chạy:
```bash
# Pull và chạy vLLM
docker run --gpus all -p 8000:8000 vllm/vllm-openai:latest \
  vllm serve Qwen/Qwen2.5-1.5B-Instruct \
  --quantization awq_marlin \
  --max-model-len 4096 \
  --gpu-memory-utilization 0.85

# Embedding chạy riêng (port 8001)
pip install sentence-transformers fastapi uvicorn
```

***

## Lưu thành template để bật lại nhanh

Sau khi setup xong, vào **Instances → Instance đó → Save Template** → đặt tên `vllm-embedding-8gb`. Lần sau chỉ cần:
- **Select Template → chọn template của anh → Rent** → 1-2 phút là có máy y hệt.

Anh muốn tớ click **RENT** con RTX 3070 $0.045/hr đó luôn không?
