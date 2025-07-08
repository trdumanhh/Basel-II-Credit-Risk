# Basel-III-Credit-Risk

Dự án này xây dựng mô hình chấm điểm tín dụng nhằm ước lượng Xác suất vỡ nợ (Probability of Default - PD) cho từng khách hàng, sử dụng dữ liệu đầu vào và các phương pháp phân tích thống kê. Quy trình bao gồm từ tiền xử lý dữ liệu đến xây dựng mô hình, đánh giá và giám sát sau triển khai.

1. Tiền xử lý dữ liệu (Run script Data Preparation)

- Làm sạch dữ liệu và xử lý giá trị thiếu (missing values).

- Thực hiện chuẩn hóa (normalization) cho các biến liên tục để đảm bảo mô hình ổn định.

2. Phân tích dữ liệu và biến đầu vào
- Phân loại các biến thành biến phân loại và biến liên tục.

- Áp dụng kỹ thuật Fine Classing, tính Weight of Evidence (WoE) và Information Value (IV) để đánh giá sức mạnh dự báo của từng biến.

3. Xây dựng mô hình
- Sử dụng Logistic Regression để ước lượng Probability of Default (PD) cho từng khách hàng.

- Lựa chọn biến đầu vào dựa trên giá trị IV, kiểm tra đa cộng tuyến (multicollinearity) và ý nghĩa kinh doanh.

4. Tạo bảng điểm tín dụng (Scorecard)
- Chuyển đổi đầu ra của mô hình thành thang điểm tín dụng (scorecard) bằng kỹ thuật binning và scale điểm.

- Scorecard ra quyết định tín dụng và định giá rủi ro theo hồ sơ khách hàng.

5. Đánh giá mô hình

Đánh giá độ chính xác và phân biệt mô hình thông qua:

- Đường cong ROC và AUC

- KS Statistic

- Gini Index

- Kiểm tra hiện tượng overfitting và tính ổn định mô hình trên tập huấn luyện và kiểm định.

6. Giám sát mô hình sau triển khai
- Theo dõi Population Stability Index (PSI) để phát hiện sự thay đổi trong phân bố dữ liệu khách hàng theo thời gian.

- Cảnh báo sớm khi có dấu hiệu thay đổi hành vi khách hàng để chuẩn bị cho việc điều chỉnh mô hình.
