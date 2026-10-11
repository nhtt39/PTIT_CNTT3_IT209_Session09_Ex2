
# Bài thực hành Docker Nginx

## 1. Khởi chạy container

Lệnh sử dụng:

```bash
docker run -d -p 8080:80 --name my-web nginx:alpine
```

Kết quả: Container `my-web` được khởi chạy ở chế độ nền, sử dụng image `nginx:alpine` và ánh xạ cổng `8080:80`.

(ảnh 1)
## 2. Kiểm tra web server

Lệnh kiểm tra:

```bash
curl http://localhost:8080
```

Kết quả mong đợi: Phản hồi HTML chứa dòng chữ `Welcome to nginx!`.

(ảnh 2)
## 3. Dừng và xóa container

Lệnh sử dụng:

```bash
docker stop my-web && docker rm my-web
```

Kết quả: Container `my-web` được dừng và xóa thành công.

(ảnh 3)
