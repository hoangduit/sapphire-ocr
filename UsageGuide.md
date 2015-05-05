## Dịch mã nguồn ##

Sử dụng IDE ưa thích của bạn, tạo project và pull (sử dụng chế độ clean update) mã nguồn về đè lên thư mục project.

Thêm các file .jar trong thư mục lib vào build path của project.

## Cấu trúc chương trình ##

  * MainFrame: entry point của chương trình demo, cái này chạy không chính xác (chưa tìm ra lỗi)
  * NeuralNetworkTrainer: chương trình huấn luyện, thay đổi tên file trong mã nguồn và chạy (khá lâu)
  * SamplePreparer: chuyển dữ liệu thô (ảnh + mã kí tự) thành tệp dữ liệu huấn luyện dạng YAML

## Thuật toán ##

  1. Trích chọn đặc trưng: chuyển ảnh nhị phân thành dãy các tham số Fourier
  1. Nhận dạng: dùng các tham số làm đầu vào của mạng nơ-ron, đầu ra là một dãy các bit 0-1
  1. Giải mã: chuyển dãy các đầu ra của mạng thành mã unicode của kí tự