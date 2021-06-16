# Hướng dẫn học git

B1: Tạo dự án trên github
B2: clone code
    git clone [link]
B3: Checkout về nhánh master (nếu đang ở một nhánh khác)
    git checkout master
B4: Đứng ở nhánh master và checkout ra một nhánh mới
    git checkout -b [tên nhánh mới]
    Hoặc
    git branch [tên nhánh mới]
    git checkout [tên nhánh mới]
B5: Code ở nhánh mới
B6: Kiểm tra những files thay đổi nội dung 
    git status
B7: Sau khi code xong, thêm những file ở working directory vào staging area
    git add [directory/tên file]
B8: Kiểm tra những files đã được thêm vào staging area
    git status
B9: (Trường hợp muốn đưa file từ staging area về working directory)
    git rm --cached [directory/tên file]
B10: Đưa những files đang ở staging vào git directory
    git commit -m'[Ghi thông điệp vào]' //Thêm commit và thông điệp về commit đó
    ------------
    git commit --amend //Thêm file vào commit cũ
    git commit --amend -m'[Ghi thông điệp vào]'  //Vừa thêm file vào commit cũ, vừa đổi thông điệp
B11: Đẩy file lên github
    git push origin [tên nhánh]

    git push origin [tên nhánh] -f //Nếu có conflict với commmit trên github

B12: Tạo pull request và merge vào nhánh thích hợp (master)

B13: Review code cùng team

B14: Merge code (sau khi đảm bảo code tính năng đó hoàn thiện hoặc fix được bug)

LẤY CODE MỚI NHẤT VỀ LOCAL

B15: Xóa nhánh cũ trên local (Đảm bảo nhánh mình đang đứng không phải là nhánh cần xóa)
    git branch -D [tên nhánh cũ] //Nhánh cũ đơn giản nhất mình làm là master

B16: Lấy code mới nhất trên github về local
    git fetch origin [tên nhánh] //master

B17: Checkout về nhánh mới nhất
    git checkout [tên nhánh] //master

B18: Lặp lại từ B5


**NÂNG CAO**

Tiếp tục từ bước 16

B17: Sau khi lấy code mới nhất về (nhánh master có code mới nhất), ta tiến hành "gắn đốt tre" vào nhánh hiện tại (để đảm bảo nhánh hiện tại cũng có code mới nhất giống master)
    git rebase master

B18: Checkout về master
    git checkout master
B19: Lặp lại từ B5

**NÂNG CAO HƠN NỮA**
( To be continue :)) )


