"# Setup" 
các thư mục trong này chứa file docker-compose.yml, file .env, file dataset dùng để setup service trên docker desktop
- đọc file setup trong từng thư mục. 

Cách dùng như sau.
    - Thay đổi đường dẫn directory trong file .env bằng đường dẫn của một thư mục trong bất kỳ (tránh đặt trong ổ C)
    - Trong Terminal của Docker desktop, cd directory đến thư mục chứa file docker-compose.yml
    - chạy câu lệnh "docker compose --env-file .env up -d"

Đối với các Database service (MongoDB, Redis, ...) => Tùy theo đặc thù của từng DB để dùng dataset khôi phục lại dữ liệu