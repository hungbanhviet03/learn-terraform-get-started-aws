# Học Terraform - Bắt Đầu Với AWS

Dự án này minh họa cách sử dụng Terraform để provision một instance EC2 trên AWS. Nó sử dụng provider AWS để tìm AMI Ubuntu mới nhất và tạo một instance t3.micro.

## Yêu Cầu

- Terraform đã được cài đặt (phiên bản >= 1.2)
- Tài khoản AWS với credentials được cấu hình (ví dụ: qua AWS CLI)
- Region AWS: us-west-2 (có thể thay đổi trong main.tf)

## Hướng Dẫn Sử Dụng

1. Khởi tạo dự án:
   ```
   terraform init
   ```

2. Lập kế hoạch:
   ```
   terraform plan
   ```

3. Áp dụng thay đổi:
   ```
   terraform apply
   ```

4. Xóa tài nguyên (sau khi sử dụng xong):
   ```
   terraform destroy
   ```

## Tài Nguyên Được Tạo

- Một instance EC2 với AMI Ubuntu 24.04, loại t3.micro, tag Name: "learn-terraform"

Lưu ý: Dự án này dành cho mục đích học tập. Hãy đảm bảo xóa tài nguyên để tránh chi phí không mong muốn. 