# GITHUB
### I.Cách hoạt động của Github
GitHub là sự kết hợp giữa 2 từ, Git – hệ thống quản lý dự án và phiên bản code và Hub – một mạng xã hội cho lập trình viên.
Github là một dịch vụ lưu trữ dựa trên web cho các dự án phát triển phần mềm trong đó sử dụng các hệ thống kiểm soát phiên bản Git.
***
### II.Các khái niệm
* Add
  > Lưu file thay đổi
* Remove
  > Để xóa một thư mục hay một file nào đó có thể xóa ở máy local.
* Commit
  > Để ghi lại việc thêm/ thay đổi file hay thư mục vào repository thì sẽ thực hiện thao tác gọi là Commit.
* Push
  > Dùng để đưa nội dung cập nhật từ local lên server.
* Pull
  > Dùng để gộp những thay đổi mới kéo về từ máy chủ từ xa với nhánh hiện tại trên máy local.
* Fetch
  > Dùng để truy cập vào một repository nào đó và cập nhật dữ liệu repository đó.
* Clone
  > Dùng để sao chép remote repository.
* Fork
  > Dùng để copy của một repository
* Star
  > Dùng để nhận biết nhưng quan tâm đế repo đó.
* Watch
  > Dùng để nhận thông báo về sự thay đổi của một repo.
***
### III.Các lệnh trong Github
1. Setting up git
  * Tải và cài đặt git
    * `https://git-scm.com/download/win`
  * Thiết lập name và email trong git
    * `git config --global user.name "username"`
    * `git config --global user.email "email@example.com"`
2. Generate and add SSH key
  * Mở terminal nhập lệnh:
    * `ssh-keygen -t rsa -b 4096 -C "email@example.com"`
    * `Enter file in which to save the key (/Users/binhcq/.ssh/id_rsa):` nhấn Enter để cài đặt ở mặc định
  * Nhập mật khẩu cho key:
    * `Enter passphrase (empty for no passphrase):` nhập mật khẩu
    * `Enter same passphrase again:` nhập lại mật khẩu
  * Thêm key vào ssh-agent
    * `eval “$(ssh-agent -s)”` kích hoạt ssh-agent
    * `ssh–add ~/.ssh/id_rsa` add key vào ssh-agent
  * Thêm SSH Public key vào tài khoản trên server
    * `pbcopy < ~/.ssh/id_rsa.pub` Copy ssh key vào clipboard
    * `ssh -T git@github.com` kiểm tra
3. Caching -your GitHub password in Git
  * Nếu clone repository GitHub bằng HTTPS, bạn có thể sử dụng trình trợ giúp thông tin xác thực để Git nhớ tên người dùng và mật khẩu GitHub của bạn mỗi khi nói chuyện với GitHub.
   * Nếu bạn clone repository bằng SSH, thì bạn xác thực bằng khóa SSH thay vì tên người dùng và mật khẩu. Để được trợ giúp thiết lập kết nối SSH, hãy xem Tạo Khóa SSH.
   * Bạn cũng có thể cài đặt trình bao Git riêng, với Git cho Windows, chạy dòng sau trong dòng lệnh sẽ lưu thông tin đăng nhập của bạn:
     * `git config --global credential.helper wincred`
***
***
# MARKDOWN
### I.Markdown là gì? Dùng để làm gì ?
  * Markdown là ngôn ngữ đánh dấu văn bản được tạo ra bởi John Gruber. Markdown sử dụng cú pháp khá đơn giản và dễ hiểu để đánh dấu văn bản và văn bản được viết bằng Markdown sẽ có thể được chuyển đổi sang HTML. Ngược lại các văn bản được viết bằng HTML cũng có thể được chuyển đổi sang Markdown.
  * Nó thường được dùng để tạo các tập tin readme, viết tin nhắn trên các diễn đàn, và tạo văn bản có định dạng bằng một trình biên tập văn bản thô.
### II.Các cú pháp thường gặp
1. Tiêu đề
  * Bạn có thể viết các lớp tiêu đề h1, h2, h3 cho đến h6 bằng cách thêm số lượng ký tự # tương ứng vào đầu dòng. Một ký tự # tương đương với h1, 2 ký tự # tương đương với h2 ...
  * Ví dụ:
    ```markdown
    # Tiêu đề 1
    ## Tiêu đề 2
    ### Tiêu đề 3
    #### Tiêu đề 4
    ##### Tiêu đề 5
    ###### Tiêu đề 6
    ```
  > # Tiêu đề 1
  > ## Tiêu đề 2
  > ### Tiêu đề 3
  > #### Tiêu đề 4
  > ##### Tiêu đề 5
  > ###### Tiêu đề 6
2. Định dạng chữ
    ```markdown
    **In đậm**
    *In nghiêng*
    ***In đậm và in nghiêng***
    ~~Chữ gạch ngang~~
    ```
  > **In đậm**
  > *In nghiêng*
  > ***In đậm và in nghiêng***
  > ~~Chữ gạch ngang~~
3. Inline code
  * Sử dụng dấu nháy ngược.
    ```markdown
    `inline code`
    ```
    > `inline`
  * highlight lock code.
    ```
    ```markdown
    ## H2```
    ```
 4. Link, hình ảnh
   * Chèn link
     * `[title](http://~)`
   * Chèn hình ảnh
     * `![alt](http://~)`
 5. List
   * Viết ký tự `*` ở đầu dòng để bắt đầu cho list
      ```
      * list1
      * list2
      * list3
      ```
      > * list1
      > * list2
      > * list3
6. Tạo trích dẫn
    `> Câu trích dẫn`
    > Câu trích dẫn
7. Horizonal rules
  * Sử dụng `***` để tạo horizonal rules
 > `***`
  ***
 > `***`
 > `***`
  ***
  ***
8. Tạo bảng.
```
   | 1 | 2 | 3 |
   |---|---|---|
   | 4 | 5 | 6 |
   | 7 | 8 | 9 |
```
   | 1 | 2 | 3 |
   |---|---|---|
   | 4 | 5 | 6 |
   | 7 | 8 | 9 |
