# Adversarial Deep Learning for Voice Activity Detection

Trong dự án này, tôi đã thực hiện sử dụng mô hình Deep Learning để thực hiện nhiệm vụ VAD trong môi trường có độ nhiễu tiếng ồn cao (SNR = -10dB, 0dB, 10dB).


Mô hình gồm 3 module chính:

1. Encoder 
2. Decoder
3. Adversarial Block


Khảo sát với bộ dữ liệu TIMIT cho thấy mô hình đạt kết quả tốt với điểm AUC cao > 85/100.

Tôi cũng thực hiện triển khai những phiên bản hiệu chỉnh của mô hình:

1. Loại bỏ khối Adersarial Block để tạo ra mô hình Encoder - Decoder truyền thống.
2. Loại bỏ khối Decoder Block để giúp giảm độ trể thuật toán và xem xét liệu việc loại bỏ khối này có làm giảm độ chính xác của mô hình.

Ngoài ra, tôi cũng triển khai thêm thuật toán "Butterworth filter" để so sánh hiệu quả giữa thuật toán học sâu và các thuật toán truyền thống.