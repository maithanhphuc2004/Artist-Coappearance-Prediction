# 🎭 Artist Co-Appearance Prediction  
*Dự đoán sự xuất hiện chung & gợi ý đối tác cho nghệ sĩ trong gameshow Việt Nam*

![Python](https://img.shields.io/badge/Python-3.10+-blue?style=flat-square&logo=python)
![Similarity-RA](https://img.shields.io/badge/Similarity-Resource%20Allocation-blueviolet?style=flat-square)
![Similarity-Jaccard](https://img.shields.io/badge/Similarity-Jaccard-green?style=flat-square)
![Similarity-AA](https://img.shields.io/badge/Similarity-Adamic–Adar-orange?style=flat-square)
![Similarity-CN](https://img.shields.io/badge/Similarity-Common%20Neighbors-yellow?style=flat-square)
![Similarity-PA](https://img.shields.io/badge/Similarity-Preferential%20Attachment-red?style=flat-square)

![Model-RandomForest](https://img.shields.io/badge/Model-Random%20Forest-darkgreen?style=flat-square)
![Model-XGBoost](https://img.shields.io/badge/Model-XGBoost-red?style=flat-square)
![Model-LogisticRegression](https://img.shields.io/badge/Model-Logistic%20Regression-blue?style=flat-square)
![Model-NeuralNetwork](https://img.shields.io/badge/Model-Neural%20Network-purple?style=flat-square)


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
