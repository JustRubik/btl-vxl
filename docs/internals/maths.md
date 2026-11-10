# Maths

File này mô tả toàn bộ các công thức toán học được sử dụng trong dự án.

## Về phần cứng

### STM32

Dùng để **lấy dữ liệu** được gửi về từ `MPU6050`, gồm: `Acceleration` và `Gyro Value`.
Và, dùng để **đẩy dữ liệu** lên `máy tính` để xử lý (trong trường hợp chỉ demo).
Đồng thời cũng dùng để **lấy dữ liệu** rồi xử lý sau.

### MPU6050

Đo đạc các trục của thông số về `gia tốc` và `gyro`.

## Về giá trị mà MPU6050 đo đạc

MPU6050 sẽ trả về 6 giá trị: 3 giá trị gia tốc theo trục x, y, z và 3 giá trị vận tốc góc.
