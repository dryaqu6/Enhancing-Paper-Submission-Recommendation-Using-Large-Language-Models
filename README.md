# Enhancing-Paper-Submission-Recommendation-Using-Large-Language-Models

Dự án nghiên cứu và cải thiện hệ thống gợi ý nơi công bố bài báo khoa học (Paper Submission Recommendation) dựa trên các mô hình ngôn ngữ lớn (LLMs) và cơ chế Attention nâng cao.
## 📝 Giới thiệu
Việc tìm kiếm một tạp chí hoặc hội nghị phù hợp với nội dung nghiên cứu là bước quan trọng nhưng tốn nhiều thời gian. Dự án này đề xuất các phương pháp tiếp cận từ truyền thống đến hiện đại (Transformer-based) để tối ưu hóa việc so khớp ngữ nghĩa giữa bài báo và mục tiêu (Aims & Scope) của các nơi công bố.

## 🚀 Các phương pháp tiếp cận (Methodology)

Dự án thử nghiệm 4 chiến lược chính:

| Phương pháp | Mô tả kỹ thuật |
| :--- | :--- |
| **Approach A** | Baseline sử dụng biểu diễn tĩnh như FastText hoặc TF-IDF. |
| **Approach B** | Sử dụng Transformer (DistilRoBERTa) để lấy Embedding ngữ cảnh. |
| **Approach C** | Áp dụng Contrastive Learning (tương tự SimCPSR) để tối ưu không gian vector. |
| **Approach D** | **(Đề xuất)** Sử dụng cơ chế **Cross-Attention** để tính toán tương tác mức độ token. |

## 📊 Kết quả nổi bật
* **Giai đoạn Truy hồi (Retrieval):** Approach C đạt hiệu quả cao nhất về tốc độ và khả năng thu hẹp phạm vi ứng viên.
* **Giai đoạn Tái sắp xếp (Re-ranking):** Approach D (Cross-Attention) cải thiện đáng kể độ chính xác (Mean Rank) nhờ khả năng "soi" kỹ mối liên hệ giữa từ vựng trong bài báo và mô tả của tạp chí.

## 📚 Tham khảo (References)
Dự án này được xây dựng dựa trên các phương pháp nghiên cứu từ bài báo:
* **SimCPSR:** [Simple Contrastive Learning for Paper Submission Recommendation](https://arxiv.org/abs/2205.05940v1) (arXiv:2205.05940).

