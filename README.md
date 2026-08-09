# Git Homework Buổi 2

Bài tập thực hành kết nối repository local với GitHub.

## Nội dung

Thực hành remote và push repository lên GitHub.

## Git commands

- git remote add
- git remote -v
- git push

  # Git Homework

## Câu 1 : Bạn cần làm gì để kết nối repository local với repository trên GitHub?

Trước tiên cần tạo một repository rỗng trên GitHub. Sau đó thêm remote URL của repository GitHub vào repository local bằng lệnh:

git remote add origin https://github.com/username/repository-name.git

Có thể kiểm tra remote bằng lệnh: git remote -v

## Câu 2 : Vì sao cần remote URL?

Remote URL là địa chỉ của repository trên GitHub. Git cần địa chỉ này để biết repository local sẽ kết nối và push dữ liệu lên repository nào.

## Câu 3 : Vì sao lần push đầu tiên thường dùng git push -u origin main?

Lần push đầu tiên thường sử dụng: git push -u origin main

Trong đó origin là tên của remote và main là branch cần push. Tùy chọn -u thiết lập upstream giữa branch local main và branch main trên GitHub.

## Câu 4 : Sau lần push đầu tiên, các lần sau có thể dùng lệnh ngắn hơn không? Vì sao?

Sau lần push đầu tiên, có thể dùng lệnh ngắn hơn: git push

Vì khi sử dụng git push -u origin main, Git đã lưu mối liên hệ giữa branch local và branch trên remote. Những lần sau Git biết cần push lên đâu nên không cần ghi lại origin main.
