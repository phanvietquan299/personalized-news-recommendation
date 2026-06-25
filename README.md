# Personalized News Recommendation

Hệ thống gợi ý tin tức cá nhân hóa dựa trên nội dung bài viết, chủ đề, embedding và dữ liệu hành vi người dùng. Dự án này được tổ chức để hỗ trợ toàn bộ pipeline từ thu thập dữ liệu, tiền xử lý, mô hình hóa chủ đề, sinh embedding, xây dựng bộ gợi ý, cho đến đánh giá kết quả.

## Mục tiêu

- Thu thập tin tức từ nhiều nguồn khác nhau.
- Làm sạch và chuẩn hóa dữ liệu bài viết.
- Trích xuất chủ đề và biểu diễn ngữ nghĩa của nội dung.
- Xây dựng cơ chế gợi ý phù hợp với sở thích người dùng.
- Đánh giá chất lượng hệ thống bằng các chỉ số rõ ràng.

## Cấu trúc dự án

```text
personalized-news-recommendation
│
├── data/
├── notebooks/
├── src/
│   ├── crawler/
│   ├── preprocessing/
│   ├── topic_modeling/
│   ├── embedding/
│   ├── recommendation/
│   └── evaluation/
│
├── reports/
├── papers/
├── experiments/
├── requirements.txt
└── README.md
```

## Ý nghĩa từng thư mục

- `data/`: dữ liệu thô, dữ liệu đã xử lý và tập dữ liệu trung gian.
- `notebooks/`: notebook cho khám phá dữ liệu, thử nghiệm mô hình và phân tích kết quả.
- `src/crawler/`: mã thu thập tin tức từ website hoặc API.
- `src/preprocessing/`: làm sạch văn bản, tách từ, chuẩn hóa và tạo đặc trưng.
- `src/topic_modeling/`: mô hình hóa chủ đề cho bài viết.
- `src/embedding/`: tạo vector biểu diễn nội dung và người dùng.
- `src/recommendation/`: logic gợi ý và xếp hạng bài viết.
- `src/evaluation/`: đánh giá offline và các chỉ số chất lượng.
- `reports/`: báo cáo phân tích, kết quả thí nghiệm và tài liệu tổng hợp.
- `papers/`: tài liệu tham khảo, bài báo, ghi chú nghiên cứu.
- `experiments/`: cấu hình và kết quả các lần chạy thử nghiệm.

## Cài đặt

1. Tạo môi trường ảo Python.
2. Cài đặt các thư viện cần thiết từ `requirements.txt`.

Ví dụ:

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

## Hướng phát triển

- Xây dựng pipeline crawl dữ liệu tin tức.
- Tạo bộ tiền xử lý cho tiếng Việt và tiếng Anh.
- Thử nghiệm các mô hình topic modeling và embedding.
- Thiết kế baseline recommendation và đánh giá theo từng kịch bản.
- Ghi lại kết quả trong `reports/` và `experiments/`.
