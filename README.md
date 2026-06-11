# git-safety-foundation
# BÁO CÁO HOÀN THÀNH PROJECT: GIT SAFETY FOUNDATION

## 1. Thông tin cá nhân
- **Họ và tên học viên:** Nguyễn Hữu Sang
- **Trạng thái:** Đã hoàn thành 02 chứng chỉ Microsoft Learn.

---

## ## 2. Nhật ký quá trình học và thực hành GitHub

### Giai đoạn 1: Tìm hiểu kiến thức cơ bản về Git và GitHub

Trong giai đoạn đầu, em tìm hiểu các khái niệm cơ bản về Git và GitHub như Repository, Commit, Branch, Merge, Pull Request và cơ chế quản lý phiên bản mã nguồn. Đồng thời em thực hành cài đặt Git trên máy tính, cấu hình tài khoản GitHub và làm quen với quy trình làm việc giữa Local Repository và Remote Repository.

### Giai đoạn 2: Xây dựng repository và thực hành quản lý nhánh

Em tạo một repository cá nhân trên GitHub có tên "github-basic-practice" để phục vụ cho bài thực hành. Sau đó tiến hành clone repository về máy tính và xây dựng một dự án website đơn giản.

Trong quá trình thực hành, em đã tạo và sử dụng nhiều nhánh khác nhau để mô phỏng quy trình phát triển phần mềm thực tế, bao gồm:

* main
* feature-homepage
* feature-contact
* feature-footer

Em thực hiện hơn 10 commit với các nội dung cụ thể như tạo cấu trúc dự án, thêm trang chủ, thêm trang liên hệ, cập nhật giao diện, cải thiện bố cục và cập nhật tài liệu hướng dẫn.

### Giai đoạn 3: Thực hành Pull Request, Conflict và Revert

Sau khi hoàn thành các tính năng trên từng nhánh, em tiến hành tạo Pull Request để đề xuất hợp nhất mã nguồn vào nhánh chính. Trong bài thực hành, em đã tạo ít nhất 2 Pull Request:

* Pull Request #1: feature-homepage → main
* Pull Request #2: feature-contact → main

Tiếp theo, em chủ động tạo một tình huống xung đột (Merge Conflict) bằng cách chỉnh sửa cùng một dòng nội dung trong file index.html trên hai nhánh khác nhau. Khi thực hiện merge, Git phát hiện xung đột và yêu cầu xử lý thủ công. Em đã chỉnh sửa lại nội dung phù hợp, đánh dấu hoàn tất và commit phần giải quyết conflict thành công.

Ngoài ra, em còn thực hành hoàn tác một commit bằng lệnh git revert. Sau khi phát hiện commit "Add footer section" có nội dung chưa phù hợp, em sử dụng git revert để tạo một commit mới đảo ngược thay đổi mà vẫn giữ nguyên lịch sử phát triển của dự án.


---


## 3. Danh sách lệnh Git đã sử dụng trong dự án

Dưới đây là các lệnh Git em đã sử dụng trong quá trình thực hành:

* git clone <url>
  Tải repository từ GitHub về máy tính cá nhân.

* git branch
  Kiểm tra danh sách các nhánh hiện có trong dự án.

* git checkout -b <tên_nhánh>
  Tạo nhánh mới và chuyển sang làm việc trên nhánh đó.

* git checkout <tên_nhánh>
  Chuyển đổi giữa các nhánh.

* git add .
  Đưa toàn bộ thay đổi vào vùng Staging Area.

* git commit -m "Tên commit"
  Ghi nhận các thay đổi vào lịch sử dự án.

* git push origin <tên_nhánh>
  Đẩy mã nguồn từ máy tính lên GitHub.

* git pull origin main
  Đồng bộ mã nguồn mới nhất từ GitHub về máy.

* git merge <tên_nhánh>
  Hợp nhất mã nguồn từ một nhánh khác vào nhánh hiện tại.

* git log --oneline
  Xem lịch sử commit dưới dạng rút gọn.

* git revert <commit_id>
  Hoàn tác một commit bằng cách tạo commit đảo ngược.

* git status
  Kiểm tra trạng thái hiện tại của repository.

* git remote -v
  Kiểm tra kết nối giữa repository cục bộ và repository trên GitHub.

---


## 4. Thu hoạch: Em sẽ dùng Git như thế nào khi Vibe Code với AI?

Khi sử dụng AI để hỗ trợ lập trình (Vibe Coding), tốc độ tạo mã nguồn có thể nhanh hơn rất nhiều so với cách lập trình truyền thống. Tuy nhiên, AI đôi khi có thể sinh ra mã nguồn chưa tối ưu, phát sinh lỗi hoặc làm ảnh hưởng đến các chức năng đang hoạt động ổn định của dự án. Vì vậy, em sẽ sử dụng Git như một công cụ quản lý và bảo vệ mã nguồn trong suốt quá trình làm việc với AI.

Trước khi yêu cầu AI phát triển một tính năng mới, em sẽ tạo một nhánh riêng để thực hiện các thay đổi thay vì làm việc trực tiếp trên nhánh main. Điều này giúp em dễ dàng kiểm thử và đánh giá kết quả do AI tạo ra mà không ảnh hưởng đến phiên bản ổn định của dự án.

Trong quá trình phát triển, em sẽ thực hiện các commit thường xuyên với nội dung rõ ràng và có ý nghĩa. Mỗi commit sẽ đánh dấu một mốc hoàn thành cụ thể, giúp em dễ dàng theo dõi lịch sử thay đổi cũng như quay lại phiên bản trước nếu phát hiện lỗi.

Khi AI tạo ra mã nguồn không phù hợp hoặc gây ra lỗi cho hệ thống, em có thể sử dụng các lệnh như git revert hoặc git reset để hoàn tác thay đổi và khôi phục trạng thái hoạt động ổn định của dự án. Đây là một lợi thế rất lớn khi làm việc với lượng mã nguồn được tạo ra nhanh chóng bởi AI.

Bên cạnh đó, em sẽ sử dụng Pull Request để xem xét lại các thay đổi trước khi hợp nhất vào nhánh chính. Việc kiểm tra mã nguồn giúp phát hiện sớm các lỗi logic, lỗi cú pháp hoặc những đoạn mã chưa đáp ứng yêu cầu của dự án.

Qua bài thực hành, em nhận thấy Git đóng vai trò như một "hệ thống an toàn" trong quá trình Vibe Coding với AI. Git không chỉ giúp quản lý lịch sử phát triển phần mềm mà còn hỗ trợ kiểm soát rủi ro, tăng khả năng cộng tác và đảm bảo chất lượng mã nguồn trong các dự án thực tế.

