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