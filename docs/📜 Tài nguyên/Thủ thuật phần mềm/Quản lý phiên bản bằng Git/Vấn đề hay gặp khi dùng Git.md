---
share: True
---
# Quên add

# [[../../../⚡Hiểu biết sâu/Khoa học máy tính/Hợp tác làm việc/Git không biết gì về folder|Git không biết gì về folder]]

# Thêm file vào  .gitignore rồi mà vẫn không thấy file bị ignore

# Lỡ commit file nặng
```
git filter-branch --force --index-filter 'git rm -r --cached --ignore-unmatch bigfile.txt' --prune-empty --tag-name-filter cat -- --all
```
