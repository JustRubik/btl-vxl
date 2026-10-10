# UAV-3

Đây là dự án bài tập lớn của môn Kĩ thuật Vi xử lý ET3300, Đại học Bách khoa Hà Nội, lớp của thầy Hàn Huy Dũng.

---

## Mô tả về dự án

### Tóm tắt

- Mã dự án: `UAV-3`
- Tên dự án: Đọc cảm biến IMU (MPU6050) qua I2C, xử lý góc nghiêng cơ bản.
- Kiến thức vi xử lý chính: I2C, xử lý dữ liệu cảm biến quán tính, bộ lọc số cơ bản, định thời bằng timer.

### Chi tiết

- Mục tiêu: Giao tiếp I2C đọc dữ liệu gia tốc/con quay hồi chuyển từ MPU6050, tính góc roll/pitch bằng bộ lọc bù (complementary filter) đơn giản với tần số lấy mẫu ổn định.
- Kiến thức vi xử lý chính: I2C, xử lý dữ liệu cảm biến quán tính, bộ lọc số cơ bản, định thời bằng timer.
- Gợi ý phần cứng/công cụ: STM32/ESP32 + MPU6050.
- Sản phẩm đầu ra: 
    - Firmware đọc IMU
    - Hiển thị góc nghiêng thời gian thực.

### Yêu cầu báo cáo bài tập lớn

#### Yêu cầu về quy trình

- Lên ý tưởng muốn giải quyết
- Xây dựng các yêu cầu chức năng/ phi chức năng đặt ra cho hệ thống
- So sánh và lựa chọn linh kiện -> sơ đồ hệ thống
- Demo sản phẩm và kiểm thử
- Thu thập dữ liệu và xây dựng thuật toán xử lý
- Đánh giá và bàn luận

#### Yêu cầu về con người

* Sinh viên:

    - Thực hiện báo cáo đúng tiến độ
    - Học hỏi yêu cầu kĩ thuật để phát triển một dự án hoàn chỉnh

* Thành viên hướng dẫn:

    - Thực hiện giám sát báo cáo đúng tiến độ
    - Thực hiện dạy học các buổi sâu hơn về VXL và thuật toán

* Hạn chế: 

    - Thông tin cho vào báo cáo không uy tín (báo lá cải/ chatGPT - AI agent/ wikipedia)
    - Sử dụng mã nguồn mở nhưng không hiểu quy trình thực hiện, nguyên lí hoạt động
    - Trình bày đúng quy trình kĩ thuật
    - Làm giả số liệu

#### Nhật kí kĩ thuật

- Theo dõi tiến độ dự án
- Theo dõi đóng góp của từng thành viên
- Bản sơ thảo cho báo cáo cuối cùng

> *100-200 Trang nhật kí (10-12 tuần)* 
*60-80 Trang báo cáo (bản thảo cuối)*

Link nhật kí: [Diary](https://drive.google.com/drive/folders/1AB1z0dgDd2E_Kyk2Xti61ocO_1wpGeU4?usp=sharing)

---

## Cấu trúc thư mục

Xem thêm trong [docs/internals/architectures.md](./docs/internals/architectures.md)

```Tree
Project
├── docs/               # Nơi lưu tài liệu dự án
├── libs/               # Thư viện ngoài của dự án
├── src/                # Mã nguồn dự án
├── Makefile            # Make scripts
├── .gitignore          # Xem thêm tài liệu về git
├── LICENSE             # License của dự án
└── README.md           # File giới thiệu của dự án
```

## License
Copyright (c) 2026 JustRubik.

This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version. See [LICENSE](LICENSE) for the full text.

Chương trình này là phần mềm tự do: bạn có thể phân phối lại và/hoặc sửa đổi nó theo các điều khoản của Giấy phép Công cộng GNU (GNU General Public License) do Tổ chức Phần mềm Tự do (Free Software Foundation) công bố, cụ thể là phiên bản 3 của Giấy phép này hoặc (tùy chọn) bất kỳ phiên bản nào sau đó. Vui lòng xem [LICENSE](LICENSE) để biết toàn văn giấy phép.
