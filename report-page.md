# Report 1 Page – FIT4012 Lab 1

## 1. Mục tiêu
Tóm tắt ngắn gọn mục tiêu của bài lab.

## 2. Cách làm
- Đọc hiểu chương trình entropy mẫu.
- Bổ sung hàm tính redundancy.
- Hoàn thiện hàm mod_inverse().
- Chạy thử trên nhiều test case.

## 3. Kết quả chính
### 3.1 Entropy và redundancy
| Input | Entropy | Redundancy | Nhận xét |
|---|---:|---:|---|
| aaaa | 0 | 8 | Không có thông tin bất ngờ, độ dư thừa tối đa |
| abcd | 2 | 6 | Ký tự xuất hiện duy nhất và đều nhau, độ phức tạp tăng lên |
| hello world | 2.84535 | 5.15465 | Chuỗi đa dạng ký tự nhất, entropy cao nhất và ít dư thừa nhất |

### 3.2 Modulo inverse
| a | m | Kết quả mong đợi | Kết quả chương trình |
|---:|---:|---|---|
| 3 | 7 | 5 | 5 |
| 10 | 17 | 12 | 12 |
| 6 | 9 | Không tồn tại | Không tồn tại |

## 4. Kết luận
Qua bài lab, em đã nắm vững cách định lượng thông tin qua Entropy/Redundancy và triển khai thuật toán Euclid mở rộng để tìm nghịch đảo modulo. Khó khăn lớn nhất là việc xử lý số dư âm trong lập trình và kiểm soát luồng biến $x, y$ khi đệ quy. Tuy nhiên, việc trực tiếp so sánh các chuỗi lặp như aaaa giúp em hiểu rõ Entropy là "độ bất ngờ",giúp em thấu hiểu bản chất toán học của nghịch đảo modulo.