# Stock Price Prediction (Dự đoán giá cổ phiếu)
Tags: Khai thác dữ liệu và khai phá tri thức, Nhập môn học máy, Time series prediction, dự đoán chứng khoán (Stock Prediction).

## Đề bài gốc:
Hãy phân tích bài toán đưa ra một giải pháp dựa vào học máy để dự đoán giá trị trong tương lai của một trong loại data sau:
<br/>
**(A)	Dự đoán giá các cổ phiếu.**
<br/>
(B)	Dự đoán giá các hàng hoá.
<br/>
(C)	Dự đoán tỉ lệ tăng trưởng GDP của các nước.

### Đối với giá hàng hoá và cổ phiếu trong tương lai thì dự đoán các mốc thời gian sau:
-	**Dự đoán giá cổ phiếu theo từng ngày trong 14 ngày tiếp theo (theo đồ thị ngày).**
-	Dự đoán giá cổ phiếu theo từng tuần trong tuần trong 7 tuần tiếp theo (theo đồ thị tuần).

### Đối bài toán dự đoán GDP thì dự đoán các mốc sau:
-	Dự đoán 4 quý tiếp theo.
-	Dự đoán 4 năm tiếp theo.

## Các nhiệm vụ (câu hỏi) cần làm:
(1) Thu thập dữ liệu các thông tin liên quan của cổ phiếu (hoặc hàng hoá, hoặc GDP) theo thời gian.
<br/>
(2) Phân tích bài toán để xác định thông tin nào được sử dụng làm đầu vào để dự đoán giá tương lai (Ví dụ đối với giá cổ phiếu, có thể phụ thuộc vào: các loại giá quá khứ, thông tin ngành nghề, thông tin tài chính của công ty, ...).
<br/>
Lưu ý:
  - Phần 2 và phần 1 liên quan đến nhau, khi phần 2 xác định sử dụng loại thông tin nào thì phần 1 thu thập theo các loại thông tin đó.
  -	Nhóm tự quyết định việc sử dụng nhiều hay ít loại thông tin là quyết định riêng của từng nhóm. Về nguyên tắc thì càng nhiều thông tin thì khả năng dự đoán càng chính xác.
<br/>
(3)	Xây dựng các mô hình học máy khác nhau để dự đoán trong đó có 2 thuật toán bắt buộc là: Reccurent Neural Network (RNN) và MultiLayer Perceptron (MLP). Khuyến khích sử dụng thêm các thuật toán khác: SVM, kNN, DT, Random Forest, ... Đánh giá độ tốt (độ chính xác) của các mô hình và so sánh. Đánh giá thời gian huấn luyện và thời gian Testing. Vẽ đồ thị bao gồm giá trị thực và giá trị dự đoán để dễ so sánh.
<br/>
(4)	Sử dụng các phương pháp xử lý vấn đề Overfiting đối với câu hỏi (3) và so sánh với việc không sử dụng Overfiting. Áp dụng trên các models ở câu hỏi (3).
<br/>
(5)	Sử dụng các tập đặc trưng khác nhau (liên quan đến câu hỏi (2)) để tìm ra tập đặc trưng hiệu quả nhất cho bài toán. Tìm đặc trưng quan trọng nhất ảnh hưởng đến sự giá trị của cái phải dự đoán (tức là feature nào ảnh hưởng nhất đến output).
<br/>
(6) Nghiên cứu áp dụng các mô hình Deep Learning để giải quyết bài toán. Ví dụ mô hình LSTM, mô hình CNN, các mô hình kết hợp các phương pháp khác nhau.

## Dataset
Tất cả các tập dữ liệu sử dụng trong bài này, đều được crawl về từ trang Cafef, ví dụ: [Mã CMX trong 'chungkhoangia.csv'](https://s.cafef.vn/Lich-su-giao-dich-CMX-1.chn). Tuy nhiên, Code chỉ gói gọn trong phạm vi của 'chungkhoangia.csv' mà thôi.
