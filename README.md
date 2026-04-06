# BÀI TẬP LỚN MÔN HỌC: Deep Learning (CO3133)

**Lớp:** A01  
**Học kỳ:** 252  
**Năm học:** 2025-2026

## Giảng viên hướng dẫn (GVHD)

- Họ tên: TS. Lê Thành Sách
- Email: <ltsach@hcmut.edu.vn>

## Thông tin các thành viên nhóm

| Họ tên              | Mã số sinh viên | Email                            |
| ------------------- | --------------- | -------------------------------- |
| Lê Quang Dũng       | 2310548         | <dung.lequang10548@hcmut.edu.vn> |
| Nguyễn Ngọc Tài Em  | 2111091         | <em.nguyenddtk21@hcmut.edu.vn>   |
| Trần Vĩnh Dũng      | 2310574         | <dung.tranvinh2005@hcmut.edu.vn> |
| Nguyễn Công Minh    | 2312080         | <minh.nguyennnn0410@hcmut.edu.vn>|

## Mục tiêu của bài tập lớn

- Vận dụng mô hình pretrained (CNN, ViT, RNN, Transformer, mô hình đa phương
thức) để giải bài toán phân loại trên dữ liệu ảnh, văn bản và đa phương thức.
- Chuẩn bị dữ liệu (Dataset, DataLoader), áp dụng augmentation phù hợp và thiết lập
quy trình huấn luyện/đánh giá.
- So sánh và phân tích kết quả giữa các họ mô hình (CNN vs. ViT, RNN vs. Transformer,
zero-shot vs. few-shot) qua bảng số liệu và biểu đồ.
- Trình bày và bảo vệ kết quả qua báo cáo, video demo và video trình bày; tổ chức mã
nguồn và tài liệu trên GitHub Pages.
- (Tùy chọn) Mở rộng bằng kỹ thuật giải thích mô hình (interpretability) hoặc hướng
tiếp cận khác để nâng cao điểm số

## Hướng dẫn chạy notebook

1. **Yêu cầu môi trường:**

   - Google Colab (khuyến nghị) hoặc môi trường Python 3.12+
   - Các thư viện cần thiết sẽ được cài tự động trong notebook:
     - scikit-learn
     - pandas
     - numpy
     - scipy
     - plotly
     - seaborn
     - torch, torchvision
     - wget

## 2. Cách tải dữ liệu

- **Tập dữ liệu Sports Image - Image Classification**  
  - Được tải tự động trong notebook từ Kaggle.  
  - Bao gồm các tập **train**, **validation**, **test** đã chuẩn bị sẵn.  
  - Link gốc: [Sports Image - Image Classification](https://www.kaggle.com/datasets/sheikhzaib/sports-image-image-classification)  

- **Tập dữ liệu Patent Classification**  
  - Được tải tự động trong notebook từ Hugging Face Datasets.  
  - Dùng cho bài toán phân loại sáng chế đa lớp.  
  - Bao gồm các tập **train**, **validation**, **test**, mỗi mẫu chứa mô tả sáng chế và nhãn tương ứng.  
  - Link gốc: [MAdAiLab/patent_classification](https://huggingface.co/datasets/MAdAiLab/patent_classification)
3. **Chạy notebook bằng Google Colab:**
   1. Mở notebook trên Google Colab.
   2. Chọn **Runtime** → **Run all**.
   3. Toàn bộ quy trình (cài thư viện, tải dữ liệu, huấn luyện, đánh giá) sẽ chạy tự động.
4. **Chạy notebook local:**
   1. Tạo virtual environment (khuyến nghị):

      ```bash
      python -m venv venv
      source venv/bin/activate   # Linux/Mac
      venv\Scripts\activate      # Windows
      ```

   2. Cài đặt dependencies:

      ```bash
      pip install -r requirements.txt
      ```

   3. Chạy notebook bằng Jupyter:

      ```bash
      cd notebooks
      jupyter notebook notebook_name.ipynb
      ```

## Cấu trúc thư mục dự án

```text
DL-Assignment-DDME/
├── docs/            # Thông tin Github Page
├── notebooks/       # Notebook Jupyter để cấu hình và chạy
└── README.md        # Tài liệu này
```

## Báo cáo và notebook Colab

1. **Notebook Image Classification (Sports Image - Image Classification):**

   - Pipeline: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/leequangduxng/ML-Assignment-DDME/blob/main/notebooks/BTL1_Image_classification.ipynb)

2. **Notebook Text Classification (Patent Classification):**

   - Pipeline truyền thống: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/leequangduxng/ML-Assignment-DDME/blob/main/notebooks/BTL1_Text_classification.ipynb)