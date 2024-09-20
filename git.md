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


### working directory (file màu đỏ)
### staging (màu xanh) chỉ xanh mới đưa lên git repo

#### git commit -m
dùng để gắn message vào trong những file đang staging được phép đưa lên remote repo
mỗi commit có 1 id riêng (sha)

## git log
check lịch sử commit

### config git (trước khi chạy)
git config --global user.name "name"
git config --global user.email "abc"

## git push -u origin <tên nhánh>
đưa code lên repo remote
chỉ cần làm lần đầu tiên, mấy lần sau chỉ cần git push

## đưa file về trạng thái staging
git reset
git restore -S . (đưa all file về staging)
git restore -S <url file> (đưa 1 file duy nhất)

### git checkout <url file>
đưa 1 file đang được chỉnh sửa về trạng thái trước đó
### git checkout <tên nhánh>
tương tự git switch

### git checkout -b <tên nhánh>
tạo ra 1 nhánh mới, đồng thời switch qua luôn (git branch + git switch)


# branch
dev: kiếm thử QA và Dev (dev)

staging: QA kiểm thử 1 lần (staging)

production: end user (main/release)

- Git branch <tên nhánh>
tạo ra 1 nhánh mới

- Git branch -a
Liệt kê nhánh


# git pull 
pull code ở repo remote về local
git pull --no-ff

# git clone <url repo>
