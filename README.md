# Recommendation System Using Content-based Graph Convolutional Network (GCN)
## Thông tin về các file
- Thư mục ml-100k chứa dữ liệu từ tập MovieLens 100k
- Thư mục ml-1m chứa dữ liệu từ tập MovieLens 1M
- file analizing_data.ipynb là phần phân tích dữ liệu đầu vào
- GCN_100k_content_context là mô hình đề xuất trên tập MovieLens 100k
- GCN_1m_content_context là mô hình đề xuất trên tập MovieLens 1M

Link github: https://github.com/CAO816/recommender_GCN.git
## Đây là sơ đồ mô hình GCN 3 lớp
![image](https://github.com/user-attachments/assets/e7382720-1da6-48f9-a989-1ca93350ef3b)

![image](https://github.com/user-attachments/assets/ab55bf54-5862-410b-aeef-90fabaaf8d79)

## Dữ liệu đầu vào
Mô hình sử dụng dữ liệu huấn luyện và thực nghiệm là MovieLens 100K và MovieLens 1M

Phần phân tích dữ liệu nằm trong file analizing_data.ipynb
## Xây dựng đồ thị user-item-context
![image](https://github.com/user-attachments/assets/7a79393d-760d-4cd1-bdc8-a42005c940e1)

## Các lớp tích chập
- Mô hình gồm 3 lớp GCN trích xuất các đặc trưng cho user và item
## Lớp Multi-head Self-attention
- Lớp attention này giúp mỗi đỉnh tự động học được mức độ liên quan đến các đỉnh khác trong toàn bộ đồ thị, từ đó cập nhật embedding của mình một cách linh hoạt và toàn cục hơn, vượt ra khỏi phạm vi láng giềng cục bộ mà GCN học được.
## Đầu ra của mô hình
- Ma trận gồm các vector đặc trưng của người dùng và item
