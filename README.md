# Hệ Thống Nhận Diện Mệnh Giá Tiền Việt Nam (Banknote Recognition)

Dự án này sử dụng mạng nơ-ron tích chập (CNN) được xây dựng từ đầu (scratch) để phân loại 11 mệnh giá tiền tệ đang lưu hành tại Việt Nam. Mô hình được tối ưu hóa để nhận diện chính xác các đặc trưng về màu sắc và hoa văn trên các tờ tiền Polymer và tiền giấy.


## Tải Xuống Mô Hình Pre-trained

Do giới hạn dung lượng file trên GitHub, file trọng số mô hình `.h5` được lưu trữ tại Google Drive. Bạn có thể tải về để sử dụng ngay mà không cần huấn luyện lại:

👉 [**Tải file mo_hinh_nhan_dien_tien_50_epochs2.h5 tại đây**](https://drive.google.com/file/d/148glXrFQ_64CmSMdZCvfsmUkDTkMOCmd/view?usp=drive_link)

---

## 📂 Cấu Trúc Thư Mục Dự Án

*   `AI_Banknotes.ipynb`: File Google Colab chứa toàn bộ mã nguồn từ xử lý dữ liệu đến huấn luyện.
*   `test_file/`: Thư mục chứa các hình ảnh mệnh giá tiền thực tế dùng để kiểm thử (Test).
*   `README.md`: Hướng dẫn và thông tin dự án.

---

## 🛠️ Cách Chạy Mô Hình

Bạn có thể nạp lại mô hình trong môi trường Python/Colab bằng lệnh sau:

```python
from tensorflow.keras.models import load_model

# Load model từ file đã tải về
model = load_model('mo_hinh_nhan_dien_tien_50_epochs2.h5')

# Dự đoán ảnh mới
# predictions = model.predict(img_prepared)
print("✅ Mô hình Banknote đã sẵn sàng!")
