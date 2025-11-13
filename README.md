# 🎭 Artist Co-Appearance Prediction  
*Dự đoán sự xuất hiện chung & gợi ý đối tác cho nghệ sĩ trong gameshow Việt Nam*

![Stars](https://img.shields.io/github/stars/maithanhphuc2004/Artist-Coappearance-Prediction?style=flat-square)
![Forks](https://img.shields.io/github/forks/maithanhphuc2004/Artist-Coappearance-Prediction?style=flat-square)
![Issues](https://img.shields.io/github/issues/maithanhphuc2004/Artist-Coappearance-Prediction?style=flat-square)
![Last Commit](https://img.shields.io/github/last-commit/maithanhphuc2004/Artist-Coappearance-Prediction?color=green&style=flat-square)

![Python](https://img.shields.io/badge/Python-3.10+-blue?style=flat-square&logo=python)
![License](https://img.shields.io/badge/License-MIT-yellow?style=flat-square)
![Status](https://img.shields.io/badge/Status-Active-success?style=flat-square)

---

## 📌 Overview *(Tổng quan)*  
This project predicts potential collaborations between Vietnamese artists in TV gameshows using **Social Network Analysis (SNA)** and **Machine Learning**.  
*(Dự án dự đoán khả năng hợp tác giữa nghệ sĩ trong gameshow bằng phân tích mạng xã hội & học máy.)*

Artists and shows are automatically extracted from Wikipedia and processed to build a large co-appearance network for link prediction.  
*(Dữ liệu nghệ sĩ–gameshow được crawl từ Wikipedia và xây dựng thành mạng đồng xuất hiện phục vụ dự đoán.)*

---

## ✨ Key Features *(Tính năng chính)*  
- 🔄 Automated Wikipedia crawling *(Thu thập dữ liệu tự động)*  
- 🧹 Name extraction & cleaning *(Làm sạch dữ liệu nghệ sĩ)*  
- 🕸 Co-appearance network construction *(Xây dựng mạng đồng xuất hiện)*  
- 🔍 Similarity-based link prediction *(Dự đoán bằng độ đo tương đồng)*  
- 🤖 Machine Learning prediction *(Dự đoán bằng học máy)*  
- 🎯 Top-K partner recommendation *(Gợi ý Top-K nghệ sĩ hợp tác)*  

---

## 📈 Model Performance *(Hiệu suất mô hình)*

### 🔹 Similarity-Based Metrics  
| Metric | AUC | Notes |
|--------|-----|-------|
| **Resource Allocation** | **0.9687** | Best |
| Jaccard | 0.9637 | Good |
| Adamic–Adar | 0.9623 | Good |
| Common Neighbors | 0.9574 | Strong |
| Preferential Attachment | 0.8428 | Weak |

---

### 🔹 Machine Learning Models  
| Model | AUC | Notes |
|-------|------|--------|
| **Random Forest** | **0.992** | Best model *(Mạnh nhất)* |
| XGBoost | 0.981 | Stable |
| Neural Network | 0.970 | Strong |
| Logistic Regression | 0.968 | Baseline |

**Resource Allocation is the most important feature.**  
*(RA là độ đo quan trọng nhất trong mô hình ML.)*

---

## 🎯 Applications *(Ứng dụng)*  
- 🎬 Artist pairing recommendation for gameshows  
  *(Gợi ý nghệ sĩ hợp tác cho gameshow)*  
- 🧑‍💼 Support for producers & casting teams  
  *(Hỗ trợ nhà sản xuất chọn nghệ sĩ)*  
- 📊 Collaboration trend analysis  
  *(Phân tích xu hướng hợp tác trong giới giải trí)*  
- 🤖 Foundation for social graph AI systems  
  *(Nền tảng cho các hệ thống AI dự đoán mạng xã hội)*  

---

## 📦 Installation *(Cài đặt)*  

```bash
pip install -r requirements.txt
python src/similarity/run_similarity.py
python src/ml/train_models.py
python src/recommend/recommend_topk.py
```
##👥 Authors (Tác giả)

Mai Thanh Phúc

Hoàng Thị Yến Nhi

Trần Trọng Thành

Supervisor: Lê Nhật Tùng (GVHD)

##📚 Citation (Trích dẫn)

Mai Thanh Phúc, Hoàng Thị Yến Nhi, Trần Trọng Thành, Lê Nhật Tùng.
Artist Co-Appearance Prediction and Partner Recommendation in Vietnamese Gameshows.
HUTECH University.
