# Transformer-Pyramid Hybrid Architecture for Vietnamese Fake News Detection

**Nghiên cứu kiến trúc mạng lai Transformer-Pyramid kết hợp đặc trưng đồ thị trong phát hiện tin giả tiếng Việt**

Tác giả: **Nguyễn Quốc Quyền**

---

## Giới thiệu
Mô hình **Transformer-Pyramid Hybrid** kết hợp:
- PhoBERT (deep semantic encoding)
- Lớp kim tự tháp đa nhánh song song (CNN + Bi-GRU + Graph Attention Network - GAT)
- Đặc trưng thống kê bổ trợ
- CatBoost Classifier

Mô hình đạt:
- **Accuracy**: 93.86%
- **AUC-PR**: 0.98
- **F1-Score (macro)**: 0.9385

Đây là nghiên cứu đầu tiên triển khai thành công nhánh **Graph Attention Network (GAT)** trên dữ liệu tin giả tiếng Việt.

---

## Kết quả nổi bật
- Vượt trội hơn các baseline truyền thống (LSTM, Bi-LSTM, CNN-BiLSTM)
- Lần đầu thực thi nhánh GAT theo hướng nghiên cứu của Võ Đức Vinh & Đỗ Phúc (2023)
- Độ bền vững cao trên dữ liệu nhiễu và tin tức thời sự năm 2026

---

## Dataset
- VNDF Vietnamese Fake News Dataset: [GitHub](https://github.com/WhySchools/VFND-vietnamese-fake-news-datasets)
- Kaggle Fake and Real News Dataset (dịch sang tiếng Việt): [Kaggle](https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset)

Tổng số mẫu: **44.472** (cân bằng giữa tin thật và tin giả).

---

## Cách tái lập kết quả (Reproduce)

1. Clone repository:
   ```bash
   git clone https://github.com/[tên-user-của-bạn]/Transformer-Pyramid-Hybrid-Vietnamese-FakeNews.git
   cd Transformer-Pyramid-Hybrid-Vietnamese-FakeNews
