Tiêu chí: 
- GPU VRAM <=8GB
- Set up mỗi lần nhanh chóng
- Dùng lúc nào tính tiền lúc đó
- Giá rẻ

Option 1: https://cloud.vast.ai/
Option 2: https://www.runpod.io/

### Bảng so sánh Vast.ai và RunPod

| Tiêu chí | Vast.ai | RunPod |
|--------|---------|--------|
| Mô hình | Marketplace: nhiều host tự đặt giá, bro chọn máy tốt/giá rẻ | Cloud “1 nhà cung cấp”: Community + Secure Cloud  [runpod](https://www.runpod.io/pricing) |
| Cách tính tiền | Pay‑as‑you‑go, **bill per‑second**, chia 3 phần: GPU, storage, bandwidth  [docs.vast](https://docs.vast.ai/documentation/instances/pricing) | Pay‑as‑you‑go, thường bill per‑minute/giờ cho Pod, storage/network riêng  [runpod](https://www.runpod.io/pricing) |
| Mức giá điển hình | GPU từ ~0.03 USD/giờ, rất nhiều GPU 0.04–0.10 USD/giờ (GTX 1080, 3070, A2000, A4000…)  [computeprices](https://computeprices.com/providers/vast) | Community Cloud: RTX 3090 ~0.22–0.46 USD/giờ, Secure Cloud/4090 ~0.44+ USD/giờ  [gpus](https://gpus.io/providers/runpod) |
| Giá GPU 24GB (ví dụ) | RTX 3090 24GB ~0.17 USD/giờ, A5000 24GB ~0.20 USD/giờ  [getdeploying](https://getdeploying.com/vast-ai) | A40 48GB ~0.40 USD/giờ; cùng GPU trên Vast khoảng 0.32 USD/giờ (rẻ hơn ~24%)  [computeprices](https://computeprices.com/compare/runpod-vs-vast) |
| Giá so với cloud lớn | Thường rẻ hơn 3–5x so với hyperscaler  [getdeploying](https://getdeploying.com/vast-ai) | Quảng cáo rẻ hơn tới 80% so với hyperscaler  [runpod](https://www.runpod.io/pricing) |
| Team / dùng chung lớp | Có **Teams** + balance riêng, billing team tách biệt cá nhân  [docs.vast](https://docs.vast.ai/documentation/teams/teams-overview) | Có **Team accounts**, role Admin/Dev/Billing, giới hạn spend/hour  [docs.runpod](https://docs.runpod.io/get-started/manage-accounts) |
| Cách nạp & quản lý tiền | Nạp tiền vào balance, team có ví riêng, xem chi tiết từng charge GPU/disk/net  [docs.vast](https://docs.vast.ai/documentation/reference/billing) | Nạp credit, xem cost per Pod, có limit chi tiêu để tránh overrun  [docs.runpod](https://docs.runpod.io/get-started/manage-accounts) |
| Tính “siêu rẻ” | Rất mạnh: nhiều GPU 6–12GB 0.04–0.06 USD/giờ; GPU 16–24GB tầm 0.10–0.20 USD/giờ  [computeprices](https://computeprices.com/providers/vast) | Rẻ so với AWS/GCP, nhưng thường **đắt hơn Vast.ai 20–80% cùng GPU**  [computeprices](https://computeprices.com/compare/runpod-vs-vast) |
| Tốc độ setup | Chọn template (Ubuntu/CUDA/PyTorch), launch vài chục giây, SSH là dùng; phải tự chọn host  [getdeploying](https://getdeploying.com/vast-ai) | Nhiều template Pod sẵn, UI mượt, launch rất nhanh, ít phải suy nghĩ về host  [runpod](https://www.runpod.io/pricing) |
| Ổn định & độ “sạch” | Phụ thuộc từng host (data center / cá nhân), cần xem rating, uptime  [getdeploying](https://getdeploying.com/vast-ai) | Có Community (rẻ) + Secure Cloud (ổn định hơn, SOC2, SLA cao)  [checkthat](https://checkthat.ai/brands/runpod/pricing) |
| Độ dễ dùng UI | Hơi “dev”, nhiều thông số (disk, bandwidth, host rating), ban đầu hơi rối  [getdeploying](https://getdeploying.com/vast-ai) | UI thân thiện, rõ concept Pod/Serverless, dễ cho người mới  [runpod](https://www.runpod.io/pricing) |
| Dùng cho bootcamp (1–2 GPU chung lớp) | Rất hợp nếu bro **ưu tiên giá**, chấp nhận vọc 1–2 buổi đầu để tìm host ngon | Hợp nếu bro muốn **ít friction**, demo nhiều, chấp nhận trả thêm tiền |
| Dùng cho production long‑run | Ok nếu chọn host DC uy tín, nhưng vẫn là marketplace, standardization thấp hơn | Secure Cloud + Serverless khá chuẩn cho production, có thêm feature enterprise  [checkthat](https://checkthat.ai/brands/runpod/pricing) |

---

- Với tiêu chí số 1 là **“siêu rẻ cho lớp, bật khi dạy, tắt là hết tiền”** → **Vast.ai** là lựa chọn tốt hơn:  
  - GPU 16–24GB giá thường 0.10–0.20 USD/giờ, rẻ hơn RunPod cùng cấu hình khoảng 20–30% trở lên. [getdeploying](https://getdeploying.com/vast-ai)
  - Có Teams + ví chung, phù hợp mô hình “deposit 1 triệu, dùng đến đâu trừ đến đó”. [docs.vast](https://docs.vast.ai/documentation/teams/teams-overview)

---
# Option 1: https://cloud.vast.ai/

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



https://www.perplexity.ai/search/goi-y-flow-trien-nhanh-cho-anh-TLm6d4h4SDSkbNNrvJn.SQ
