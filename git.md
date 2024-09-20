## tạo repo : 
git init
nhánh chính: master

### tạo repo đồng bộ vs github
git init -b main

U: untracked, chưa track dc file

## link repo local với repo remote
git remote add origin + url repo

## trước khi commit hay push thì nên xóa file node_modules

### file .gitignore sẽ quy định những file không được phép đẩy lên repo
file .gitignore phải nằm ở thư mục root

### git status
check dự án

## git add (git add -A, git add .)
-A: add all files trong project
. : add cụ thể 1 thư mục đang đứng
add : thêm 1 thư mục cụ thể


### demo git conflict