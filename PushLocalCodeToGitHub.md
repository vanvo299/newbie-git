// Cách đưa một thư mục code mới lên github
‌echo "# abcxyz" >> README.md
git init
git add .
git commit -m "first commit"
git branch -M main
git remote add origin <link http cua repo>
git push -u origin main

// Cách tạo một nhánh mới
- git checkout -b ten_nhanh_moi : tạo một nhánh mới và chuyển đến nhánh đó ngay lập tức
- git branch ten_nhanh_moi : chỉ tạo nhánh mà không chuyển đến nhánh đó
Sau khi tạo nhánh, bạn có thể chuyển đến nhánh mới bằng cách sử dụng : git checkout ten_nhanh_moi
- git branch : xem danh sách nhánh mới 
- git status : Xem trạng thái hiện tại 
- git log --oneline --graph --decorate --all : Xem lịch sử commit của nhánh hiện tại 

- Merge nhánh chính vào nhánh riêng
+ git checkout VoLuong : Chuyển đến nhánh của bạn
+ Cập nhật nhánh chính từ xa:
    git checkout main
    git pull origin main
+ Chuyển lại đến nhánh của tôi: 
    git checkout VoLuong
+ Merge nhánh chính vào nhánh của bạn (lấy code của nhánh main về nhánh riêng)
    git merge main

- Update sự thay đổi từ nhánh riêng lên nhánh main
1. git add <ten file thay doi>
2. git commit -m "noi dung thay doi"
3. Chuyển sang nhánh chính main
    git checkout main
4. cập nhật nhánh main (nếu cần) :
    git pull origin main
5. merge nhánh riêng vào nhánh chính
    git pull VoLuong
6. Đẩy các thay đổi lên remote repository 
    git push origin main 