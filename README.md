# git-safety-foundation
# BÁO CÁO HOÀN THÀNH PROJECT: GIT SAFETY FOUNDATION

## 1. Thông tin cá nhân
- **Họ và tên học viên:** Nguyễn Hữu Sang
- **Trạng thái:** Đã hoàn thành 02 chứng chỉ Microsoft Learn.

---

## 2. Nhật ký quá trình học và thực hành Git
- **Giai đoạn 1:** Học và hoàn thành các module lý thuyết được giao trên Microsoft Learn, nắm vững các khái niệm về Repository, Commit, Branch, Pull Request, và cơ chế quản lý mã nguồn.
- **Giai đoạn 2:** Tạo GitHub repository cá nhân, kết nối local với remote. Thực hành chia nhánh độc lập (`tính năng-1`, `tính năng-2`) để giả lập quy trình làm việc nhóm.
- **Giai đoạn 3:** Thực hành nâng cao về an toàn mã nguồn: Tự tạo tình huống xung đột (Conflict) trên file `nhatky.txt` và tiến hành giải quyết conflict trực tiếp trên GitHub. Thực hành lệnh `git revert` để hoàn tác commit lỗi an toàn mà không làm mất lịch sử dự án.

---

## 3. Danh sách lệnh Git đã sử dụng trong dự án
Dưới đây là các lệnh Git cốt lõi em đã thực hành thành thạo dưới máy tính:
- `git clone <url>`: Tải repository từ GitHub về máy cá nhân.
- `git checkout -b <tên_nhánh>`: Tạo nhánh mới và chuyển sang nhánh đó.
- `git checkout <tên_nhánh>`: Chuyển đổi qua lại giữa các nhánh.
- `git add .`: Lưu lại các thay đổi vào khu vực chờ (Staging Area).
- `git commit -m "tin_nhắn"`: Ghi lại lịch sử thay đổi kèm thông điệp có ý nghĩa.
- `git pull origin <tên_nhánh>`: Cập nhật và kéo code mới nhất từ GitHub về máy.
- `git push origin <tên_nhánh>`: Đẩy code và các nhánh từ máy cá nhân lên GitHub.
- `git reset --hard origin/main`: Ép trạng thái code ở máy đồng bộ sạch sẽ với GitHub khi bị kẹt lỗi.
- `git revert <commit_id>`: Hoàn tác an toàn một commit bị lỗi bằng cách tạo ra một commit đảo ngược.
- `git log --oneline`: Xem lịch sử commit rút gọn để quản lý mã nguồn.

---

## 4. Thu hoạch: Em sẽ dùng Git như thế nào khi Vibe Code với AI?
Khi tham gia khóa học **Vibe Code với AI**, tốc độ sinh code của AI là rất nhanh nhưng cũng tiềm ẩn rủi ro sinh ra code lỗi, code rác hoặc làm phá hỏng các tính năng đang chạy ổn định. Vì vậy, em sẽ áp dụng Git làm **"Hệ thống phanh an toàn"** như sau:
1. **Luôn chia nhánh trước khi gọi AI:** Trước khi nhờ AI viết một tính năng mới, em sẽ tạo một nhánh phụ riêng (ví dụ: `feature-ai`). Tuyệt đối không để AI can thiệp trực tiếp vào nhánh `main`.
2. **Commit nhỏ và có ý nghĩa:** Mỗi khi AI viết xong một đoạn code chạy thử thành công, em sẽ `git commit` ngay lập tức để đánh dấu mốc an toàn.
3. **Sử dụng Revert/Rollback làm cỗ máy thời gian:** Nếu AI sinh code lỗi làm sập hệ thống hoặc gây ra lỗi nghiêm trọng, em sẽ dùng ngay lệnh `git revert` hoặc `git reset` để quay về trạng thái ổn định trước đó chỉ trong vài giây.
4. **Kiểm soát thông qua Pull Request:** Trước khi gộp code của AI vào nhánh chính, em sẽ tận dụng PR trên GitHub để kiểm tra lại dòng code (Code Review), đảm bảo tính an toàn trước khi nghiệm thu.
