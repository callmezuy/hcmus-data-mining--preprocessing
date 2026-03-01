# Bài Tập Thực Hành 01: Tiền Xử Lý Dữ Liệu
## Khai Phá Dữ Liệu và Ứng Dụng

### Thông Tin Nhóm
- **Mã nhóm:** 05
- **Thành viên:**
  - Bùi Minh Duy - 23127040
  - Phi Anh Khôi - 23127073
  - Lê Minh Đức - 23127351

### Tổng Quan Bài Tập
Dự án này tập trung vào các kỹ thuật tiền xử lý dữ liệu cho các loại dữ liệu khác nhau:
- **Phần 1 (Bắt buộc):** Tiền xử lý dữ liệu hình ảnh
- **Phần 2 (Bắt buộc):** Tiền xử lý dữ liệu dạng bảng
- **Phần 3/4 (Bonus - Chọn một):** Tiền xử lý dữ liệu văn bản hoặc dữ liệu thời gian

### Bộ Dữ Liệu Sử Dụng

#### Phần 1: Dữ Liệu Hình Ảnh
- **Tên dataset:** Chest X-Ray Pneumonia
- **Nguồn:** https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia
- **Mô tả:** 5.863 ảnh X-quang ngực (JPEG) thuộc 2 lớp: Pneumonia và Normal, được chia thành tập train/test/val

#### Phần 2: Dữ Liệu Dạng Bảng
- **Tên dataset:** Car Resale Data - 2023
- **Nguồn:** https://www.kaggle.com/datasets/rahulmenon1758/car-resale-prices
- **Mô tả:** 17.446 bản ghi với 15 thuộc tính về các xe ô tô đã qua sử dụng tại Ấn Độ (giá, động cơ, tiêu hao nhiên liệu, loại nhiên liệu, v.v.); biến mục tiêu là resale_price

#### Phần 3: Dữ Liệu Văn Bản (Bonus)
- **Tên dataset:** IMDB Dataset of 50K Movie Reviews
- **Nguồn:** https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews
- **Mô tả:** 50.000 đánh giá phim từ IMDB được gán nhãn tích cực (positive) hoặc tiêu cực (negative) cho bài toán phân tích cảm xúc

#### Phần 4: Dữ Liệu Thời Gian (Bonus)
- **Tên dataset:** NASDAQ Stock Market Data (AAPL)
- **Nguồn:** https://www.kaggle.com/datasets/jacksonce/stock-market-dataset
- **Mô tả:** Dữ liệu giá cổ phiếu AAPL theo ngày từ năm 1980 đến 2022 (hơn 40 năm) bao gồm Open, High, Low, Close, Adjusted Close và Volume

### Cấu Trúc Dự Án
```
Lab01/
├── README.md                          # File này
├── requirements.txt                   # Các thư viện Python cần thiết
├── data/                             # Thư mục dữ liệu
│   ├── images/                       # Dữ liệu hình ảnh
│   ├── tabular/                      # Dữ liệu dạng bảng
│   ├── text/                         # Dữ liệu văn bản (nếu có)
│   └── temporal/                     # Dữ liệu chuỗi thời gian (nếu có)
├── notebooks/                        # Jupyter notebooks
│   ├── 01_image_preprocessing.ipynb         # Phần 1 (Bắt buộc)
│   ├── 02_tabular_preprocessing.ipynb       # Phần 2 (Bắt buộc)
│   ├── 03_text_preprocessing.ipynb          # Phần 3 (Bonus)
│   └── 04_temporal_preprocessing.ipynb      # Phần 4 (Bonus)
└── docs/                             # Tài liệu
    └── Report.pdf                     # Báo cáo cuối kỳ
```

### Hướng Dẫn Cài Đặt

#### 1. Tạo Môi Trường Ảo Python (Khuyến nghị)

Môi trường ảo giúp cách ly các thư viện của dự án, tránh xung đột với các dự án khác.

```bash
# Di chuyển đến thư mục dự án
python -m venv .venv

# Kích hoạt môi trường ảo
# Trên Windows:
.venv\Scripts\activate

# Trên macOS/Linux:
source .venv/bin/activate
```

#### 2. Cài Đặt Các Thư Viện Python

Sau khi kích hoạt môi trường ảo:

```bash
# Nâng cấp pip trước (khuyến nghị)
python -m pip install --upgrade pip

# Cài đặt tất cả các thư viện cần thiết
pip install -r requirements.txt
```

#### 3. Tải Dữ Liệu

- Tải toàn bộ dữ liệu từ link Google Drive bên dưới:
  - **Google Drive:** https://drive.google.com/drive/folders/1ktw0bJKU2pjxvoPSB1UC9_NDBxa3u5qO
- Đặt dữ liệu vào các thư mục con tương ứng trong `data/`:
  - `data/images/` - dữ liệu hình ảnh
  - `data/tabular/` - dữ liệu dạng bảng
  - `data/text/` - dữ liệu văn bản
  - `data/temporal/` - dữ liệu chuỗi thời gian

### Chạy Notebooks

1. Di chuyển đến thư mục dự án
2. Khởi động Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
3. Mở các notebook trong thư mục `notebooks/`:
   - `01_image_preprocessing.ipynb` (Bắt buộc - Phần 1)
   - `02_tabular_preprocessing.ipynb` (Bắt buộc - Phần 2)
   - `03_text_preprocessing.ipynb` (Bonus - Phần 3)
   - `04_temporal_preprocessing.ipynb` (Bonus - Phần 4)

   **Lưu ý:** Chỉ chọn một trong Phần 3 hoặc Phần 4 cho phần bonus

### Thông Tin Môn Học
- **Giảng viên:** ThS. Lê Nhựt Nam
- **Email:** lnnam@fit.hcmus.edu.vn

### Lưu Ý
- **Notebook 1 (Tiền xử lý hình ảnh):** Do giới hạn phần cứng, `01_image_preprocessing.ipynb` có thể không chạy được trên một số máy. Thầy có thể truy cập link GitHub bên dưới để xem output đã được chạy sẵn. Do giới hạn dung lượng, nhóm không thể nộp notebook kèm output lên Moodle:
  - **GitHub:** https://github.com/callmezuy/hcmus-data-mining--preprocessing

### Giấy Phép
Dự án này chỉ phục vụ mục đích học tập trong khuôn khổ môn CSC14004 - Khai phá dữ liệu và ứng dụng tại Trường Đại học Khoa học Tự nhiên, ĐHQG-HCM.

