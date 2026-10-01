# Bài 2: Khởi tạo User thường và thiết lập đặc quyền quản trị

## 1. Mục tiêu bài thực hành

Bài thực hành thực hiện việc tạo một tài khoản người dùng thường trên
Ubuntu Server để hạn chế việc sử dụng trực tiếp tài khoản `root` trong
quá trình vận hành hệ thống.

User được tạo có tên là `devops`. Sau khi tạo, user này sẽ được cấp
quyền quản trị thông qua nhóm `sudo`.

Bên cạnh đó, bài thực hành thực hiện cấu hình SSH Key cho user `devops`,
phân quyền cho thư mục `.ssh` và file `authorized_keys`, sau đó kiểm tra
khả năng đăng nhập SSH và quyền quản trị của user.

## 2. Tạo user devops

### 2.1. Kiểm tra user trước khi tạo

Trước tiên kiểm tra xem user `devops` đã tồn tại trên Ubuntu Server hay chưa:

```bash

